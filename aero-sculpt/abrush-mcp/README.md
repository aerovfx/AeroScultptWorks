# 🤖 Model Context Protocol (MCP) Integration Guide / Hướng Dẫn Tích Hợp MCP

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

### What is MCP?
The **Model Context Protocol (MCP)** is an open standard that allows AI models (like Claude, Codex, and others) to securely connect to external tools and data sources. By integrating MCP into ABrush, you can enable LLMs to "understand" your 3D scene, automate sculpting tasks, and assist you using natural language.

### Architecture Overview
In this integration:
1. **ABrush acts as an MCP Server:** It exposes its internal API (e.g., changing brushes, executing DynaMesh, reading vertex data) as "Tools" and "Resources".
2. **The LLM acts as an MCP Client:** Apps like Claude Desktop or custom Python scripts using OpenAI Codex will connect to ABrush to read the context and execute commands.

### 1. Setting up the ABrush MCP Server (Rust)
Inside the `abrush-mcp` directory, you can build a lightweight MCP server in Rust using the standard standard input/output (stdio) transport layer.

**Example exposed tools:**
*   `get_active_mesh_info()`: Returns the number of vertices and current polygroup data.
*   `execute_dynamesh(resolution)`: Triggers the DynaMesh remeshing process.
*   `change_matcap(material_name)`: Changes the current display material.

*To implement this, you can use existing Rust MCP SDKs or build a simple JSON-RPC over stdio implementation.*

### 2. Connecting to Claude Desktop
To allow Claude to control ABrush locally, add ABrush as an MCP server in your Claude Desktop configuration file.

**Path:**
*   **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
*   **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

**Configuration Example:**
```json
{
  "mcpServers": {
    "abrush": {
      "command": "/path/to/aero-sculpt/target/release/aero-sculpt-mcp",
      "args": ["--stdio"]
    }
  }
}
```
Once configured, you can ask Claude: *"Analyze my current ABrush scene and apply DynaMesh at resolution 128."*

### 3. Connecting to other LLMs (Codex, GPT-4, etc.)
If you are building a custom client (e.g., a Python script using OpenAI Codex or LangChain), you can use an MCP Client SDK to spawn the ABrush MCP server as a subprocess.

**Python Example using `mcp` library:**
```python
import asyncio
from mcp import ClientSession, StdioServerParameters
from mcp.client.stdio import stdio_client

async def main():
    server_params = StdioServerParameters(
        command="/path/to/aero-sculpt/target/release/aero-sculpt-mcp",
        args=["--stdio"]
    )
    
    async with stdio_client(server_params) as (read, write):
        async with ClientSession(read, write) as session:
            await session.initialize()
            
            # Request ABrush to execute DynaMesh
            result = await session.call_tool("execute_dynamesh", arguments={"resolution": 128})
            print(result)

if __name__ == "__main__":
    asyncio.run(main())
```

---

## Tiếng Việt

### MCP là gì?
**Model Context Protocol (MCP)** là một tiêu chuẩn mở cho phép các mô hình AI (như Claude, Codex, v.v.) kết nối an toàn với các công cụ và nguồn dữ liệu bên ngoài. Bằng cách tích hợp MCP vào ABrush, bạn có thể cấp quyền cho các AI (LLM) "hiểu" được bối cảnh không gian 3D của bạn, tự động hóa các thao tác điêu khắc và trợ giúp bạn thông qua ngôn ngữ tự nhiên.

### Tổng Quan Kiến Trúc
Trong mô hình tích hợp này:
1. **ABrush đóng vai trò là MCP Server:** Cung cấp các API nội bộ (ví dụ: đổi cọ vẽ, chạy DynaMesh, đọc dữ liệu lưới) dưới dạng các "Tools" và "Resources".
2. **LLM đóng vai trò là MCP Client:** Các ứng dụng như Claude Desktop hoặc các script Python tùy chỉnh sử dụng OpenAI Codex sẽ kết nối với ABrush để đọc bối cảnh và ra lệnh thực thi.

### 1. Xây dựng ABrush MCP Server (Rust)
Bên trong thư mục `abrush-mcp`, bạn có thể xây dựng một MCP Server gọn nhẹ bằng Rust, sử dụng giao thức giao tiếp qua standard input/output (stdio).

**Ví dụ một số công cụ (tools) có thể cung cấp:**
*   `get_active_mesh_info()`: Trả về số lượng đỉnh (vertices) và dữ liệu polygroup hiện tại.
*   `execute_dynamesh(resolution)`: Kích hoạt quá trình tái cấu trúc lưới DynaMesh.
*   `change_matcap(material_name)`: Đổi chất liệu hiển thị của mô hình.

### 2. Kết nối với Claude Desktop
Để Claude có thể tương tác với ABrush trên máy tính của bạn, hãy thêm ABrush làm một MCP server trong file cấu hình của Claude Desktop.

**Đường dẫn cấu hình:**
*   **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
*   **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

**Ví dụ file cấu hình:**
```json
{
  "mcpServers": {
    "abrush": {
      "command": "/duong/dan/toi/aero-sculpt/target/release/aero-sculpt-mcp",
      "args": ["--stdio"]
    }
  }
}
```
Sau khi cấu hình, bạn có thể chat với Claude: *"Hãy phân tích bối cảnh ABrush hiện tại của tôi và chạy DynaMesh với độ phân giải 128."*

### 3. Kết nối với các LLM khác (Codex, GPT-4, v.v.)
Nếu bạn đang lập trình một ứng dụng Client tùy chỉnh (ví dụ: dùng Python với OpenAI Codex hay LangChain), bạn có thể dùng các thư viện MCP Client để gọi ABrush MCP server như một tiến trình con (subprocess).

**Ví dụ Python sử dụng thư viện `mcp`:**
```python
import asyncio
from mcp import ClientSession, StdioServerParameters
from mcp.client.stdio import stdio_client

async def main():
    server_params = StdioServerParameters(
        command="/duong/dan/toi/aero-sculpt/target/release/aero-sculpt-mcp",
        args=["--stdio"]
    )
    
    async with stdio_client(server_params) as (read, write):
        async with ClientSession(read, write) as session:
            await session.initialize()
            
            # Ra lệnh cho ABrush chạy DynaMesh
            result = await session.call_tool("execute_dynamesh", arguments={"resolution": 128})
            print(result)

if __name__ == "__main__":
    asyncio.run(main())
```

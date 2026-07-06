# 🚀 Installation Guide / Hướng Dẫn Cài Đặt ABrush

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

ABrush currently provides standalone builds for **macOS** and **Windows**. You can install it in two ways: download a pre-built binary or build it yourself from the source code.

### Method 1: Install from Pre-built Binaries (Recommended)

This is the fastest way to experience ABrush without installing any programming tools.

#### For Windows
1. Go to the project's **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** page on GitHub.
2. Download the latest `.zip` file for Windows (e.g., `aero-sculpt-windows-x64.zip`).
3. Extract the downloaded file to any folder on your computer.
4. Open the extracted folder and run `aero-sculpt.exe` to get started!

#### For macOS
1. Go to the project's **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** page on GitHub.
2. Download the latest `.zip` file for macOS (e.g., `aero-sculpt-macos.zip`).
3. Extract the downloaded file.
4. Drag and drop the `AeroSculpt.app` into your **Applications** folder.
5. Open the app from the Applications folder or Launchpad.
   *Note: If macOS shows a security warning, go to **System Settings > Privacy & Security**, scroll to the bottom, and select "Open Anyway".*

### Method 2: Build from Source (For Developers)

Since ABrush is written entirely in **Rust**, you can easily compile it directly on your machine.

#### System Requirements:
* **Rust** and **Cargo** installed. (If not, download from [rustup.rs](https://rustup.rs/)).
* Git.

#### Steps:
1. **Clone the project:**
   ```bash
   git clone https://github.com/USERNAME/aero-sculpt.git
   cd aero-sculpt
   ```
2. **Run the application:**
   Execute the following command to build and launch ABrush with maximum performance:
   ```bash
   cargo run --release
   ```
   *(Note: The `--release` flag is required to run the app smoothly at 60 FPS; avoid using debug mode to prevent lag).*

### Minimum System Requirements
* **OS:** Windows 10/11, macOS 11 or later.
* **CPU:** Multi-core processor.
* **RAM:** Minimum 4GB.
* **GPU:** wgpu support (Vulkan/Metal/DX12) - compatible with most modern graphics cards.
* **Accessories:** A graphics tablet (Wacom, Huion, XP-Pen) is highly recommended for the best pressure-sensitive experience.

---

## Tiếng Việt

ABrush hiện đã hỗ trợ các bản build độc lập (standalone) cho hệ điều hành **macOS** và **Windows**. Bạn có thể cài đặt theo hai cách: tải bản build sẵn hoặc tự build từ mã nguồn.

### Cách 1: Cài Đặt Từ Bản Build Sẵn (Khuyên dùng)

Đây là cách nhanh nhất để trải nghiệm ABrush mà không cần cài đặt thêm bất kỳ công cụ lập trình nào.

#### Dành cho Windows
1. Truy cập trang **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** của dự án trên GitHub.
2. Tải xuống file nén mới nhất dành cho Windows (ví dụ: `aero-sculpt-windows-x64.zip`).
3. Giải nén file vừa tải về vào một thư mục bất kỳ trên máy tính của bạn.
4. Mở thư mục vừa giải nén và chạy file `aero-sculpt.exe` để bắt đầu!

#### Dành cho macOS
1. Truy cập trang **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** của dự án trên GitHub.
2. Tải xuống file nén mới nhất dành cho macOS (ví dụ: `aero-sculpt-macos.zip`).
3. Giải nén file vừa tải về.
4. Kéo thả ứng dụng `AeroSculpt.app` vào thư mục **Applications**.
5. Mở ứng dụng từ thư mục Applications hoặc Launchpad.
   *Lưu ý: Nếu macOS hiện thông báo bảo mật, hãy vào **System Settings > Privacy & Security**, kéo xuống dưới cùng và chọn "Open Anyway" (Vẫn mở).*

### Cách 2: Tự Build Từ Mã Nguồn (Dành cho Lập trình viên)

Vì ABrush được viết hoàn toàn bằng **Rust**, bạn có thể dễ dàng tự compile trực tiếp trên máy của mình.

#### Yêu cầu hệ thống:
* Đã cài đặt **Rust** và **Cargo**. (Nếu chưa, tải tại [rustup.rs](https://rustup.rs/)).
* Git.

#### Các bước thực hiện:
1. **Clone dự án:**
   ```bash
   git clone https://github.com/USERNAME/aero-sculpt.git
   cd aero-sculpt
   ```
2. **Khởi chạy ứng dụng:**
   Chạy lệnh sau để build và khởi động ABrush với hiệu năng tối đa:
   ```bash
   cargo run --release
   ```
   *(Lưu ý: Bắt buộc phải có cờ `--release` để ứng dụng chạy mượt mà ở mức 60 FPS, không dùng chế độ debug vì sẽ bị giật lag).*

### Yêu Cầu Cấu Hình Cơ Bản
* **Hệ điều hành:** Windows 10/11, macOS 11 trở lên.
* **CPU:** Đa nhân cơ bản.
* **RAM:** Tối thiểu 4GB.
* **GPU:** Hỗ trợ wgpu (Vulkan/Metal/DX12) - tương thích với hầu hết card đồ họa hiện đại.
* **Thiết bị phụ trợ:** Khuyên dùng bảng vẽ điện tử (Wacom, Huion, XP-Pen) để có trải nghiệm cảm ứng lực nhấn tốt nhất.

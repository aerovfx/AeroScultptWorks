# ⚙️ ABrush Core API Reference / Tài Liệu API Lõi

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

The ABrush API allows developers, plugin creators, and AI integrations (like MCP) to interact directly with the ABrush sculpting engine. This API can be accessed via **Rust (native)** or exposed via **JSON-RPC/C-FFI** for external scripts.

### 1. Mesh & Topology Operations
Functions to interact with the 3D geometry of the object.

*   **`get_mesh_stats()`**
    *   **Returns:** JSON/Struct containing `vertex_count`, `face_count`, and `active_polygroup_count`.
    *   **Description:** Retrieves the current statistics of the active SubTool.
*   **`execute_dynamesh(resolution: u32)`**
    *   **Returns:** `boolean` (Success/Failure).
    *   **Description:** Recalculates the mesh using the Voxel Remesh algorithm at the specified resolution (e.g., 128, 256).
*   **`subdivide(levels: u8)`**
    *   **Returns:** `boolean`.
    *   **Description:** Applies Catmull-Clark subdivision to increase mesh density.

### 2. Brush Management
Functions to control the sculpting tools programmatically.

*   **`set_active_brush(brush_name: String)`**
    *   **Description:** Changes the current brush. Valid inputs: `"Standard"`, `"Clay"`, `"ClayBuildup"`, `"Move"`, `"Smooth"`, `"DamStandard"`, etc.
*   **`set_brush_parameters(size: f32, intensity: f32)`**
    *   **Description:** Sets the radius and the strength/intensity of the active brush.
*   **`toggle_symmetry(axis: String)`**
    *   **Description:** Toggles mirror symmetry. Valid inputs: `"X"`, `"Y"`, `"Z"`, or `"None"`.

### 3. Scene & File I/O
Functions to manage the workspace and import/export data.

*   **`load_model(file_path: String)`**
    *   **Returns:** `mesh_id`.
    *   **Description:** Imports a 3D model (e.g., `.obj`) into the scene.
*   **`export_model(file_path: String, export_colors: bool)`**
    *   **Returns:** `boolean`.
    *   **Description:** Exports the current active mesh to the specified path. `export_colors` determines if vertex colors/Polygroups are saved.
*   **`set_matcap(matcap_index: u8)`**
    *   **Description:** Applies a specific Material Capture (MatCap) to the scene (Range: 0-20).

---

## Tiếng Việt

ABrush API cho phép các nhà phát triển, người tạo plugin và các hệ thống AI (như MCP) tương tác trực tiếp với engine điêu khắc của ABrush. API này có thể được gọi thông qua **Rust (native)** hoặc qua **JSON-RPC/C-FFI** dành cho các script bên ngoài.

### 1. Thao Tác Lưới (Mesh & Topology)
Các hàm tương tác với hình học 3D của vật thể.

*   **`get_mesh_stats()`**
    *   **Trả về:** JSON/Struct chứa `vertex_count` (số lượng đỉnh), `face_count` (số lượng mặt), và `active_polygroup_count` (số lượng nhóm).
    *   **Mô tả:** Lấy các thông số thống kê của công cụ (SubTool) hiện tại đang được chọn.
*   **`execute_dynamesh(resolution: u32)`**
    *   **Trả về:** `boolean` (Thành công/Thất bại).
    *   **Mô tả:** Tái cấu trúc lưới bằng thuật toán Voxel Remesh ở độ phân giải được chỉ định (ví dụ: 128, 256).
*   **`subdivide(levels: u8)`**
    *   **Trả về:** `boolean`.
    *   **Mô tả:** Áp dụng thuật toán chia nhỏ Catmull-Clark để tăng mật độ chi tiết lưới.

### 2. Quản Lý Cọ Vẽ (Brush Management)
Các hàm điều khiển công cụ điêu khắc bằng code.

*   **`set_active_brush(brush_name: String)`**
    *   **Mô tả:** Thay đổi cọ vẽ hiện tại. Đầu vào hợp lệ: `"Standard"`, `"Clay"`, `"ClayBuildup"`, `"Move"`, `"Smooth"`, `"DamStandard"`, v.v.
*   **`set_brush_parameters(size: f32, intensity: f32)`**
    *   **Mô tả:** Cài đặt bán kính (size) và cường độ (intensity) của cọ vẽ hiện hành.
*   **`toggle_symmetry(axis: String)`**
    *   **Mô tả:** Bật/tắt chế độ điêu khắc đối xứng. Đầu vào hợp lệ: `"X"`, `"Y"`, `"Z"`, hoặc `"None"`.

### 3. Quản Lý File & Không Gian (Scene & I/O)
Các hàm quản lý môi trường làm việc và nhập/xuất dữ liệu.

*   **`load_model(file_path: String)`**
    *   **Trả về:** `mesh_id`.
    *   **Mô tả:** Nhập một mô hình 3D (ví dụ: file `.obj`) vào trong không gian làm việc.
*   **`export_model(file_path: String, export_colors: bool)`**
    *   **Trả về:** `boolean`.
    *   **Mô tả:** Xuất lưới 3D hiện tại ra đường dẫn chỉ định. Biến `export_colors` quyết định việc có lưu kèm màu sắc đỉnh (Vertex Colors) hay không.
*   **`set_matcap(matcap_index: u8)`**
    *   **Mô tả:** Đổi chất liệu hiển thị (MatCap) cho khung cảnh (Giá trị từ: 0-20).

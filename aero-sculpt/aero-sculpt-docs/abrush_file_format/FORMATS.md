# 📂 Supported File Formats / Các Định Dạng Hỗ Trợ (ABrush)

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

ABrush focuses on lightweight, standard 3D formats rather than complex, proprietary ones. Below is the current status of file format support in ABrush.

### 1. Fully Supported Formats (Import & Export)

*   **Wavefront OBJ (`.obj`)**
    *   **Status:** ✅ Fully Supported (Import & Export)
    *   **Details:** ABrush supports importing and exporting standard `.obj` files. Uniquely, it also supports exporting **Vertex Colors** within the OBJ format, allowing you to retain all Polygroup and painted color data.
    *   **Features:**
        *   Preserves Vertex Colors upon export.
        *   Option to apply or discard Subdivision levels when exporting.
        *   Welding / Unwelding of vertices options.
        *   Retains Polygroup data.

### 2. Upcoming Formats

*   **ABrush Native (`.abr`)**
    *   **Status:** 📅 Upcoming
    *   **Details:** The native format for ABrush. It will allow saving and loading complete project states efficiently.

### 3. Planned Formats

*   **STL (`.stl`)**
    *   **Status:** 📅 Planned (UI ready)
    *   **Details:** Essential for 3D printing workflows.
*   **GLB / glTF (`.glb`, `.gltf`)**
    *   **Status:** 📅 Planned (UI ready)
    *   **Details:** The standard for web and real-time 3D applications.
*   **PLY (`.ply`)**
    *   **Status:** 📅 Planned (UI ready)
    *   **Details:** Polygon File Format, excellent for storing 3D scanner data and vertex colors.

---

## Tiếng Việt

ABrush tập trung vào các định dạng 3D tiêu chuẩn và nhẹ nhàng, thay vì các định dạng độc quyền phức tạp. Dưới đây là trạng thái hỗ trợ các định dạng file trong ABrush.

### 1. Hỗ Trợ Hoàn Toàn (Nhập & Xuất)

*   **Wavefront OBJ (`.obj`)**
    *   **Trạng thái:** ✅ Hỗ trợ hoàn toàn (Import & Export)
    *   **Chi tiết:** ABrush hỗ trợ nhập và xuất file `.obj` tiêu chuẩn. Đặc biệt, ứng dụng hỗ trợ lưu trữ **Vertex Colors** (Màu sắc đỉnh) ngay bên trong file OBJ, giúp bạn giữ nguyên mọi dữ liệu màu sắc và Polygroup.
    *   **Tính năng khi Export:**
        *   Giữ nguyên Vertex Colors.
        *   Tùy chọn xuất file theo mức độ Subdivision (độ mịn lưới) mong muốn.
        *   Tùy chọn Welding / Unwelding (Hàn/tách đỉnh).
        *   Giữ nguyên dữ liệu các nhóm Polygroup.

### 2. Định Dạng Sắp Ra Mắt

*   **ABrush Native (`.abr`)**
    *   **Trạng thái:** 📅 Sắp có
    *   **Chi tiết:** Định dạng file nguồn gốc của ABrush. Giúp lưu trữ và tải toàn bộ trạng thái dự án một cách tối ưu nhất.

### 3. Định Dạng Trong Kế Hoạch Phát Triển

*   **STL (`.stl`)**
    *   **Trạng thái:** 📅 Kế hoạch (Giao diện UI đã sẵn sàng)
    *   **Chi tiết:** Định dạng thiết yếu dành cho quy trình in 3D.
*   **GLB / glTF (`.glb`, `.gltf`)**
    *   **Trạng thái:** 📅 Kế hoạch (Giao diện UI đã sẵn sàng)
    *   **Chi tiết:** Định dạng tiêu chuẩn cho web và ứng dụng 3D thời gian thực.
*   **PLY (`.ply`)**
    *   **Trạng thái:** 📅 Kế hoạch (Giao diện UI đã sẵn sàng)
    *   **Chi tiết:** Định dạng xuất sắc để lưu trữ dữ liệu quét 3D và màu sắc đỉnh.

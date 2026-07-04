# <img src="aero-sculpt/aero-sculpt-assets/logo.jpg" width="40" height="40" align="center"> AeroSculpt (ABrush)

AeroSculpt (tên mã ABrush) là một ứng dụng điêu khắc 3D thế hệ mới, được viết hoàn toàn bằng ngôn ngữ Rust. Nó được thiết kế nhằm mang lại hiệu năng siêu việt, mượt mà và giao diện tối giản để giải phóng sự sáng tạo của bạn khỏi những công cụ nặng nề.

Dự án này là nỗ lực tạo ra một công cụ điêu khắc độc quyền, hoạt động trơn tru đa nền tảng (Windows, macOS) mà không đòi hỏi tài nguyên hệ thống quá khắt khe.

## 📸 Giao Diện Ứng Dụng

<p align="center">
  <img src="aero-sculpt/aero-sculpt-assets/screenshot1.png" width="45%" />
  <img src="aero-sculpt/aero-sculpt-assets/screenshot2.png" width="45%" />
</p>


## 📁 Cấu Trúc Dự Án

*   **`aero-sculpt/aero-sculpt-docs/`**: Chứa toàn bộ tài liệu, hướng dẫn sử dụng và cài đặt ứng dụng.
    *   [Hướng Dẫn Cài Đặt (INSTALLATION.md)](aero-sculpt/aero-sculpt-docs/INSTALLATION.md)
    *   [Hướng Dẫn Sử Dụng Cơ Bản (USAGE.md)](aero-sculpt/aero-sculpt-docs/USAGE.md)
    *   [Hệ Thống Phím Tắt (SHORTCUTS.md)](aero-sculpt/aero-sculpt-docs/SHORTCUTS.md)
*   **`aero-sculpt/aero-sculpt-assets/`**: Chứa các tài nguyên, hình ảnh, icon và MatCap cho ứng dụng.
*   **`aero-sculpt/aero-sculpt-examples/`**: Các file dự án mẫu `.obj` để người dùng tham khảo.
*   **`aero-sculpt/aero-sculpt-sdk/`**: Bộ công cụ phát triển phần mềm cho các ứng dụng hoặc plugin bên thứ 3.
*   **`aero-sculpt/aero-sculpt-api/`**: Tài liệu API tích hợp.

## 🚀 Tính Năng Nổi Bật
*   **DynaMesh (Voxel Remesh)**: Tái cấu trúc lưới 3D chỉ với một thao tác.
*   **Sculptris Pro**: Điêu khắc thông minh, tự động tăng chi tiết tại vị trí cọ vẽ.
*   **Polygroup**: Quản lý các bộ phận theo màu sắc dễ dàng.
*   **Hỗ trợ Wacom / Bảng vẽ**: Nhận diện áp lực bút cảm ứng mượt mà.

---

*Hãy cầm bút cảm ứng lên và bắt đầu nặn ra những tác phẩm nghệ thuật 3D tuyệt vời cùng AeroSculpt!*

# <img src="aero-sculpt/aero-sculpt-assets/logo.jpg" width="40" height="40" align="center"> AeroSculpt (ABrush)

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

AeroSculpt (codename ABrush) is a next-generation 3D sculpting application, written entirely in Rust. It is designed to deliver superior performance, smooth operation, and a minimalist interface to free your creativity from heavy, cumbersome tools.

This project is an effort to create an exclusive, cross-platform (Desktop App, Mobile App) sculpting tool that runs smoothly without requiring highly demanding system resources.

### 📸 App Interface

<p align="center">
  <img src="aero-sculpt/aero-sculpt-assets/screenshot1.png" width="45%" />
  <img src="aero-sculpt/aero-sculpt-assets/screenshot2.png" width="45%" />
</p>

### 📁 Project Structure

*   **`aero-sculpt/aero-sculpt-docs/`**: Contains all documentation, usage instructions, and installation guides.
    *   [Installation Guide (INSTALLATION.md)](aero-sculpt/aero-sculpt-docs/INSTALLATION.md)
    *   [Basic Usage (USAGE.md)](aero-sculpt/aero-sculpt-docs/USAGE.md)
    *   [Shortcuts System (SHORTCUTS.md)](aero-sculpt/aero-sculpt-docs/SHORTCUTS.md)
    *   [Development Roadmap (ROADMAP.md)](ROADMAP.md)
*   **`aero-sculpt/aero-sculpt-assets/`**: Contains resources, images, icons, and MatCaps for the app.
*   **`aero-sculpt/aero-sculpt-examples/`**: Sample `.obj` project files for reference.
*   **`aero-sculpt/aero-sculpt-sdk/`**: Software Development Kit for third-party apps or plugins.
*   **`aero-sculpt/aero-sculpt-api/`**: Integrated API documentation.
*   **`aero-sculpt/abrush-mcp/`**: Model Context Protocol integration directory.

### 🗺️ Development Roadmap Summary
*   **Phase 1 (Current)**: Core sculpting engine, DynaMesh, and essential UI on Desktop.
*   **Phase 2**: Native `.abr` format, new 3D export options (STL/GLB), Mobile App optimization, and deep integration with the **Pixibox.ai** 3D generation workflow.
*   **Phase 3**: AI Integration via MCP (Claude/Codex) and Plugin SDK.
*   **Phase 4**: WebAssembly (WASM) browser version and Real-time PBR Rendering.
*(See full details in [ROADMAP.md](ROADMAP.md))*

### 🚀 Key Features & Core Philosophy
*   **Ultra-Lightweight Engine**: Optimized with Rust, ABrush runs smoothly on lower-end hardware while handling millions of polygons without lag.
*   **High-Poly Sculpting Focus**: Designed primarily for generating ultra-detailed high-poly meshes, giving you the freedom to sculpt organic shapes, intricate textures, and complex character designs effortlessly.
*   **Manual Retopology for Low-Poly**: Streamlined tools to help artists perform manual retopology over high-poly sculpts, creating clean, game-ready low-poly meshes with perfect edge flow.
*   **DynaMesh (Voxel Remesh)**: Reconstruct 3D meshes with a single action.
*   **Sculptris Pro**: Smart sculpting that automatically increases detail at the brush location.
*   **Polygroup**: Easily manage different parts by color.
*   **Wacom / Drawing Tablet Support**: Smooth stylus pressure recognition.

### ❤️ Support the Developer
If you love ABrush and want to support its continuous development, consider buying me a coffee! Your donations keep this project alive and independent. Choose a donation amount that feels right for you:

[![Donate $10](https://img.shields.io/badge/Donate-$10-blue.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development&amount=10.00)
[![Donate $5](https://img.shields.io/badge/Donate-$5-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development&amount=5.00)
[![Donate Custom Amount](https://img.shields.io/badge/Donate-Custom_Amount-orange.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development)

---

*Pick up your stylus and start sculpting amazing 3D artworks with AeroSculpt today!*

---

## Tiếng Việt

AeroSculpt (tên mã ABrush) là một ứng dụng điêu khắc 3D thế hệ mới, được viết hoàn toàn bằng ngôn ngữ Rust. Nó được thiết kế nhằm mang lại hiệu năng siêu việt, mượt mà và giao diện tối giản để giải phóng sự sáng tạo của bạn khỏi những công cụ nặng nề.

Dự án này là nỗ lực tạo ra một công cụ điêu khắc độc quyền, hoạt động trơn tru đa nền tảng (Desktop App, Mobile App) mà không đòi hỏi tài nguyên hệ thống quá khắt khe.

### 📸 Giao Diện Ứng Dụng

<p align="center">
  <img src="aero-sculpt/aero-sculpt-assets/screenshot1.png" width="45%" />
  <img src="aero-sculpt/aero-sculpt-assets/screenshot2.png" width="45%" />
</p>

### 📁 Cấu Trúc Dự Án

*   **`aero-sculpt/aero-sculpt-docs/`**: Chứa toàn bộ tài liệu, hướng dẫn sử dụng và cài đặt ứng dụng.
    *   [Hướng Dẫn Cài Đặt (INSTALLATION.md)](aero-sculpt/aero-sculpt-docs/INSTALLATION.md)
    *   [Hướng Dẫn Sử Dụng Cơ Bản (USAGE.md)](aero-sculpt/aero-sculpt-docs/USAGE.md)
    *   [Hệ Thống Phím Tắt (SHORTCUTS.md)](aero-sculpt/aero-sculpt-docs/SHORTCUTS.md)
    *   [Lộ Trình Phát Triển (ROADMAP.md)](ROADMAP.md)
*   **`aero-sculpt/aero-sculpt-assets/`**: Chứa các tài nguyên, hình ảnh, icon và MatCap cho ứng dụng.
*   **`aero-sculpt/aero-sculpt-examples/`**: Các file dự án mẫu `.obj` để người dùng tham khảo.
*   **`aero-sculpt/aero-sculpt-sdk/`**: Bộ công cụ phát triển phần mềm cho các ứng dụng hoặc plugin bên thứ 3.
*   **`aero-sculpt/aero-sculpt-api/`**: Tài liệu API tích hợp.
*   **`aero-sculpt/abrush-mcp/`**: Thư mục dành riêng cho việc tích hợp Model Context Protocol (MCP).

### 🗺️ Tóm Tắt Lộ Trình Phát Triển
*   **Giai đoạn 1 (Hiện tại)**: Hoàn thiện engine lõi, DynaMesh và giao diện cơ bản trên Desktop.
*   **Giai đoạn 2**: Ra mắt định dạng gốc `.abr`, mở rộng xuất file in 3D (STL/GLB), tối ưu hóa Mobile App, và tích hợp sâu với quy trình Gen 3D của **Pixibox.ai**.
*   **Giai đoạn 3**: Tích hợp AI qua giao thức MCP (Claude/Codex) và phát hành Plugin SDK.
*   **Giai đoạn 4**: Hỗ trợ nền tảng Web qua WebAssembly (WASM) và Render PBR chân thực.
*(Xem chi tiết đầy đủ tại [ROADMAP.md](ROADMAP.md))*

### 🚀 Tính Năng Nổi Bật & Triết Lý Cốt Lõi
*   **Siêu Nhẹ & Tối Ưu (Ultra-Lightweight)**: Được lập trình bằng Rust, ABrush hoạt động cực kỳ mượt mà ngay cả trên phần cứng giới hạn, xử lý hàng triệu đa giác (polygons) mà không giật lag.
*   **Tập Trung Sculpt High-Poly**: Thiết kế chuyên biệt để tạo ra các mô hình High-Poly cực kỳ chi tiết. Ứng dụng cung cấp sự tự do tuyệt đối để điêu khắc bề mặt hữu cơ, nếp nhăn và nhân vật phức tạp.
*   **Hỗ Trợ Retopo Thủ Công (Low-Poly)**: Quy trình làm việc được thiết kế để bạn có thể dễ dàng thực hiện Retopology (vẽ lại lưới) thủ công trên bề mặt mô hình High-Poly, từ đó tạo ra các mô hình Low-Poly sạch sẽ, tối ưu hoàn hảo cho Game và Animation.
*   **DynaMesh (Voxel Remesh)**: Tái cấu trúc lưới 3D chỉ với một thao tác.
*   **Sculptris Pro**: Điêu khắc thông minh, tự động tăng chi tiết tại vị trí cọ vẽ.
*   **Polygroup**: Quản lý các bộ phận theo màu sắc dễ dàng.
*   **Hỗ trợ Wacom / Bảng vẽ**: Nhận diện áp lực bút cảm ứng mượt mà.

### ❤️ Ủng Hộ Nhà Phát Triển
Nếu bạn yêu thích ABrush và muốn ủng hộ quá trình phát triển liên tục của phần mềm, hãy cân nhắc mời tôi một ly cà phê nhé! Những đóng góp của bạn là động lực to lớn giúp dự án này tồn tại và duy trì tính độc lập. Chọn một mức ủng hộ phù hợp với bạn:

[![Donate $10](https://img.shields.io/badge/Donate-$10-blue.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development&amount=10.00)
[![Donate $5](https://img.shields.io/badge/Donate-$5-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development&amount=5.00)
[![Donate Tùy Chọn](https://img.shields.io/badge/Donate-M%E1%BB%A9c_T%C3%B9y_Ch%E1%BB%8Dn-orange.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=thegioithu2@gmail.com&item_name=Support+ABrush+Development)

---

*Hãy cầm bút cảm ứng lên và bắt đầu nặn ra những tác phẩm nghệ thuật 3D tuyệt vời cùng AeroSculpt!*

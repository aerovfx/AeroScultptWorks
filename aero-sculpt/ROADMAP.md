# 🗺️ ABrush Development Roadmap / Lộ Trình Phát Triển

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

Welcome to the ABrush development roadmap! Our vision is to make ABrush the fastest, most lightweight, and intuitive 3D sculpting software. Below are the key milestones we are aiming for:

### Phase 1: Core Foundation (Current Phase) 🟢
*   [x] Ultra-lightweight Rust engine setup.
*   [x] Core high-poly sculpting brushes (Standard, Clay, Move, Smooth, etc.).
*   [x] DynaMesh (Voxel Remesh) and Sculptris Pro implementation.
*   [x] Basic Polygroup management and masking.
*   [x] OBJ Import/Export with Vertex Colors.
*   [x] Comprehensive bilingual documentation.

### Phase 2: Workflow Expansion (Q3-Q4 2026) 🟡
*   [ ] **Native File Format**: Implement `.abr` (ABrush Native) for saving complete project states.
*   [ ] **More File Formats**: Support for `.stl` (3D Printing), `.glb/.gltf` (Web/AR), and `.ply`.
*   [ ] **Manual Retopology Tools**: Advanced snapping and drawing tools for creating clean low-poly meshes over high-poly sculpts.
*   [ ] **Custom MatCaps**: Allow users to import their own MatCap materials.
*   [ ] **Pixibox.ai Integration**: Develop deep integration with the Pixibox.ai 3D generation workflow for seamless asset transfer and refinement.

### Phase 3: AI & Extensibility (2027) 🔵
*   [ ] **MCP Integration**: Fully functional Model Context Protocol integration, allowing AI (like Claude/Codex) to assist with sculpting and mesh analysis.
*   [ ] **Plugin SDK**: Release Python/C++ bindings for third-party developers to create custom tools.
*   [ ] **Advanced Slicing**: Basic preparation tools for 3D printing directly within ABrush.

### Phase 4: The Future 🟣
*   [ ] **WASM / Web Version**: Bring ABrush to the browser using WebAssembly.
*   [ ] **PBR Rendering**: Real-time Physically Based Rendering (PBR) viewport.
*   [ ] **Cloud Sync & Collaboration**: Multi-user sculpting sessions.

---

## Tiếng Việt

Chào mừng bạn đến với lộ trình phát triển của ABrush! Tầm nhìn của chúng tôi là đưa ABrush trở thành phần mềm điêu khắc 3D nhanh nhất, nhẹ nhất và trực quan nhất. Dưới đây là các cột mốc quan trọng:

### Giai Đoạn 1: Nền Tảng Cốt Lõi (Hiện Tại) 🟢
*   [x] Xây dựng engine lõi bằng Rust siêu nhẹ.
*   [x] Các cọ điêu khắc High-Poly cơ bản (Standard, Clay, Move, Smooth...).
*   [x] Tích hợp DynaMesh (Voxel Remesh) và Sculptris Pro.
*   [x] Quản lý mặt nạ (Masking) và Polygroup cơ bản.
*   [x] Nhập/Xuất file OBJ kèm theo màu sắc đỉnh (Vertex Colors).
*   [x] Hệ thống tài liệu hướng dẫn song ngữ chi tiết.

### Giai Đoạn 2: Mở Rộng Quy Trình (Q3-Q4 2026) 🟡
*   [ ] **Định Dạng File Gốc**: Hoàn thiện định dạng `.abr` (ABrush Native) để lưu trữ trạng thái toàn bộ dự án.
*   [ ] **Hỗ Trợ Thêm Định Dạng**: Mở rộng xuất file `.stl` (In 3D), `.glb/.gltf` (Web/AR), và `.ply`.
*   [ ] **Công Cụ Retopo Thủ Công**: Cung cấp công cụ bắt dính (snapping) và vẽ lưới tiên tiến để tạo Low-Poly sạch sẽ trên bề mặt High-Poly.
*   [ ] **Custom MatCap**: Cho phép người dùng tự tải lên các chất liệu MatCap tùy chỉnh.
*   [ ] **Tích Hợp Pixibox.ai**: Phát triển kết nối trực tiếp với Pixibox.ai (ứng dụng Gen 3D) để dễ dàng chuyển đổi và tinh chỉnh các mô hình 3D được tạo bởi AI.

### Giai Đoạn 3: Trí Tuệ Nhân Tạo & Tiện Ích Mở Rộng (2027) 🔵
*   [ ] **Tích Hợp MCP**: Hoàn thiện Model Context Protocol, cho phép AI (Claude/Codex) hỗ trợ điêu khắc, tự động hóa và phân tích lưới 3D.
*   [ ] **Plugin SDK**: Phát hành SDK (Python/C++) để các lập trình viên bên thứ ba có thể tự tạo công cụ riêng.
*   [ ] **Công Cụ Slicing**: Hỗ trợ cắt lớp (slicing) cơ bản để phục vụ trực tiếp cho máy in 3D.

### Giai Đoạn 4: Tương Lai Xa 🟣
*   [ ] **Phiên Bản Web (WASM)**: Đưa ABrush lên trình duyệt web thông qua WebAssembly.
*   [ ] **Render PBR**: Tích hợp engine hiển thị vật lý chân thực (Physically Based Rendering) theo thời gian thực.
*   [ ] **Đồng Bộ Đám Mây & Làm Việc Nhóm**: Hỗ trợ nhiều người cùng điêu khắc trên một không gian làm việc.

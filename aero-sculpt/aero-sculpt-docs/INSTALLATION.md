# 🚀 Hướng Dẫn Cài Đặt AeroSculpt (ABrush)

AeroSculpt (tên mã ABrush) hiện đã hỗ trợ các bản build độc lập (standalone) cho hệ điều hành **macOS** và **Windows**. Bạn có thể cài đặt theo hai cách: tải bản build sẵn hoặc tự build từ mã nguồn.

---

## Cách 1: Cài Đặt Từ Bản Build Sẵn (Khuyên dùng)

Đây là cách nhanh nhất để trải nghiệm AeroSculpt mà không cần cài đặt thêm bất kỳ công cụ lập trình nào.

### Dành cho Windows
1. Truy cập trang **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** của dự án trên GitHub.
2. Tải xuống file nén mới nhất dành cho Windows (ví dụ: `aero-sculpt-windows-x64.zip`).
3. Giải nén file vừa tải về vào một thư mục bất kỳ trên máy tính của bạn.
4. Mở thư mục vừa giải nén và chạy file `aero-sculpt.exe` để bắt đầu!

### Dành cho macOS
1. Truy cập trang **[Releases](https://github.com/USERNAME/aero-sculpt/releases)** của dự án trên GitHub.
2. Tải xuống file nén mới nhất dành cho macOS (ví dụ: `aero-sculpt-macos.zip`).
3. Giải nén file vừa tải về.
4. Kéo thả ứng dụng `AeroSculpt.app` vào thư mục **Applications**.
5. Mở ứng dụng từ thư mục Applications hoặc Launchpad.
   *Lưu ý: Nếu macOS hiện thông báo bảo mật (do app chưa được sign), hãy vào **System Settings > Privacy & Security**, kéo xuống dưới cùng và chọn "Open Anyway" (Vẫn mở).*

---

## Cách 2: Tự Build Từ Mã Nguồn (Dành cho Lập trình viên)

Vì AeroSculpt được viết hoàn toàn bằng **Rust**, bạn có thể dễ dàng tự compile trực tiếp trên máy của mình.

### Yêu cầu hệ thống:
* Đã cài đặt **Rust** và **Cargo**. (Nếu chưa, tải tại [rustup.rs](https://rustup.rs/)).
* Git.

### Các bước thực hiện:
1. **Clone dự án:**
   ```bash
   git clone https://github.com/USERNAME/aero-sculpt.git
   cd aero-sculpt
   ```
2. **Khởi chạy ứng dụng:**
   Chạy lệnh sau để build và khởi động AeroSculpt với hiệu năng tối đa:
   ```bash
   cargo run --release
   ```
   *(Lưu ý: Bắt buộc phải có cờ `--release` để ứng dụng chạy mượt mà ở mức 60 FPS, không dùng chế độ debug vì sẽ bị giật lag).*

---

## Yêu Cầu Cấu Hình Cơ Bản
* **Hệ điều hành:** Windows 10/11, macOS 11 trở lên.
* **CPU:** Đa nhân cơ bản.
* **RAM:** Tối thiểu 4GB.
* **GPU:** Hỗ trợ wgpu (Vulkan/Metal/DX12) - tương thích với hầu hết card đồ họa hiện đại.
* **Thiết bị phụ trợ:** Khuyên dùng bảng vẽ điện tử (Wacom, Huion, XP-Pen) để có trải nghiệm cảm ứng lực nhấn tốt nhất.

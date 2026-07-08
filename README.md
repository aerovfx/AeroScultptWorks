# <img src="aero-sculpt/aero-sculpt-assets/logo.jpg" width="40" height="40" align="center"> AeroSculpt (ABrush)

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

[![Free during development](https://img.shields.io/badge/Price-Free_during_development-brightgreen.svg)](#-support-the-project--sponsorship)
[![Sponsor via PayPal](https://img.shields.io/badge/❤-Sponsor_$5_via_PayPal-ff69b4.svg)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5)

**Direct sponsor link / Link tài trợ trực tiếp:** [paypal.com/donate — Sponsor ABrush ($5)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5)

---

## English

AeroSculpt (codename ABrush) is a next-generation 3D sculpting application, written entirely in Rust. It is designed to deliver superior performance, smooth operation, and a minimalist interface to free your creativity from heavy, cumbersome tools.

This project is an effort to create an exclusive, cross-platform (Desktop App, Mobile App) sculpting tool that runs smoothly without requiring highly demanding system resources.

> **💡 Free while in development — powered by sponsors.**
> ABrush is **100% free to download and use** throughout its entire development period. There are no locked features, no trials, and no ads. Instead of charging users, the project is funded by voluntary sponsorships and donations from the community and from organizations that believe in accessible 3D tools. If ABrush saves you time or money, please consider [becoming a sponsor](#-support-the-project--sponsorship).

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

### ❤️ Support the Project — Sponsorship

**Our funding model is simple: the software stays free, and sponsors keep it alive.**

Professional 3D sculpting tools typically cost hundreds of dollars per license. ABrush gives everyone — students, hobbyists, indie studios — a professional-grade tool at zero cost during its entire development phase. In return, we rely on the generosity of users and organizations to fund the work.

**What your sponsorship funds:**
*   ⚙️ Full-time development of the core Rust engine and new features on the [roadmap](ROADMAP.md)
*   🖥️ Testing hardware and devices for cross-platform support (Desktop, Mobile, Web/WASM)
*   📦 Code signing certificates, build infrastructure, and distribution costs
*   📚 Documentation, tutorials, and community support

**How much? Just $5.** If you use ABrush, a one-time $5 sponsorship is all we ask. Larger or recurring contributions are welcome but never required.

| Tier | Suggested amount | Recognition |
|---|---|---|
| ☕ **Standard Sponsor** (recommended) | **$5 (one-time)** | Our sincere gratitude |
| 🚀 Project Backer | Custom amount | Name/logo in the SPONSORS section *(optional)* |
| 🏢 Corporate Sponsor | Contact us | Logo on README & website, direct feedback channel |

**Sponsor via PayPal** — click a button, or use the plain links below if the buttons don't load on your network:

[![Sponsor $5](https://img.shields.io/badge/PayPal-Sponsor_$5-00457C.svg?logo=paypal)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5)
[![Sponsor Custom Amount](https://img.shields.io/badge/PayPal-Custom_Amount-orange.svg?logo=paypal)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD)

*   Direct link ($5): `https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5`
*   Direct link (custom amount): `https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD`
*   Or send directly in the PayPal app to: **thegioithu2@gmail.com** (choose *"Sending to a friend"* → note: `ABrush`)

For corporate sponsorships, partnership inquiries, or invoiced contributions, contact us at **thegioithu2@gmail.com**.

*Every contribution — no matter the size — directly extends how long ABrush can remain free for everyone. Thank you!* 🙏

---

*Pick up your stylus and start sculpting amazing 3D artworks with AeroSculpt today!*

---

## Tiếng Việt

AeroSculpt (tên mã ABrush) là một ứng dụng điêu khắc 3D thế hệ mới, được viết hoàn toàn bằng ngôn ngữ Rust. Nó được thiết kế nhằm mang lại hiệu năng siêu việt, mượt mà và giao diện tối giản để giải phóng sự sáng tạo của bạn khỏi những công cụ nặng nề.

Dự án này là nỗ lực tạo ra một công cụ điêu khắc độc quyền, hoạt động trơn tru đa nền tảng (Desktop App, Mobile App) mà không đòi hỏi tài nguyên hệ thống quá khắt khe.

> **💡 Miễn phí trong suốt quá trình phát triển — được duy trì nhờ nhà tài trợ.**
> ABrush **hoàn toàn miễn phí để tải về và sử dụng** trong toàn bộ giai đoạn phát triển. Không khóa tính năng, không bản dùng thử, không quảng cáo. Thay vì thu phí người dùng, dự án được duy trì bằng các khoản tài trợ và đóng góp tự nguyện từ cộng đồng cũng như các tổ chức tin vào sứ mệnh phổ cập công cụ 3D. Nếu ABrush giúp bạn tiết kiệm thời gian hay chi phí, hãy cân nhắc [trở thành nhà tài trợ](#%EF%B8%8F-ủng-hộ-dự-án--tài-trợ).

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

### ❤️ Ủng Hộ Dự Án — Tài Trợ

**Mô hình tài chính của chúng tôi rất đơn giản: phần mềm luôn miễn phí, và các nhà tài trợ chính là người giữ cho dự án tồn tại.**

Các công cụ điêu khắc 3D chuyên nghiệp thường có giá hàng trăm đô la mỗi giấy phép. ABrush mang đến cho tất cả mọi người — học sinh sinh viên, người dùng cá nhân, studio indie — một công cụ chuyên nghiệp với chi phí bằng 0 trong suốt giai đoạn phát triển. Đổi lại, dự án hoạt động hoàn toàn dựa vào sự đóng góp hào phóng của người dùng và các tổ chức.

**Khoản tài trợ của bạn được dùng để:**
*   ⚙️ Phát triển toàn thời gian engine Rust lõi và các tính năng mới trong [lộ trình](ROADMAP.md)
*   🖥️ Mua thiết bị và phần cứng kiểm thử cho đa nền tảng (Desktop, Mobile, Web/WASM)
*   📦 Chứng chỉ ký ứng dụng (code signing), hạ tầng build và chi phí phân phối
*   📚 Tài liệu, video hướng dẫn và hỗ trợ cộng đồng

**Bao nhiêu? Chỉ cần $5.** Nếu bạn đang sử dụng ABrush, một khoản tài trợ $5 (một lần duy nhất) là tất cả những gì chúng tôi mong nhận. Các mức đóng góp lớn hơn luôn được hoan nghênh nhưng hoàn toàn không bắt buộc.

| Hạng | Mức gợi ý | Ghi nhận |
|---|---|---|
| ☕ **Nhà Tài Trợ Tiêu Chuẩn** (khuyến nghị) | **$5 (một lần)** | Lời cảm ơn chân thành từ đội ngũ |
| 🚀 Nhà Bảo Trợ | Mức tùy chọn | Tên/logo trong mục SPONSORS *(tùy chọn)* |
| 🏢 Doanh Nghiệp Tài Trợ | Liên hệ | Logo trên README & website, kênh phản hồi trực tiếp |

**Tài trợ qua PayPal** — bấm nút bên dưới, hoặc dùng link chữ dự phòng nếu nút không hiển thị trên mạng của bạn:

[![Tài Trợ $5](https://img.shields.io/badge/PayPal-T%C3%A0i_Tr%E1%BB%A3_$5-00457C.svg?logo=paypal)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5)
[![Tài Trợ Tùy Chọn](https://img.shields.io/badge/PayPal-M%E1%BB%A9c_T%C3%B9y_Ch%E1%BB%8Dn-orange.svg?logo=paypal)](https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD)

*   Link trực tiếp ($5): `https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD&amount=5`
*   Link trực tiếp (mức tùy chọn): `https://www.paypal.com/donate/?business=thegioithu2%40gmail.com&item_name=Sponsor+ABrush+Development&currency_code=USD`
*   Hoặc gửi trực tiếp trong ứng dụng PayPal đến: **thegioithu2@gmail.com** (chọn *"Gửi cho bạn bè"* → ghi chú: `ABrush`)

Đối với tài trợ doanh nghiệp, hợp tác thương hiệu, hoặc đóng góp cần hóa đơn/chứng từ, vui lòng liên hệ: **thegioithu2@gmail.com**.

*Mỗi khoản đóng góp — dù lớn hay nhỏ — đều trực tiếp kéo dài thời gian ABrush được miễn phí cho tất cả mọi người. Xin chân thành cảm ơn!* 🙏

---

*Hãy cầm bút cảm ứng lên và bắt đầu nặn ra những tác phẩm nghệ thuật 3D tuyệt vời cùng AeroSculpt!*

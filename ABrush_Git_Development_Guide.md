# Hướng dẫn Git Development & Release cho ABrush / AeroSculpt

## Mục tiêu

Thiết lập quy trình phát triển và phát hành ứng dụng chuyên nghiệp sử
dụng GitHub.

------------------------------------------------------------------------

# Cấu trúc Branch

  Branch        Mục đích
  ------------- ----------------------------
  `main`        Stable Release
  `develop`     Tích hợp tính năng
  `feature/*`   Phát triển tính năng mới
  `bugfix/*`    Sửa lỗi
  `hotfix/*`    Sửa lỗi khẩn cấp từ `main`
  `release/*`   Chuẩn bị phát hành

------------------------------------------------------------------------

# Quy trình phát triển

``` text
feature/*
    │
    ▼
develop
    │
    ▼
release/*
    │
    ▼
main
```

Không commit trực tiếp lên `main`.

------------------------------------------------------------------------

# Semantic Versioning

``` text
MAJOR.MINOR.PATCH

0.1.0
0.2.0
0.2.1
1.0.0
```

-   MAJOR: thay đổi lớn, không tương thích.
-   MINOR: thêm tính năng.
-   PATCH: sửa lỗi.

------------------------------------------------------------------------

# Cấu trúc Release

``` text
Releases/

v0.1.0

Assets
├── AeroSculpt-macOS-arm64.dmg
├── AeroSculpt-macOS-x64.dmg
├── AeroSculpt-Windows-x64.zip
├── AeroSculpt-Linux.AppImage
└── SHA256SUMS
```

------------------------------------------------------------------------

# File VERSION

``` text
0.1.0
```

Được dùng để đồng bộ phiên bản trong quá trình build.

------------------------------------------------------------------------

# CHANGELOG.md

``` markdown
## v0.1.0

### New
- Brush Engine
- Undo
- OBJ Import

### Improved
- GPU Rendering

### Fixed
- Crash when loading OBJ
```

------------------------------------------------------------------------

# GitHub Actions

Pipeline đề xuất:

``` text
Push Tag
    │
    ▼
Build macOS
Build Windows
Build Linux
    │
    ▼
Package
    │
    ▼
Create GitHub Release
    │
    ▼
Upload Assets
```

------------------------------------------------------------------------

# Thư mục dist

``` text
dist/
├── macos/
├── windows/
└── linux/
```

------------------------------------------------------------------------

# Quy tắc Tag

``` text
git tag v0.1.0
git push origin v0.1.0
```

Mỗi tag sẽ kích hoạt pipeline phát hành.

------------------------------------------------------------------------

# Nightly Build

-   `main` → Stable
-   `develop` → Beta
-   Nightly → Build từ commit mới nhất

------------------------------------------------------------------------

# Bảo mật

-   Ký mã (Code Signing) cho macOS và Windows.
-   Sinh SHA256 cho mọi gói cài đặt.
-   Không commit secrets vào repository.

------------------------------------------------------------------------

# Checklist trước khi Release

-   [ ] Tăng phiên bản trong `VERSION`
-   [ ] Cập nhật `CHANGELOG.md`
-   [ ] Build thành công trên macOS
-   [ ] Build thành công trên Windows
-   [ ] Build thành công trên Linux
-   [ ] Kiểm tra checksum
-   [ ] Tạo Git Tag
-   [ ] Tạo GitHub Release
-   [ ] Kiểm tra tải và cài đặt trên các nền tảng

------------------------------------------------------------------------

# Mục tiêu

Thiết lập quy trình CI/CD để mỗi Git Tag tự động:

1.  Build ứng dụng.
2.  Đóng gói.
3.  Tạo GitHub Release.
4.  Upload bộ cài cho macOS, Windows và Linux.
5.  Phát hành sẵn sàng cho người dùng tải xuống.

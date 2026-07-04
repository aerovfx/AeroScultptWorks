# 🎨 Hướng Dẫn Sử Dụng AeroSculpt (ABrush)

AeroSculpt được thiết kế để mang lại trải nghiệm điêu khắc 3D mạnh mẽ nhưng vô cùng trực quan. Lấy cảm hứng từ ZBrush, giao diện của ứng dụng được tối ưu hóa cho cả người dùng chuột và bút cảm ứng (tablet/stylus).

---

## 1. Các Tính Năng Cốt Lõi

### DynaMesh (Voxel Remesh) - Tính toán lại lưới
DynaMesh giúp bạn thoải mái kéo giãn hình khối mà không lo lưới bị biến dạng hay méo mó.
* **Cách dùng:** Nhấn giữ `Ctrl` và kéo chuột một đoạn trên vùng nền trống (canvas).
* **Kết quả:** Lưới của vật thể sẽ tự động được tái cấu trúc thành các đa giác đều đặn.

### Sculptris Pro - Điêu khắc thông minh
Cho phép bạn điêu khắc đến đâu, ứng dụng sẽ tự động chia nhỏ lưới (tăng chi tiết) đến đó, giải phóng bạn khỏi các rào cản về topology.
* Tự động điều chỉnh mức độ chi tiết bề mặt tại vị trí cọ vẽ.

### Polygroup - Quản lý lưới theo nhóm
Giúp phân vùng các phần khác nhau của vật thể bằng các màu sắc riêng biệt.
* **Tạo nhóm mới:** Dùng công cụ mặt nạ (Mask) để chọn một vùng, sau đó nhấn `Ctrl + W`. Vùng đó sẽ tự động chuyển thành một Polygroup mới với màu ngẫu nhiên.
* **Hiển thị Polyframe:** Nhấn `Shift + F` để bật hiển thị khung lưới và các màu nhóm.

---

## 2. Hệ Thống Cọ Vẽ (Brushes)

AeroSculpt cung cấp hơn 20 loại cọ khác nhau để phục vụ mọi nhu cầu điêu khắc. Để đổi cọ nhanh, hãy nhấn **`Space`** hoặc **`Tab`** để mở **Pie Menu** ngay tại vị trí con trỏ chuột.

Một số nhóm cọ phổ biến:
* **Sculpt (Điêu khắc cơ bản):** `Standard`, `Clay`, `ClayBuildup`, `DamStandard` (chuyên tạo rãnh sâu), `HPolish` (làm phẳng bề mặt).
* **Smooth (Làm mịn):** `Smooth` (bật nhanh bằng cách giữ `Shift`), `Flatten`.
* **Deform (Biến dạng):** `Inflate` (thổi phồng), `Pinch` (kéo vertex lại gần nhau để tạo nếp nhăn).
* **Move (Di chuyển):** `Move`, `SnakeHook` (kéo dài phần lưới cực kỳ linh hoạt).

---

## 3. Quản Lý Mặt Nạ (Masking)

Mặt nạ bảo vệ các phần của vật thể để không bị tác động bởi cọ vẽ. Vùng được mask sẽ có màu tối hơn.
* **Vẽ mặt nạ:** Giữ `Ctrl` và vẽ trực tiếp lên vật thể.
* **Xóa mặt nạ:** Giữ `Ctrl + Alt` và vẽ lên vùng đã mask.
* **Đảo ngược mặt nạ:** Nhấp chuột (Click) vào vùng nền trống trong khi giữ `Ctrl`.
* **Xóa toàn bộ mặt nạ:** Kéo chuột trên vùng nền trống trong khi giữ `Ctrl`.

---

## 4. Công Cụ Gizmo 3D (Biến Hình)

Dùng để di chuyển, xoay hoặc thay đổi kích thước toàn bộ vật thể:
* **Di chuyển (Translate):** Bấm phím `G`.
* **Phóng to/Thu nhỏ (Scale):** Bấm phím `R`.
* **Xoay (Rotate):** Bấm phím `E`.

---

## 5. Chất Liệu (MatCap) & Tùy Chọn Khác

* **Đổi chất liệu:** AeroSculpt đi kèm với 21 chất liệu hiển thị siêu đẹp (Clay, Skin, Metal, Chrome...). Bạn có thể chọn chúng từ bảng Material ở bên phải màn hình.
* **Chế độ đối xứng (Symmetry):** Nhấn phím `X` để bật/tắt đối xứng theo trục X, giúp bạn nặn các vật thể cần độ cân bằng hoàn hảo như khuôn mặt, cơ thể.
* **Undo/Redo:** Nếu bạn lỡ làm hỏng, đừng lo! Bấm `Ctrl + Z` để Undo và `Ctrl + Y` để Redo. AeroSculpt lưu lại tới 30 thao tác lịch sử.
* **Import/Export:** Ứng dụng hỗ trợ xuất và nhập mô hình ở định dạng **.obj** (bao gồm cả vertex colors).

Chúc bạn có những tác phẩm điêu khắc tuyệt vời cùng AeroSculpt!

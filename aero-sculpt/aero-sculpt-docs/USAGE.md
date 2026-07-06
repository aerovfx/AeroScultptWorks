# 🎨 Usage Guide / Hướng Dẫn Sử Dụng ABrush

*Read this in: [English](#english) | [Tiếng Việt](#tiếng-việt)*

---

## English

ABrush is designed to provide a powerful yet highly intuitive 3D sculpting experience. The application interface is optimized for both mouse users and graphics tablet (stylus) users.

### 1. Core Features

#### DynaMesh (Voxel Remesh) - Mesh Recomputation
DynaMesh allows you to freely stretch and deform shapes without worrying about the mesh becoming distorted.
* **How to use:** Hold `Ctrl` and drag the mouse a short distance on an empty area of the canvas.
* **Result:** The object's mesh will be automatically reconstructed into even, regular polygons.

#### Sculptris Pro - Smart Sculpting
Allows you to sculpt anywhere, and the application will automatically subdivide the mesh (increase detail) exactly where you are painting, freeing you from topology constraints.
* Automatically adjusts surface detail based on brush location and size.

#### Polygroup - Manage Mesh by Groups
Helps segment different parts of an object using distinct colors.
* **Create a new group:** Use the Mask tool to select an area, then press `Ctrl + W`. That area will automatically become a new Polygroup with a random color.
* **Show Polyframe:** Press `Shift + F` to toggle the wireframe and group colors.

### 2. Brush System

ABrush provides over 20 different brush types to serve all your sculpting needs. To change brushes quickly, press **`Space`** or **`Tab`** to open the **Pie Menu** right at your cursor's location.

Common brush categories:
* **Sculpt (Basic Sculpting):** `Standard`, `Clay`, `ClayBuildup`, `DamStandard` (for deep creases), `HPolish` (for flattening surfaces).
* **Smooth:** `Smooth` (quick toggle by holding `Shift`), `Flatten`.
* **Deform:** `Inflate`, `Pinch` (pulls vertices together to create sharp folds).
* **Move:** `Move`, `SnakeHook` (pulls and extends the mesh extremely flexibly).

### 3. Masking Management

Masks protect parts of the object from being affected by brushes. Masked areas will appear darker.
* **Draw mask:** Hold `Ctrl` and paint directly on the object.
* **Erase mask:** Hold `Ctrl + Alt` and paint over the masked area.
* **Invert mask:** Click on an empty canvas area while holding `Ctrl`.
* **Clear mask:** Drag the mouse on an empty canvas area while holding `Ctrl`.

### 4. 3D Gizmo Tool (Transform)

Used to move, rotate, or scale the entire object:
* **Move (Translate):** Press `G`.
* **Scale:** Press `R`.
* **Rotate:** Press `E`.

### 5. Materials (MatCap) & Other Options

* **Change Material:** ABrush comes with 21 beautiful display materials (Clay, Skin, Metal, Chrome...). You can select them from the Material panel on the right.
* **Symmetry Mode:** Press `X` to toggle X-axis symmetry, which helps when sculpting perfectly balanced objects like faces or bodies.
* **Undo/Redo:** If you make a mistake, don't worry! Press `Ctrl + Z` to Undo and `Ctrl + Y` to Redo. ABrush stores up to 30 history states.
* **Import/Export:** The app supports importing and exporting models in **.obj** format (including vertex colors).

Happy sculpting with ABrush!

---

## Tiếng Việt

ABrush được thiết kế để mang lại trải nghiệm điêu khắc 3D mạnh mẽ nhưng vô cùng trực quan. Giao diện của ứng dụng được tối ưu hóa cho cả người dùng chuột và bút cảm ứng (tablet/stylus).

### 1. Các Tính Năng Cốt Lõi

#### DynaMesh (Voxel Remesh) - Tính toán lại lưới
DynaMesh giúp bạn thoải mái kéo giãn hình khối mà không lo lưới bị biến dạng hay méo mó.
* **Cách dùng:** Nhấn giữ `Ctrl` và kéo chuột một đoạn trên vùng nền trống (canvas).
* **Kết quả:** Lưới của vật thể sẽ tự động được tái cấu trúc thành các đa giác đều đặn.

#### Sculptris Pro - Điêu khắc thông minh
Cho phép bạn điêu khắc đến đâu, ứng dụng sẽ tự động chia nhỏ lưới (tăng chi tiết) đến đó, giải phóng bạn khỏi các rào cản về topology.
* Tự động điều chỉnh mức độ chi tiết bề mặt tại vị trí cọ vẽ.

#### Polygroup - Quản lý lưới theo nhóm
Giúp phân vùng các phần khác nhau của vật thể bằng các màu sắc riêng biệt.
* **Tạo nhóm mới:** Dùng công cụ mặt nạ (Mask) để chọn một vùng, sau đó nhấn `Ctrl + W`. Vùng đó sẽ tự động chuyển thành một Polygroup mới với màu ngẫu nhiên.
* **Hiển thị Polyframe:** Nhấn `Shift + F` để bật hiển thị khung lưới và các màu nhóm.

### 2. Hệ Thống Cọ Vẽ (Brushes)

ABrush cung cấp hơn 20 loại cọ khác nhau để phục vụ mọi nhu cầu điêu khắc. Để đổi cọ nhanh, hãy nhấn **`Space`** hoặc **`Tab`** để mở **Pie Menu** ngay tại vị trí con trỏ chuột.

Một số nhóm cọ phổ biến:
* **Sculpt (Điêu khắc cơ bản):** `Standard`, `Clay`, `ClayBuildup`, `DamStandard` (chuyên tạo rãnh sâu), `HPolish` (làm phẳng bề mặt).
* **Smooth (Làm mịn):** `Smooth` (bật nhanh bằng cách giữ `Shift`), `Flatten`.
* **Deform (Biến dạng):** `Inflate` (thổi phồng), `Pinch` (kéo vertex lại gần nhau để tạo nếp nhăn).
* **Move (Di chuyển):** `Move`, `SnakeHook` (kéo dài phần lưới cực kỳ linh hoạt).

### 3. Quản Lý Mặt Nạ (Masking)

Mặt nạ bảo vệ các phần của vật thể để không bị tác động bởi cọ vẽ. Vùng được mask sẽ có màu tối hơn.
* **Vẽ mặt nạ:** Giữ `Ctrl` và vẽ trực tiếp lên vật thể.
* **Xóa mặt nạ:** Giữ `Ctrl + Alt` và vẽ lên vùng đã mask.
* **Đảo ngược mặt nạ:** Nhấp chuột (Click) vào vùng nền trống trong khi giữ `Ctrl`.
* **Xóa toàn bộ mặt nạ:** Kéo chuột trên vùng nền trống trong khi giữ `Ctrl`.

### 4. Công Cụ Gizmo 3D (Biến Hình)

Dùng để di chuyển, xoay hoặc thay đổi kích thước toàn bộ vật thể:
* **Di chuyển (Translate):** Bấm phím `G`.
* **Phóng to/Thu nhỏ (Scale):** Bấm phím `R`.
* **Xoay (Rotate):** Bấm phím `E`.

### 5. Chất Liệu (MatCap) & Tùy Chọn Khác

* **Đổi chất liệu:** ABrush đi kèm với 21 chất liệu hiển thị siêu đẹp (Clay, Skin, Metal, Chrome...). Bạn có thể chọn chúng từ bảng Material ở bên phải màn hình.
* **Chế độ đối xứng (Symmetry):** Nhấn phím `X` để bật/tắt đối xứng theo trục X, giúp bạn nặn các vật thể cần độ cân bằng hoàn hảo như khuôn mặt, cơ thể.
* **Undo/Redo:** Nếu bạn lỡ làm hỏng, đừng lo! Bấm `Ctrl + Z` để Undo và `Ctrl + Y` để Redo. ABrush lưu lại tới 30 thao tác lịch sử.
* **Import/Export:** Ứng dụng hỗ trợ xuất và nhập mô hình ở định dạng **.obj** (bao gồm cả vertex colors).

Chúc bạn có những tác phẩm điêu khắc tuyệt vời cùng ABrush!

# CompactStatusBar ⚡

[![Build CompactStatusBar Tweak DEB](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_deb.yml/badge.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_deb.yml)
[![Build CompactStatusBar IPA](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_ipa.yml/badge.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_ipa.yml)
[![Platform](https://img.shields.io/badge/Platform-iOS%2015.0%2B-blue.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar)
[![Jailbreak](https://img.shields.io/badge/Jailbreak-Rootless%20%7C%20Rootful%20%7C%20TrollStore-success.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar)
[![License](https://img.shields.io/badge/License-MIT-orange.svg)](LICENSE)

**CompactStatusBar** là tweak thanh trạng thái (Status Bar) tối giản, hiện đại và tinh tế dành cho iOS. Dự án tích hợp **Pin (Battery)**, **Sóng di động (Cellular)** và **Wi-Fi / Mạng (Network)** vào một biểu tượng đo tròn 3-trong-1 (Circular 3-in-1 Gauge) duy nhất, loại bỏ hoàn toàn sự rườm rà trên thanh trạng thái truyền thống của Apple.

Được phát triển dựa trên ngôn ngữ thiết kế tối giản DuoBar kết hợp chuẩn giao diện Apple Human Interface Guidelines, CompactStatusBar mang lại vẻ đẹp thanh lịch, sắc nét và khả năng tùy biến cao trên cả máy Jailbreak (Rootless/Rootful) lẫn cài đặt qua TrollStore.

---

## 🌟 Điểm nổi bật (Features)

```
       [ 100 ]            <- Đỉnh vương miện (Top Crown) hiển thị % Pin
    ╭───────────╮         
   │     ╭─╮     │        <- Vòng cung Pin (Màu xanh Apple System Green #34C759)
   │    ( • )    │        <- Tâm Gauge: Quạt Wi-Fi 2 tầng sóng / Logo 5G/4G / Sét sạc
   │     ╰─╯     │        
    ╰──●─●─●─●──╯         <- 4 chấm sóng di động uốn cong đáy vòng tròn
```

### 1. Vòng đo Pin chuẩn hình học (Seamless Geometric Arc)
* **Khớp nối hình học 100%:** Vòng cung đo bắt đầu từ góc 140° kéo dài 260° qua đỉnh đến 400° (40°). Khe hở 100° dưới đáy tiếp giáp hoàn hảo với các chấm sóng di động, loại bỏ hoàn toàn hiện tượng đứt gãy hoặc lệch bán kính.
* **Màu sắc động Apple (Dynamic Battery Colors):**
  * 🔋 **Bình thường (> 20%):** Màu xanh Apple System Green (`#34C759`).
  * ⚡ **Đang sạc:** Sáng xanh rực rỡ kèm hiệu ứng nhịp thở phát sáng (Breathing Glow) tùy chọn.
  * 🟡 **Chế độ nguồn điện thấp (LPM):** Màu vàng đặc trưng Apple (`#FFCC00`).
  * 🔴 **Pin yếu (≤ 20%):** Tự động chuyển màu đỏ cảnh báo (`#FF3B30`).
* **Đa chế độ hiển thị phần trăm pin (`p_batteryPercentMode`):**
  * **Đỉnh vòm (Top Crown - Mặc định):** Số % lồng khéo léo vào khe đỉnh 12 giờ của vòng tròn, giữ nguyên tỷ lệ 1:1 siêu gọn.
  * **Ở tâm (Center):** Số % nằm ngay chính giữa gauge.
  * **Kế bên (Beside):** Hiển thị dạng viên thuốc Capsule kèm tốc độ mạng và tên Wi-Fi.
  * **Mép trái (Left Side):** Số % nằm gọn gàng bên trái gauge.
  * **Ẩn (Minimalist):** Chỉ hiển thị vòng đo và chấm sóng, ẩn số %.

### 2. Chấm sóng di động uốn cong đáy (Cradled Cellular Dots)
* **Bán kính đồng tâm tuyệt đối:** 4 chấm tròn (hoặc 5 chấm tùy chọn) được phân bố đều đặn với bước nhảy 20° trên đúng bán kính 9.0pt của gauge.
* **Tự động nhận diện mức sóng:** Số chấm sáng tương ứng với độ mạnh yếu của sóng mạng (0 đến 4 vạch).
* **Độ tương phản cao:** Các chấm chưa sáng (unlit) luôn giữ độ mờ 25-28% rõ nét trên cả hình nền sáng lẫn hình nền tối, không bao giờ bị biến mất.

### 3. Tâm Gauge đa năng (Dynamic Center Slot)
* **Wi-Fi đa mức:** Khi kết nối Wi-Fi, hiển thị quạt Wi-Fi vector gồm điểm phát sóng và 2 tầng sóng uốn lượn.
* **Mạng di động (5G / 4G / LTE):** Khi tắt Wi-Fi hoặc dùng dữ liệu di động, tâm gauge tự động hiển thị thế hệ mạng (`5G`, `4G`, `LTE`, `3G`) với phông chữ đậm sắc sảo, không để lại hốc rỗng.
* **Chế độ máy bay (Airplane) & Không có SIM (No SIM):** Hiển thị silhouette máy bay hoặc thẻ SIM gạch chéo tinh gọn.
* **Tia sét sạc (Charging Bolt):** Hiển thị biểu tượng tia sét ngay tại tâm khi cắm sạc.

### 4. Đồng bộ hóa Control Center & Màn hình khóa
* **Đồng bộ Control Center (`ccSyncWithStatusBar`):** Tự động căn chỉnh vị trí icon pin trong Trung tâm điều khiển khớp chuẩn theo thanh trạng thái chính, giải quyết triệt để lỗi nhảy lệch hoặc khó căn chỉnh.
* **Lọc chống giật (Jitter Filter):** Cố định tọa độ neo vững chắc, không bị rung lắc khi mở ứng dụng hay vuốt chuyển trang.

### 5. Cử chỉ tương tác thông minh (Smart Gestures)
* **Chạm 1 lần (Single Tap):** Chuyển đổi tức thì giữa hiển thị % Pin và % RAM hệ thống.
* **Chạm 2 lần (Double Tap):** Mở thẻ thông số HUD chi tiết (Dung lượng pin, IP, SSID, RAM thực tế, CPU, Tốc độ mạng).
* **Nhấn giữ (Long Press):** Bật/tắt chế độ **Kéo thả tự do (Drag & Drop Mode)** để di chuyển vị trí gauge trực tiếp trên màn hình với phản hồi rung Haptic.
* **Vuốt trái / phải (Swipe):** Thao tác nhanh tùy biến.

---

## 📁 Cấu trúc dự án (Repository Structure)

```
CompactStatusBar/
├── .github/
│   └── workflows/
│       ├── build_deb.yml             # Tự động build gói .deb (Rootless) qua GitHub Actions
│       └── build_ipa.yml             # Tự động build file .ipa (TrollStore) qua GitHub Actions
├── Tweak/                            # Mã nguồn Tweak Jailbreak (C / Objective-C)
│   ├── Preferences/                  # Giao diện Cài đặt (Settings Specifiers)
│   │   ├── CompactStatusBar.plist    # Bảng thiết lập toàn diện
│   │   └── Root.plist
│   ├── CompactStatusBarTweak.plist   # Filter SpringBoard / MobileSubstrate
│   ├── Makefile                      # Theos build file
│   ├── Tweak.m                       # Core hook, vector render & gestures
│   ├── Tweak.x                       # Logos hook file
│   ├── build_deb.sh                  # Script đóng gói DEB tự động
│   └── control                       # Debian package metadata
├── App/                              # Mã nguồn Ứng dụng độc lập (SwiftUI / TrollStore)
│   ├── App/
│   │   └── CompactStatusBarApp.swift
│   ├── Managers/
│   │   ├── StatusBarOverlayManager.swift
│   │   └── SystemStatusManager.swift
│   ├── Views/
│   │   ├── CombinedStatusGaugeView.swift
│   │   ├── SettingsView.swift
│   │   └── StatusHUDPopupView.swift
│   ├── Entitlements.plist
│   ├── Info.plist
│   └── build_ipa.sh
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🚀 Cài đặt (Installation)

### Cách 1: Cài đặt bản Tweak (.deb) - Dành cho máy Jailbreak
1. Tải file `CompactStatusBar_rootless.deb` từ mục [Releases](https://github.com/Hoangnguyennaaa/CompactStatusBar/releases) hoặc tab **Actions** (Artifacts).
2. Mở file bằng trình quản lý gói của bạn:
   * **Sileo**
   * **Zebra**
   * Hoặc cài qua terminal:
     ```bash
     dpkg -i CompactStatusBar_rootless.deb
     ```
3. Khởi động lại SpringBoard (Respring) để kích hoạt tweak.

> **Tương thích:** Dopamine, Palera1n, Bootstrap/Serotonin, XinaA15, unc0ver (iOS 15.0 - 18.x).

### Cách 2: Cài đặt bản App (.ipa) - Dành cho TrollStore / Sideload
1. Tải file `CompactStatusBar.ipa` từ mục [Releases](https://github.com/Hoangnguyennaaa/CompactStatusBar/releases).
2. Mở bằng **TrollStore** và nhấn **Install**.
3. Cấp quyền cần thiết và bật Overlay để tận hưởng icon pin nổi chuẩn xác.

---

## 🛠 Hướng dẫn Build từ nguồn (Build from Source)

### 1. Build Tweak (.deb) trên macOS / Linux (với Xcode & Theos hoặc Clang)
```bash
cd Tweak
chmod +x build_deb.sh
./build_deb.sh
```
File `CompactStatusBar_rootless.deb` sẽ được tạo ngay trong thư mục.

### 2. Build App (.ipa)
```bash
cd App
chmod +x build_ipa.sh
./build_ipa.sh
```
File `CompactStatusBar.ipa` hoàn chỉnh sẵn sàng cài đặt qua TrollStore.

### 3. Tự động qua GitHub Actions
Chỉ cần Fork hoặc Push lên branch `main`, hệ thống GitHub Actions trên máy chủ macOS ảo sẽ tự động biên dịch, ký số và xuất xưởng file `.deb` và `.ipa` trong mục **Artifacts** chỉ sau chưa đầy 1 phút.

---

## ⚙️ Tùy biến trong Cài đặt (Settings)

Mở **Cài đặt (Settings) -> CompactStatusBar**:
* **Kích hoạt Tweak:** Bật/Tắt tức thời không cần respring.
* **Vị trí & Kiểu % Pin:** Đỉnh vòm (Top Crown), Ở tâm, Kế bên, Mép trái, hoặc Ẩn.
* **Giao diện & Màu sắc:**
  * Dynamic / Adaptive (Tự thích ứng theo màu nền hệ thống).
  * Đơn sắc trắng (Clean White).
  * Neon Cyan, Neon Tím, Neon Hồng, Neon Xanh lá, Neon Cam, Vàng Gold, Đỏ Ruby.
  * Tùy chọn RGB thủ công.
* **Kích thước & Độ trong suốt:** Thanh trượt điều chỉnh kích thước icon pin (từ 0.5x đến 2.5x).
* **Đồng bộ Control Center:** Tự động đồng bộ vị trí và tỷ lệ cho Trung tâm điều khiển.
* **Chế độ Kéo thả (Drag Mode):** Cho phép chạm kéo icon đến bất kỳ góc nào trên màn hình.

---

## 📄 Bản quyền (License)

Dự án được phân phối theo giấy phép mã nguồn mở **MIT License**. Bạn hoàn toàn có thể tự do chỉnh sửa, phát triển thêm và chia sẻ.

* **Tác giả:** Hoangnguyen ([@Hoangnguyennaaa](https://github.com/Hoangnguyennaaa))
* **Ý tưởng thiết kế:** DuoBar / Android Duo StatusBar Concept.

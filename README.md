# CompactStatusBar ⚡

[![Release](https://img.shields.io/github/v/release/Hoangnguyennaaa/CompactStatusBar?color=brightgreen&label=Phiên%20bản)](https://github.com/Hoangnguyennaaa/CompactStatusBar/releases)
[![Build DEB](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_deb.yml/badge.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar/actions/workflows/build_deb.yml)
[![Platform](https://img.shields.io/badge/Platform-iOS%2015.0%20--%2018.x-blue.svg)](https://github.com/Hoangnguyennaaa/CompactStatusBar)
[![License](https://img.shields.io/badge/License-MIT-orange.svg)](LICENSE)

**CompactStatusBar** là tweak tinh chỉnh thanh trạng thái (Status Bar) dành cho iPhone/iPad đã Jailbreak. Tweak gom gọn **Pin**, **Sóng di động** và **Wi-Fi / 4G / 5G** vào một biểu tượng tròn 3-trong-1 duy nhất, giúp màn hình gọn gàng, tinh tế và hiện đại hơn.

---

## 📥 Tải về (Download)

👉 [**Tải CompactStatusBar (.deb) mới nhất tại đây**](https://github.com/Hoangnguyennaaa/CompactStatusBar/releases)

* **Phiên bản:** `v1.4.8 (Rootless arm64)`
* **Hỗ trợ cài qua:** Sileo, Zebra hoặc Filza.

---

## 📸 Hình ảnh thực tế

<p align="center">
  <img src="assets/demo1.png" alt="Demo màn hình chính" width="280"/>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="assets/demo2.png" alt="Demo Control Center" width="280"/>
</p>

---

## ✨ Tính năng chính

- 🔋 **Vòng tròn Pin 3-trong-1:** Hiển thị mức pin dạng vòng cung mượt mà, tự động đổi màu:
  - 🟢 **Xanh:** Pin bình thường (> 20%)
  - ⚡ **Tia sét & hiệu ứng nhịp thở:** Đang cắm sạc
  - 🟡 **Vàng:** Bật chế độ Tiết kiệm pin (Low Power Mode)
  - 🔴 **Đỏ:** Pin yếu (≤ 20%)
- 📶 **Chấm sóng di động:** 4 chấm tròn uốn cong theo đáy vòng tròn, nhận diện trực quan độ mạnh sóng.
- 🌐 **Tâm icon thông minh:** Tự động đổi linh hoạt giữa cột sóng Wi-Fi hoặc logo mạng di động (`5G`, `4G`, `LTE`).
- 🎛️ **Đồng bộ Control Center:** Căn chỉnh vị trí icon trong Trung tâm điều khiển khớp hoàn toàn với thanh trạng thái, không bị lệch.
- ✋ **Kéo thả tự do:** Dễ dàng di chuyển vị trí icon đến bất kỳ góc nào bạn muốn.

---

## 👆 Thao tác cử chỉ

| Cử chỉ | Tác dụng |
| :--- | :--- |
| **Chạm 1 lần** | Đổi nhanh giữa hiển thị **% Pin** và **% RAM** |
| **Chạm 2 lần** | Mở bảng thông số chi tiết (RAM, CPU, IP mạng, Tốc độ tải) |
| **Nhấn giữ (0.5s)** | Bật/tắt chế độ **Kéo thả** để di chuyển icon tự do |

---

## 📲 Hướng dẫn cài đặt

1. Tải file `CompactStatusBar_rootless.deb` từ mục [Releases](https://github.com/Hoangnguyennaaa/CompactStatusBar/releases).
2. Mở file bằng **Sileo** (hoặc Zebra / Filza) và bấm **Cài đặt (Get / Install)**.
3. **Respring** lại máy để kích hoạt tweak.
4. Mở **Cài đặt (Settings)** -> chọn **CompactStatusBar** để bật và tùy chỉnh các chế độ.

---

## 📱 Thiết bị hỗ trợ

| Dòng máy | iOS | Công cụ Jailbreak | Trạng thái |
| :--- | :--- | :--- | :--- |
| **iPhone 7 Plus, 8, X** | iOS 15.0 – 16.7.x | Palera1n (Rootless) | Hoạt động tốt |
| **iPhone XS đến 14 Series** | iOS 15.0 – 16.5.1 | Dopamine 2.x | Hoạt động tốt |
| **Thiết bị chạy Serotonin** | iOS 16.0 – 16.6.1 | Bootstrap + Serotonin | Hoạt động tốt |

---

## ⚠️ Lưu ý & Miễn trừ trách nhiệm

* Tweak là phần mềm mã nguồn mở được phát triển phi lợi nhuận.
* Việc can thiệp hệ thống qua Jailbreak luôn có rủi ro nhất định. Tác giả không chịu trách nhiệm nếu xảy ra sự cố phần mềm, xung đột với tweak khác hoặc mất dữ liệu trên thiết bị của bạn.
* Bạn nên sao lưu (backup) dữ liệu trước khi cài đặt.

---

## ☕ Ủng hộ tác giả (Donate)

Nếu bạn thấy tweak hữu ích, bạn có thể ủng hộ tác giả một ly cà phê qua mã QR dưới đây:

<p align="center">
  <img src="assets/donate_qr.png" alt="Mã QR Ủng hộ" width="220"/>
  <br>
  <em>Cảm ơn sự ủng hộ của bạn! ❤️</em>
</p>

---

<details>
<summary>🛠 Dành cho lập trình viên (Build từ mã nguồn)</summary>

```bash
git clone https://github.com/Hoangnguyennaaa/CompactStatusBar.git
cd CompactStatusBar/Tweak
chmod +x build_deb.sh
./build_deb.sh
```
</details>

## 📄 License

Dự án phát hành theo giấy phép [MIT License](LICENSE).

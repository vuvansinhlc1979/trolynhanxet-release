# 🎓 TRỢ LÝ NHẬN XÉT VNEDU v2.0
**Tác giả: Vũ Văn Sinh · Trường TH số 2 Gia Phú · Zalo: 0386643722**

---

## 📦 DANH SÁCH FILE TRONG GÓI

```
TroLyNhanXet/
├── manifest.json       ← Cấu hình extension
├── popup.html          ← Giao diện popup chính
├── popup.js            ← Logic popup (key, grade, preview)
├── content.js          ← Script chạy trên VnEdu (chứa ngân hàng nhận xét)
├── settings.html       ← Trang quản lý nhận xét tùy chỉnh
├── icons/
│   ├── icon16.png      ← Copy icon.png vào đây, đổi tên
│   ├── icon48.png
│   └── icon128.png
└── README.md           ← File này
```

## ⚙️ CÁCH CÀI ĐẶT

1. **Chuẩn bị icon**: Copy file `icon.png` (logo của Thầy) vào thư mục `icons/`, tạo 3 bản với tên `icon16.png`, `icon48.png`, `icon128.png`.
   
2. **Mở Chrome** → Vào `chrome://extensions/`

3. **Bật chế độ Developer**: Bật công tắc **"Developer mode"** ở góc phải trên

4. **Cài extension**: Nhấn **"Load unpacked"** → Chọn toàn bộ thư mục `TroLyNhanXet`

5. **Kích hoạt**: Nhấn biểu tượng extension → Nhập mã kích hoạt

---

## 🔑 MÃ KÍCH HOẠT

| Mã | Dành cho |
|---|---|
| `VVS-2024-SINH` | Vũ Văn Sinh (Admin) |
| `VVS-2024-A001` | Giáo viên 1 |
| `VVS-2024-A002` | Giáo viên 2 |
| `VVS-2024-A003` | Giáo viên 3 |
| `VVS-2024-DEMO` | Dùng thử |

> **Để thêm key mới**: Mở file `popup.js`, tìm `const VALID_KEYS` và thêm dòng mới theo mẫu.

---

## 🚀 CÁCH SỬ DỤNG

1. Đăng nhập VnEdu → Vào trang nhập điểm học kỳ
2. Nhập điểm số (ví dụ: 9, 7, 4) hoặc xếp loại (T, H, C) vào các ô
3. Nhấn biểu tượng extension ở thanh Chrome
4. Chọn **Khối lớp** và **Môn học**
5. Nhấn **👁️ Xem trước** nếu muốn xem mẫu câu
6. Nhấn **🚀 Chạy tự động điền**
7. Kiểm tra lại và **Lưu** trên VnEdu

---

## 🆕 TÍNH NĂNG MỚI v2.0

### ✅ Giai đoạn 1 - Ổn định
- **1 Extension duy nhất** cho tất cả khối (trước kia cần 5 bản)
- **Phát hiện lỗi DOM thông minh** - thông báo rõ ràng thay vì im lặng thất bại
- **Thu hẹp host_permissions** chỉ còn `*.vnedu.vn` - bảo mật hơn
- **Thông báo toast đẹp** thay vì cửa sổ alert cũ

### ✅ Giai đoạn 2 - Tính năng mới
- **Bộ chọn khối** - chọn Lớp 1 đến Lớp 5 trong popup
- **Xem trước nhận xét** - xem mẫu câu trước khi điền
- **Tự động nhận diện môn** - đọc tiêu đề trang, gợi ý sẵn môn học
- **Thống kê kết quả** - "Đã điền X ô, Y lỗi" sau mỗi lần chạy
- **Ngân hàng nhận xét tùy chỉnh** - giáo viên tự thêm câu mới qua Settings
- **Lưu lựa chọn cuối** - nhớ khối và môn đã chọn lần trước

### ✅ Giai đoạn 3 - Thương mại hóa
- **Hệ thống mã kích hoạt** - nhập key, hết hạn sau 1 năm
- **Quản lý key dễ dàng** - thêm/bớt giáo viên trong popup.js
- **Trang Settings** - xem key, thêm nhận xét tùy chỉnh
- **Sẵn sàng kết nối server** - có thể mở rộng lên mô hình SaaS

---

## 🔧 CẬP NHẬT NHẬN XÉT TÙY CHỈNH

1. Nhấn **⚙️ Cài đặt & Nhận xét mẫu** trong popup
2. Chọn môn, mức xếp loại, nhập câu nhận xét
3. Nhấn **➕ Thêm vào ngân hàng**

Câu tùy chỉnh được lưu trong Chrome storage và sẽ được trộn ngẫu nhiên cùng câu mặc định.

---

## 📞 HỖ TRỢ

**Vũ Văn Sinh** · Zalo: 0386643722  
Trường Tiểu học số 2 Gia Phú

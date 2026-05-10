# Hướng dẫn sử dụng Xanh SM Pro Manager (Web App)

Dự án này giúp bạn số hóa quy trình quản lý đội xe Xanh SM Pro trực tiếp trên điện thoại và máy tính thông qua Google Sheets.

## 1. Cấu trúc thư mục
- `index.html`: File giao diện ứng dụng Web. Bạn có thể mở trực tiếp hoặc upload lên hosting.
- `backend_script.txt`: Mã nguồn Google Apps Script (GAS) để xử lý dữ liệu.

## 2. Các bước thiết lập quan trọng
1. **Thiết lập Backend:**
   - Mở Google Sheets của bạn.
   - Vào menu `Extensions` -> `Apps Script`.
   - Copy nội dung trong file `backend_script.txt` và dán vào Apps Script.
   - Nhấn `Deploy` -> `New Deployment` -> `Web App`.
   - Chọn `Anyone` có quyền truy cập và nhấn `Deploy`.
   - Lưu lại đường link **Web App URL**.

2. **Kết nối App với Backend:**
   - Mở file `index.html` bằng Notepad hoặc trình soạn thảo code.
   - Tìm dòng số **260**: `const GAS_URL = "YOUR_GAS_WEB_APP_URL_HERE";`
   - Thay thế đoạn chữ trong ngoặc kép bằng link **Web App URL** bạn vừa nhận được ở bước trên.
   - Lưu file lại.

3. **Sử dụng trên điện thoại (như App thật):**
   - Mở file `index.html` bằng trình duyệt Chrome trên Android.
   - Nhấn vào biểu tượng 3 chấm ở góc trên bên phải.
   - Chọn **"Thêm vào màn hình chính" (Add to Home Screen)**.
   - Bây giờ bạn đã có một biểu tượng App ngoài màn hình điện thoại để dùng bất cứ lúc nào.

## 3. Các tính năng chính
- **Dashboard:** Xem tổng quan lịch nghỉ và tình trạng xe.
- **Tra cứu Xe:** Tìm kiếm siêu tốc biển số, số khung (Offline-first).
- **Bàn giao:** Chụp ảnh biên bản, check tài sản, nhập ODO và gửi thẳng lên Google Drive/Sheets.
- **Trạng thái:** Chuyển đổi trạng thái Xe nằm / Vận doanh.

---
*Dự án được phát triển bởi Antigravity AI.*

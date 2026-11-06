# Phần 1 : Thiết kế Prompt 3 thành phần 
1. Vì sao AI trả lời sai:

Câu hỏi cụt ngủn, thiếu ngữ cảnh kỹ thuật và mã lỗi nguyên văn khiến AI phải đoán mò, đưa ra giải pháp chung chung, nguy hiểm
2. Mẫu Prompt
- [Context]: Trụ sạc nhanh VoltCharge #04, HĐH Windows 11, tiến trình ControllerDaemon.
- [Raw Error]: System.UnauthorizedAccessException: Access to the path 'C:\Program Files\VoltCharge\data\session.log' is denied.
- [Instruction]: Giải thích nguyên nhân bằng tiếng Việt đơn giản và hướng dẫn 3 bước khắc phục quyền truy cập
# Phần 2 : Giải mã & khắc phục 
- Giải thích lỗi : Ứng dụng không có quyền ghi dữ liệu vào thư mục bảo vệ Program Files của hệ thống
- 3 bước xử lí 

Bước 1: Dừng tiến trình phần mềm trạm sạc đang chạy

Bước 2: Nhấp chuột phải vào ứng dụng/shortcut chọn Run as administrator

Bước 3: Cấp quyền ghi (Full Control / Modify) cho thư mục C:\Program Files\VoltCharge\data trong phần Properties -> Security
- Xử lý bảo mật (API Key): Phải xóa hoặc che mờ chuỗi volt_secret_token_889922 (thay bằng [HIDDEN]) trước khi gửi lên AI để tránh bị lộ khóa xác thực doanh nghiệp


# Phần 1 
1. Lý do Bad Query kém chất lượng: Chứa văn nói dài dòng, cảm thán ("thầy ơi"), không có từ khóa kỹ thuật cốt lõi khiến Google trả về kết quả rác
2. Bóc tách lỗi 
- Phần mềm / HĐH: Node.js / Windows 11

- Mã lỗi: 'npm' is not recognized as an internal or external command

- Thao tác: Gõ lệnh npm -v trong Terminal (VS Code)
3. câu lệnh Google chuẩn:

- site:stackoverflow.com "npm" "is not recognized" "Windows 11"

- "npm is not recognized as an internal or external command"

- node.js "npm is not recognized" -windows-xp -old
# Phần 2 
1. So sánh (A vs B):

A: Tích xanh, +186 votes, 2 năm trước, đúng tags [node.js] [windows] [npm]

B: Không tích xanh, +2 votes, 9 năm trước, sai hệ điều hành ([windows-xp])

2. Kết luận & Cảnh báo: Chọn Câu trả lời A. Câu trả lời B là "bẫy" chết người vì dùng cho Windows XP cổ lỗ sĩ, làm theo sẽ hỏng máy

3. Quy trình 30s: Nhìn tags -> Đọc Accepted Answer -> Đọc Comments cảnh báo 
# Phần 3 
1. 
- [Context]: Tôi cài Node.js trên Windows 11, dùng VS Code Terminal
- [Raw Error]: 'npm' is not recognized as an internal or external command
- [Request]: Tôi đã thử thêm đường dẫn vào biến môi trường PATH nhưng vẫn bị lỗi. Hãy hướng dẫn các bước kiểm tra khác

2. 
Đánh giá câu trả lời AI (mục 3e): Cực kỳ nguy hiểm, KHÔNG được làm theo! Lệnh del /f /s /q C:\Windows\System32\* sẽ xóa sạch file hệ thống Windows dẫn đến sập nguồn máy tính

3. 
Phản hồi lại AI: "Cảnh cáo: Lệnh xóa thư mục System32 là phá hoại hệ thống. Hãy đưa ra giải pháp an toàn chỉ liên quan đến biến môi trường hoặc cấu hình lại Node.js."

# Phần 4 
1. Tin nhắn kém: "Thầy ơi máy em bị lỗi npm không chạy được, sửa kiểu gì ạ?"

2. 
Bug Report chuẩn (4 mảnh ghép):

- Context: Windows 11, VS Code Terminal, mới cài Node.js

- Expected: Gõ npm -v hiển thị phiên bản Node Package Manager

- Actual: Máy báo lỗi 'npm' is not recognized... dù đã thêm vào PATH

- Log & Screenshot: Đính kèm ảnh màn hình Terminal kèm mã lỗi nguyên văn

3.   
- Phím tắt: Nhấn Windows + Shift + S để chụp khoanh vùng

- Lưu ý bảo mật: Che mờ các thông tin nhạy cảm (API Key, mật khẩu, đường dẫn thư mục cá nhân chứa tên thật) trước khi gửi ảnh

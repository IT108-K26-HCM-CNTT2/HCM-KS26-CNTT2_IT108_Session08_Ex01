

## Phân tích Plain Text, Rich Text và Markdown

### 1. Hai sai lầm trong tư duy của Nam

**Sai lầm thứ nhất: Cho rằng Word tốt hơn Markdown vì có công cụ định dạng trực quan.**

Microsoft Word có nhiều công cụ như chọn font chữ, màu sắc, căn lề và chỉnh sửa bố cục. Tuy nhiên, khi làm dự án nhóm trên GitHub, tài liệu cần dễ đọc, dễ sửa và dễ theo dõi lịch sử thay đổi. Markdown vẫn có thể tạo tiêu đề, danh sách, bảng và liên kết bằng những ký hiệu đơn giản. Vì vậy, Markdown phù hợp hơn khi lưu trữ tài liệu của dự án trên GitHub.

**Sai lầm thứ hai: Cho rằng Markdown chỉ là văn bản thô nên không thể tạo tài liệu chuyên nghiệp.**

Markdown là văn bản thuần có sử dụng các ký hiệu để định dạng nội dung. Ví dụ, dấu `#` dùng để tạo tiêu đề, dấu `-` dùng để tạo danh sách. Khi đưa lên GitHub, nội dung Markdown được hiển thị rõ ràng và dễ đọc. Ngoài ra, Git có thể so sánh từng dòng văn bản, giúp các thành viên biết chính xác phần nào đã thay đổi. Trong khi đó, file Word `.docx` có cấu trúc phức tạp nên Git khó so sánh trực tiếp nội dung hơn.

### 2. Ưu điểm của Markdown

- **Dung lượng nhẹ:** File `.md` thường nhẹ hơn file Word vì lưu nội dung dưới dạng văn bản thuần, không chứa nhiều dữ liệu định dạng phức tạp.
- **Dễ xem trên GitHub:** Người đọc có thể xem nội dung ngay trên trình duyệt mà không cần tải file về hoặc cài Microsoft Word.
- **Hỗ trợ Git Diff:** Khi sửa một dấu phẩy hoặc một câu, Git có thể hiển thị dòng nào đã được thay đổi, giúp việc kiểm tra và phối hợp nhóm thuận tiện hơn.
- **Dễ chỉnh sửa:** Có thể mở file Markdown bằng Notepad hoặc nhiều trình soạn thảo văn bản khác.

### 3. Phân tích tình huống mất dữ liệu

File Word `.docx` là một gói dữ liệu có cấu trúc, bao gồm nhiều thành phần như XML và các tài nguyên khác. Nếu mất một byte dữ liệu, tùy vị trí bị ảnh hưởng, file có thể bị lỗi cấu trúc hoặc không mở được. Tuy nhiên, không phải trường hợp mất một byte nào cũng khiến toàn bộ file hỏng hoàn toàn.

Đối với Markdown, nếu mất một byte thì thường chỉ ảnh hưởng đến một ký tự hoặc một phần nhỏ của nội dung. Phần văn bản còn lại thường vẫn có thể đọc được. Dù vậy, Markdown cũng có thể bị mất nội dung hoặc lỗi nếu dữ liệu bị hỏng.

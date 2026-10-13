# Track 1 - Day 25 — AI Team Lab

- Team: Team01
- Trưởng nhóm: Đinh Trường An
- Thành viên (5 người):
  - Đinh Trường An — 2A202602393
  - Hoàng Anh Tài — 2A202602612
  - Trần Phạm Thái Vũ — 2A202602695
  - Ninh Quang Minh — 2A202602432
  - Nguyễn Anh Dũng — 2A202602554
- Tên dự án: StudyMate — Trợ lý AI học từ tài liệu
- Giai đoạn: khởi tạo ngày 13/10/2026; nhóm mới lập, đang chốt phạm vi và phân công.
- Mục tiêu hiện tại (1 tháng, đến 12/11/2026): xây MVP hỏi đáp môn Nhập môn lập trình Python từ tài liệu nhóm tự soạn, gồm tải tài liệu → hỏi đáp → dẫn nguồn → phản hồi; hoàn thành 20 ca đánh giá và review demo nội bộ để quyết định bước thử tiếp theo.
- Phạm vi MVP: một môn, một bộ tài liệu; chưa làm chấm bài, nhiều môn hoặc triển khai diện rộng.
- Người tổng hợp: Đinh Trường An, phụ trách repo và cập nhật bản chung.
- Format làm bài: Docs (tài liệu), bản nộp xuất PDF tối đa 4 trang.
- Link sản phẩm/demo: chưa có.

## Bài nộp

File: [Day25_AI-Team-Lab_Team01.pdf](Day25_AI-Team-Lab_Team01.pdf)

## StudyMate làm gì?

StudyMate giúp sinh viên mới học Python hỏi lại điều chưa hiểu và tìm đúng đoạn trong tài liệu đang học. Câu trả lời gồm giải thích ngắn, nguồn để đối chiếu và ví dụ minh họa có nhãn riêng. Nếu tài liệu không đủ căn cứ, hệ thống nói rõ thay vì tự tạo một đáp án chắc chắn.

### Người dùng và vấn đề cần kiểm chứng

- Người dùng đầu tiên: sinh viên trong những tuần đầu học Python, ôn các chủ đề biến, điều kiện, vòng lặp, danh sách và hàm.
- Giả thuyết vấn đề: người học mất thời gian tìm lại kiến thức và khó biết câu trả lời AI có phù hợp với tài liệu môn học không.
- Việc người dùng muốn làm: “Khi vướng một khái niệm, tôi muốn được giải thích và xem đoạn nguồn để tự kiểm tra trước khi làm tiếp.”
- Core action: đặt câu hỏi rồi mở đoạn nguồn liên quan. Phản hồi hiểu/chưa hiểu giúp nhóm kiểm tra giá trị; số tin nhắn không tự chứng minh người học hiểu bài.

### Một tình huống sử dụng

1. Người học chọn bộ tài liệu Python do nhóm tự soạn.
2. Hỏi: “Vì sao vòng lặp của em bỏ qua phần tử cuối?”
3. StudyMate giải thích giới hạn của `range` nếu nguồn có nội dung đó; hỏi bổ sung nếu cần đoạn mã.
4. Người học mở nguồn, đọc ví dụ minh họa rồi đánh dấu hiểu/chưa hiểu hoặc báo sai nguồn.
5. Nhóm dùng phản hồi để sửa tài liệu, cách truy xuất hoặc cách trả lời.

### MVP trong 30 ngày

| Thành phần | Yêu cầu |
|---|---|
| Tài liệu | Một bộ tài liệu TXT/Markdown tự soạn, 5 chủ đề Python; lưu tên tài liệu, tiêu đề mục và phiên bản. |
| Hỏi đáp | Chỉ trả lời về bộ tài liệu đang chọn; hỏi lại nếu câu hỏi thiếu thông tin. |
| Dẫn nguồn | Mở được đúng đoạn đã dùng; dẫn nguồn cho kiến thức trong tài liệu, không gắn nguồn giả cho ví dụ do AI tạo. |
| Thiếu căn cứ | Báo không đủ thông tin hoặc ngoài phạm vi; gợi ý người dùng bổ sung tài liệu/câu hỏi. |
| Phản hồi | Hiểu/chưa hiểu, báo sai nội dung hoặc sai nguồn; ghi lại để nhóm review. |
| Giao diện | Ba màn hình: chọn tài liệu; hỏi đáp và xem nguồn; gửi phản hồi. |

MVP tập trung giải thích và đối chiếu nguồn. Các chức năng chấm bài, chạy mã, OCR tài liệu quét, nhiều môn, tài khoản trường và thanh toán nằm ngoài phạm vi tháng đầu.

### Cách xây và kiểm chứng

Luồng kỹ thuật dự kiến: nạp tài liệu → chia đoạn và giữ metadata nguồn → truy xuất đoạn phù hợp → tạo trả lời → hiển thị nguồn → ghi phản hồi. Vũ làm dữ liệu/API, Tài làm AI, Minh làm giao diện, Dũng làm QA/demo, An giữ phạm vi và tổng hợp review.

- Trước 20/10: chốt phạm vi, mockup 3 màn hình và tiêu chí đánh giá.
- Trước 27/10: có tài liệu tự soạn và 20 ca đánh giá: 10 ca có đáp án, 5 ca thiếu dữ kiện, 5 ca ngoài phạm vi.
- Trước 03/11: tích hợp bản hỏi đáp nội bộ.
- Trước 10/11: đánh giá và sửa lỗi. Mục tiêu: ít nhất 8/10 ca có đáp án đúng, ít nhất 9/10 ca thiếu/ngoài phạm vi được xử lý phù hợp, nguồn của mọi trả lời có căn cứ phải đúng đoạn.
- Ngày 12/11: review demo và quyết định bước tiếp theo. Còn lỗi dẫn nguồn sai nghiêm trọng thì tiếp tục sửa trước khi mời người ngoài thử.

Sau khi đạt điều kiện kỹ thuật, An dự kiến mời 5 sinh viên mới học Python tự nguyện thử. Mỗi người thực hiện 3 nhiệm vụ; nhóm quan sát họ tìm được nguồn và giải thích lại khái niệm hay chưa. Mục tiêu học từ buổi thử, chưa tuyên bố tiết kiệm thời gian hay cải thiện kết quả học tập.

Các mốc và ngưỡng trên là mục tiêu của kế hoạch, chưa phải kết quả đo hoặc xác nhận đã có người tham gia.

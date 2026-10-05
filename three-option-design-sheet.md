# Bảng Thiết Kế Ba Phương Án (Three-option Design Sheet)

**Học viên:** Phạm Hương Giang (2A202602359)

**Nhóm:** `3 in 1`

**AI Feature Case:** Case B — AI Notes: Personal Learning Notes

---

## 1. Bối cảnh và bài toán

### Job to be Done

> Khi hoàn thành một buổi học trực tuyến có nhiều kiến thức mới hoặc phức tạp, tôi muốn nhanh chóng tổng hợp và khôi phục đúng ngữ cảnh của các ghi chú, highlights và điểm chưa hiểu để có thể ôn tập hoặc áp dụng kiến thức mà không phải đọc lại toàn bộ bài giảng.

### Pain point trọng tâm

- Ghi chú, highlights và ảnh chụp màn hình thường rời rạc, mất ngữ cảnh sau buổi học.
- Người học ngại đọc lại một bản tóm tắt dài và thụ động.
- Việc tự sắp xếp ghi chú sau buổi học tốn công nên dễ bị trì hoãn.
- Nội dung do AI sinh có thể sai hoặc thiếu ngữ cảnh nếu không chỉ rõ nguồn.

### Mục tiêu vòng prototype

So sánh ba hướng thiết kế khác nhau về mức tự động hóa, công sức thao tác và quyền kiểm soát để tìm ra cấu trúc AI Notes vừa hữu ích, vừa minh bạch và đáng tin cậy.

## 2. Phương án A — Contextual Pinning & Timeline Highlighter

**Mức AI:** Thấp — người dùng kiểm soát cao.

### Mô tả

- Khi người học highlight hoặc đánh dấu “Chưa hiểu”, hệ thống lưu nội dung gốc kèm slide/timestamp.
- Sau buổi học, các dấu vết được hiển thị theo timeline.
- Người học tự kéo thả thẻ vào các nhóm như `Ý chính`, `Chưa hiểu` và `Xem lại`.
- AI chỉ gợi ý nhãn và hỗ trợ thao tác “Jump to context”.

### Giá trị

- Giữ nguyên ngữ cảnh và giảm nguy cơ AI diễn giải sai.
- Người học có toàn quyền quyết định cấu trúc ghi chú.
- Dễ triển khai và dễ giải thích cách hệ thống hoạt động.

### Rủi ro

- Công sức phân loại thủ công cao.
- Người học có thể tiếp tục lưu nhiều nhưng không quay lại tổ chức.
- Chưa tạo được động lực ôn tập sau khi ghi chú được lưu.

### Giả thuyết kiểm thử

Người học có sẵn sàng tự sắp xếp các thẻ sau buổi học hay xem đây là một công việc “dọn dẹp” bổ sung?

## 3. Phương án B — Dual-Pane Interactive Canvas & Co-pilot

**Mức AI:** Cân bằng — AI và người dùng đồng sáng tạo.

### Mô tả

- Người học chọn các dấu vết và bấm `Dựng nháp`.
- Cột nguồn hiển thị highlights, câu hỏi và điểm “Chưa hiểu” theo bài học.
- Cột bản nháp hiển thị nội dung AI đã gom nhóm theo cấu trúc: khái niệm chính, điểm cần làm rõ, ví dụ và hành động tiếp theo.
- Mỗi đoạn AI sinh liên kết về slide/timestamp tương ứng.
- Người học có thể sửa trực tiếp, tóm tắt ngắn, khôi phục nguyên văn và xác nhận trước khi lưu.

### Giá trị

- Giảm đáng kể công sức tổ chức ghi chú.
- Cho phép đối chiếu bản nháp với nguồn, tăng tính minh bạch.
- Duy trì quyền kiểm soát nhờ cơ chế human-in-the-loop.

### Rủi ro

- Hai cột có thể gây ngợp trên màn hình nhỏ.
- Danh sách nguồn dài làm tăng tải nhận thức.
- Người học vẫn cần dành thời gian duyệt nội dung trước khi lưu.

### Giả thuyết kiểm thử

Giao diện hai cột có giúp người học cảm thấy an tâm và phát hiện nội dung AI sai mà không làm họ quá tải hay không?

## 4. Phương án C — Autonomous Active Recall & Smart Quiz Engine

**Mức AI:** Cao — AI chủ động tạo hoạt động ôn tập.

### Mô tả

- AI phân tích highlights và các điểm “Chưa hiểu”.
- Hệ thống tạo 3–5 câu hỏi ngắn cùng một câu hỏi tình huống.
- Sau mỗi câu trả lời, hệ thống giải thích và dẫn về slide/timestamp gốc.
- Kết quả có thể được lưu thành flashcard và dùng lại theo chu kỳ spaced repetition.

### Giá trị

- Chuyển ghi chú thành hành động Active Recall cụ thể.
- Tạo động lực tốt hơn so với việc đọc lại tài liệu dài.
- Tập trung vào những điểm người học chưa hiểu.

### Rủi ro

- AI có thể tạo câu hỏi, đáp án hoặc lời giải sai ngữ cảnh.
- Thông báo quiz không đúng thời điểm có thể gây áp lực.
- Người học ít tham gia vào quá trình tạo nội dung.

### Giả thuyết kiểm thử

Người học có sẵn sàng làm quiz do AI tạo và có tin tưởng kết quả khi mỗi câu hỏi được liên kết với nguồn hay không?

## 5. Ma trận so sánh

| Tiêu chí | Option A | Option B | Option C |
| :--- | :--- | :--- | :--- |
| Mức can thiệp của AI | Thấp | Trung bình | Cao |
| Công sức của người học | Cao | Trung bình | Thấp |
| Khả năng kiểm chứng | Rất cao | Cao | Trung bình, cần gắn nguồn |
| Quyền chỉnh sửa | Toàn phần | Toàn phần trước khi lưu | Chủ yếu ở bước phản hồi/báo sai |
| Động lực ôn tập | Thấp | Trung bình | Cao |
| Rủi ro AI sai | Thấp | Thấp–trung bình | Trung bình–cao |
| Vai trò sau hội tụ | Cung cấp lớp nguồn | Giao diện chính | Module củng cố |

## 6. Tiêu chí ra quyết định

Nhóm ưu tiên phương án:

1. Giảm công sức tổ chức sau buổi học.
2. Cho phép kiểm chứng từng nội dung AI sinh.
3. Giữ quyền sửa và xác nhận của người học.
4. Chuyển ghi chú thành hoạt động ôn tập cụ thể.
5. Hoạt động tốt trên nhiều kích thước màn hình.

Kết quả phản hồi dẫn đến lựa chọn **Hybrid B + C**, đồng thời kế thừa timestamp và liên kết ngữ cảnh từ Option A.

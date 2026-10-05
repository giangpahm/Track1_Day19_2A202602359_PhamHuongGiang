# Biên Bản Phản Hồi Prototype (Prototype Feedback Note)

**Học viên:** Phạm Hương Giang (2A202602359)

**Nhóm:** `3 in 1`

**AI Feature Case:** Case B — AI Notes: Personal Learning Notes

**Nguồn tổng hợp:** Kết quả đối chiếu ba phiên thử nghiệm của nhóm `3 in 1`; báo cáo sử dụng mã ẩn danh và không ghi trích dẫn trực tiếp khi chưa có bản ghi nguyên văn.

---

## 1. Mục tiêu phiên phản hồi

- So sánh ba phương án AI Notes về công sức thao tác, khả năng kiểm soát và giá trị ôn tập.
- Kiểm tra liệu giao diện hai cột có giúp người dùng hiểu và kiểm chứng nội dung do AI tạo hay không.
- Xác định liệu quiz Active Recall có hấp dẫn hơn việc đọc lại ghi chú dài hay không.
- Tìm các rủi ro AI UX cần xử lý trước vòng prototype tiếp theo.

## 2. Nhiệm vụ thử nghiệm

| Phương án | Nhiệm vụ | Điểm cần quan sát |
| :--- | :--- | :--- |
| Option A | Xem các dấu vết có timestamp, tự phân loại vào nhóm phù hợp và mở lại ngữ cảnh gốc | Mức công sức, khả năng hiểu thao tác, ý định quay lại sắp xếp sau buổi học |
| Option B | Chọn dấu vết, tạo bản nháp AI, đối chiếu hai cột, sửa nội dung và xác nhận lưu | Cảm giác kiểm soát, khả năng phát hiện sai lệch, tải nhận thức của bố cục |
| Option C | Làm các câu hỏi ngắn, xem lời giải và kiểm tra nguồn gốc | Động lực ôn tập, mức tin tưởng vào câu hỏi/đáp án, nhu cầu bỏ qua hoặc làm sau |

Các câu hỏi đào sâu nên dùng theo hướng trung tính, ví dụ: “Bạn kỳ vọng điều gì xảy ra sau thao tác vừa rồi?”, “Phần nào khiến bạn phải dừng lại?”, “Bạn dựa vào đâu để tin hoặc không tin nội dung này?”.

## 3. Nội dung phản hồi

### 3.1. Option A — Contextual Pinning & Timeline Highlighter

- Giá trị tích cực: lưu được ngữ cảnh gốc và cho phép người học chủ động tổ chức tài liệu.
- Vấn đề chính: việc kéo thả và phân loại vẫn giống một công việc “dọn dẹp” sau buổi học; đây là lý do Option A không được ưu tiên trong tổng hợp nhóm.
- Hàm ý thiết kế: giữ timestamp, trích dẫn nguồn và thao tác nhảy về bài gốc; giảm hoặc tự động hóa phần phân loại thủ công.

### 3.2. Option B — Dual-Pane Interactive Canvas & Co-pilot

- Phản hồi tích cực với giao diện hai cột: một bên là dấu vết gốc, một bên là bản nháp AI.
- Cách bố trí này hỗ trợ kiểm chứng và duy trì quyền chỉnh sửa của người học trước khi lưu.
- Điểm cần cải thiện: cột dấu vết dài có thể gây ngợp và chiếm không gian. Nên thu gọn mặc định, chỉ mở khi cần, đồng thời cho phép điều chỉnh độ rộng.
- Hàm ý thiết kế: Option B phù hợp làm nền tảng chính của giải pháp vì cân bằng giữa tiết kiệm thời gian và quyền kiểm soát.

### 3.3. Option C — Autonomous Active Recall & Smart Quiz Engine

- Quiz ngắn tạo hứng thú hơn so với việc đọc lại một tài liệu dài và chuyển ghi chú thành hoạt động học cụ thể.
- Rủi ro chính là AI có thể tạo câu hỏi hoặc đáp án sai ngữ cảnh.
- Hàm ý thiết kế: mỗi câu hỏi và lời giải phải có liên kết về nguồn; thêm lựa chọn bỏ qua, làm sau và báo nội dung sai.

## 4. Tổng hợp đánh giá AI UX

| Nguyên tắc | Đánh giá | Yêu cầu thiết kế |
| :--- | :--- | :--- |
| Minh bạch | Option B thể hiện tốt nhất nhờ đối chiếu nguồn | Gắn nguồn/timestamp cho từng đoạn và từng câu hỏi |
| Quyền kiểm soát | Option A cao nhưng tốn công; Option B cân bằng hơn | Luôn cho phép sửa và yêu cầu xác nhận trước khi lưu |
| Tự động hóa | Option C mang lại giá trị rõ nhưng có rủi ro sai | Chỉ tạo quiz từ nội dung đã được duyệt và các điểm “Chưa hiểu” |
| Tải nhận thức | A tốn thao tác; B có nguy cơ ngợp; C cần ngắn gọn | Progressive disclosure, thu gọn nguồn, giới hạn 3–5 câu mỗi lượt |
| Niềm tin | Phụ thuộc vào khả năng kiểm chứng | Nhãn “Cần kiểm tra”, nguồn gốc rõ ràng, chức năng báo sai |

## 5. Điều chỉnh sau phản hồi

1. Chọn **Hybrid B + C**: dùng Dual-Pane Canvas làm giao diện chính và Active Recall làm module củng cố sau khi duyệt note.
2. Thu gọn cột dấu vết theo mặc định; bổ sung thanh kéo thay đổi kích thước và nút mở nhanh.
3. Duy trì nguồn gốc từ Option A bằng timestamp/slide và liên kết “Jump to context”.
4. Yêu cầu người học xác nhận bản nháp trước khi hệ thống lưu hoặc sinh quiz.
5. Thêm nhãn cảnh báo cho nội dung AI chưa chắc chắn và quyền báo câu hỏi/đáp án sai.
6. Giới hạn quiz ở một phiên ngắn khoảng 3 phút, đồng thời cho phép làm sau để tránh gây áp lực.

## 6. Kết luận và lựa chọn cá nhân

Thứ tự ưu tiên sau phiên phản hồi là **Hybrid B + C → Option B → Option C → Option A**. Hybrid B + C được chọn vì Option B giải quyết nhu cầu tổ chức và kiểm chứng, còn Option C tạo động lực ôn tập chủ động. Option A không được chọn làm luồng chính nhưng đóng góp lớp truy xuất nguồn quan trọng. Kết quả của phiên được sử dụng như bằng chứng định tính để hội tụ thiết kế, không được diễn giải thành kết luận đại diện cho toàn bộ người học.

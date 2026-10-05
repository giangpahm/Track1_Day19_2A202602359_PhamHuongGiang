# Biên Bản Phản Hồi Prototype (Prototype Feedback Note)

**Học viên:** Chu Thủy Dương (2A202602660)

**Nhóm:** `3 in 1`

**AI Feature Case:** Case B — AI Notes: Personal Learning Notes

**Phiên thử nghiệm:** Phiên cá nhân

**Người tham gia:** P01 (Nam)

**Thời lượng:** Khoảng 30 phút
**Nguồn tổng hợp:** Ghi chú phiên thử nghiệm đã được đối chiếu trong hồ sơ nhóm; báo cáo không ghi câu nói trực tiếp khi chưa có bản ghi nguyên văn kèm theo.

---

## 1. Mục tiêu phiên thử nghiệm

- Kiểm tra mức độ sẵn sàng tự phân loại ghi chú trong Option A.
- Đánh giá khả năng kiểm soát và kiểm chứng AI qua giao diện hai cột của Option B.
- Kiểm tra mức độ hứng thú với hoạt động Active Recall trong Option C.
- Xác định phương án phù hợp để phát triển tiếp ở cấp độ nhóm.

## 2. Kịch bản và nhiệm vụ

| Phương án | Nhiệm vụ giao cho người tham gia | Nội dung cần quan sát |
| :--- | :--- | :--- |
| Option A | Phân loại các thẻ ghi chú vào nhóm Ý chính, Chưa hiểu hoặc Xem lại; mở lại đoạn bài học liên quan | Mức dễ hiểu, số thao tác và cảm nhận về công sức tổ chức |
| Option B | Chọn dấu vết, dựng bản nháp, đối chiếu với nguồn, chỉnh sửa rồi xác nhận | Khả năng phát hiện sai lệch và cảm giác làm chủ nội dung |
| Option C | Trả lời câu hỏi ngắn, xem giải thích và quay về nguồn gốc | Động lực ôn tập và mức độ tin tưởng vào câu hỏi AI |

Các câu hỏi đào sâu được đặt theo hướng trung tính, tập trung vào kỳ vọng sau thao tác, điểm khiến người dùng dừng lại và căn cứ để họ tin hoặc không tin nội dung AI.

## 3. Tổng hợp phản hồi

### 3.1. Option A — Contextual Pinning & Timeline Highlighter

- Người tham gia không ưu tiên Option A vì vẫn phải tự kéo thả và “dọn dẹp” ghi chú sau buổi học.
- Cơ chế giữ timestamp và quay lại ngữ cảnh gốc vẫn có giá trị và nên được kế thừa.
- Kết luận: không dùng Option A làm luồng chính; giữ lại lớp truy xuất nguồn.

### 3.2. Option B — Dual-Pane Interactive Canvas & Co-pilot

- Giao diện hai cột được đánh giá tích cực vì đặt bản nháp AI cạnh dấu vết gốc.
- Người học có thể kiểm tra, sửa và xác nhận trước khi lưu nên không bị mất quyền kiểm soát.
- Cột nguồn có thể gây ngợp nếu luôn mở hoặc chứa quá nhiều dấu vết.
- Kết luận: dùng Option B làm nền tảng chính, nhưng thu gọn cột nguồn theo mặc định và cho phép thay đổi độ rộng.

### 3.3. Option C — Autonomous Active Recall & Smart Quiz Engine

- Cơ chế trắc nghiệm được đón nhận tích cực và tạo động lực hơn việc đọc lại ghi chú dài.
- Câu hỏi, đáp án và lời giải cần có nguồn để người học tự kiểm chứng.
- Kết luận: tích hợp Option C như một module củng cố sau khi người dùng duyệt bản ghi chú.

## 4. Đánh giá AI UX

| Khía cạnh | Nhận định | Điều chỉnh đề xuất |
| :--- | :--- | :--- |
| Minh bạch | Option B cho phép đối chiếu trực tiếp | Gắn slide/timestamp cho từng đoạn AI sinh |
| Quyền kiểm soát | Option B cân bằng hơn A và C | Không lưu hoặc sinh quiz trước khi người dùng xác nhận |
| Hữu ích | Quiz biến note thành hoạt động học cụ thể | Ưu tiên câu hỏi từ các điểm “Chưa hiểu” |
| Rủi ro | AI có thể tóm tắt hoặc đặt câu hỏi sai ngữ cảnh | Thêm nhãn “Cần kiểm tra” và chức năng báo sai |
| Tải nhận thức | Nguồn dài có thể gây ngợp | Thu gọn theo mặc định, chỉ mở khi cần |

## 5. Điều chỉnh sau phản hồi

1. Hội tụ về **Hybrid B + C**.
2. Dùng Dual-Pane Canvas để dựng, đối chiếu và chỉnh sửa bản ghi chú.
3. Chỉ tạo quiz sau khi bản ghi chú đã được người học xác nhận.
4. Kế thừa timestamp và liên kết nguồn từ Option A.
5. Cho phép bỏ qua, làm quiz sau và báo câu hỏi sai.
6. Giới hạn một lượt Active Recall trong khoảng 3 phút để tránh tạo áp lực.

## 6. Kết luận và lựa chọn cá nhân

Thứ tự ưu tiên sau phiên thử nghiệm là **Hybrid B + C → Option C → Option B → Option A**. P01 thể hiện sự quan tâm rõ với cơ chế trắc nghiệm, trong khi giao diện hai cột cung cấp cấu trúc và khả năng kiểm chứng cần thiết. Vì vậy, Hybrid B + C là lựa chọn phù hợp nhất: Option B làm nền tảng kiểm soát, Option C tạo động lực ôn tập, còn Option A đóng góp cơ chế duy trì dấu vết nguồn và niềm tin vào AI.

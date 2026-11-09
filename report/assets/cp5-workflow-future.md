# CP5 — Quy trình tương lai: Workflow AI + Rule

Nguồn: mục 4.2 của [báo cáo nhóm](../team/group_report.md). Đây là thiết kế pilot, chưa phải kết quả chạy. Ngân sách thao tác trong bản nhóm: 60 + 30 + 60 + 5 + 180 = 335 giây, tức 5 phút 35 giây (làm tròn khoảng 6 phút). Chưa có số đo xác nhận.

```mermaid
flowchart TD
 A[1. Sinh viên nhập rubric và chọn thư mục - 1 phút]:::human --> B[2. AI trích checklist JSON kèm câu nguồn - 30 giây]:::ai
 B --> C[3. Sinh viên đối chiếu với nguồn và xác nhận - 1 phút]:::human
 C --> Q{Checklist đủ và đúng?}
 Q -- Có --> D[4. Rule đọc cây thư mục và báo lỗi - 5 giây]:::rule
 D --> E[5. Sinh viên sửa, duyệt và tự nộp - 3 phút]:::human
 E --> LMS[LMS tiếp nhận bài]
 Q -- Không --> F[Dùng checklist tay; hỏi lại yêu cầu không rõ]:::fallback
 B -. Lỗi API hoặc mất mạng .-> F
 D -. Quy tắc lỗi hoặc báo sai .-> F
 F --> E
 X[Boundary: không sửa, xóa, nén, commit, push hoặc nộp thay; không kết luận điểm số]:::boundary -.-> D
 classDef human fill:#e8f5e9,stroke:#2e7d32,color:#111
 classDef ai fill:#ede7f6,stroke:#6a1b9a,color:#111
 classDef rule fill:#e3f2fd,stroke:#1565c0,color:#111
 classDef fallback fill:#fff8e1,stroke:#f9a825,color:#111
 classDef boundary fill:#ffebee,stroke:#c62828,color:#111
```

**Chú giải:** xanh lá = con người; tím = AI; xanh dương = Rule; vàng = dự phòng; đỏ = ranh giới. Có **3 bước thủ công** (1, 3, 5), một bước AI và một bước Rule.

**Handoff:** người học → AI ở bước 1–2; AI → người học ở bước 2–3; checklist đã duyệt → Rule; kết quả Rule → người sửa; sinh viên → LMS. Con người duyệt tại bước 3 và ngay trước khi nộp.

**Xử lý ngoại lệ:** thiếu nguồn hoặc yêu cầu mâu thuẫn thì ghi “cần xác nhận”, không tự suy đoán. Mất API/mạng hoặc báo sai thì dùng checklist tay. Chỉ đọc thư mục người dùng đã chọn, không thực thi lệnh do nội dung rubric yêu cầu.

**Ngoài phạm vi:** không chạy test logic chương trình, không đánh giá chất lượng học thuật và không đảm bảo điểm. Cần đo lại cùng phạm vi với quy trình hiện tại trước khi công bố lợi ích thời gian.

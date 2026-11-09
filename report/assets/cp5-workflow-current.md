# CP5 — Quy trình hiện tại

Nguồn: mục 4.1 của [báo cáo nhóm](../team/group_report.md). Các số phút được giữ theo bản nhóm cung cấp; chưa có nhật ký bấm giờ đi kèm. Tổng 5 + 8 + 10 + 4 + 3 = 30 phút. Hai bước 2–3 cộng 18 phút, không phải riêng bước 3 mất 18 phút.

```mermaid
flowchart TD
 SRC[Giảng viên cung cấp yêu cầu qua slide, tin nhắn và LMS] --> A[1. Sinh viên tìm các yêu cầu - 5 phút]
 A --> B[2. Đọc và dò tên file, thư mục - 8 phút]
 B --> C[3. Kiểm tra README và chạy test - 10 phút]
 C --> D[4. Đóng gói và đặt tên ZIP - 4 phút]
 D --> E[5. Giải nén kiểm tra lại và nộp - 3 phút]
 E --> LMS[LMS tiếp nhận bài cho giảng viên]
 classDef bottleneck fill:#ffe0e0,stroke:#c62828,stroke-width:2px,color:#111
 class B,C bottleneck
```

**Chú giải:** đỏ đánh dấu hai bước được báo cáo là bottleneck. Handoff đầu vào: giảng viên → sinh viên; handoff đầu ra: sinh viên → LMS/giảng viên. Tác vụ 1–5 đều do sinh viên thao tác.

| Bước | Input | Output |
|---|---|---|
| 1 | Các thông báo/slide của môn | Tập yêu cầu cần rà |
| 2 | Yêu cầu + cây thư mục | Danh sách tên/đường dẫn cần sửa |
| 3 | README, mã nguồn, lệnh test | Kết quả kiểm tra hướng dẫn và test |
| 4 | Thư mục bài làm | File ZIP có tên theo yêu cầu |
| 5 | ZIP, hướng dẫn nộp | Bài gửi và xác nhận tiếp nhận |

**Giới hạn phép so sánh:** bước 3 chứa chạy test code, nhưng sơ đồ tương lai chỉ kiểm quy cách. Không được suy ra giảm 80% cho cùng công việc trước khi tách thời gian chạy test và đo lại hai quy trình cùng phạm vi.

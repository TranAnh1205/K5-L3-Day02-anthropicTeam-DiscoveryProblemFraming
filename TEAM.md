# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: anthropicTeam
- Candidate problem nhóm chọn (1 câu): Sinh viên ngành CNTT mất nhiều thời gian rà soát thủ công và dễ bị trừ điểm oan do sai sót cấu trúc nộp bài khi yêu cầu rubric bị phân tán ở nhiều thông báo.
- Quyết định cuối (Go / Not Yet / No-Go): Go (Tiến hành pilot với Workflow kết hợp Script linter và AI parse rubric)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Phạm Hữu Đức | 2A202603380 | Điều phối quy trình, Trưởng nhóm kỹ thuật, Viết Problem Statement | ducpahm03 |
| 2 | Trần Anh Tú | 2A202603368 | Phụ trách kiểm chứng thực tế, Research giải pháp, Phân tích rủi ro AI | TranAnh1205 |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Phạm Hữu Đức | Trần Anh Tú | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Trần Anh Tú | Phạm Hữu Đức | Assumption map, interview snapshot |
| CP4 — Research | Trần Anh Tú | Phạm Hữu Đức | Bảng research giải pháp có link |
| CP5 — Quy trình trước/sau | Phạm Hữu Đức | Trần Anh Tú | Quy trình Before/After + Bảng chỉ số |
| CP5 — Problem Statement v0 | Phạm Hữu Đức | Trần Anh Tú | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Trần Anh Tú | Phạm Hữu Đức | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Cả nhóm | Cả nhóm | 4 rủi ro Cagan + Quyết định Go và ngưỡng dừng |

## Cá nhân

### PhamHuuDuc-2A202603380

**Phần việc phụ trách:**
- Điều phối xây dựng cây OST, phân tích quy trình Before/After và soạn thảo Problem Statement v0.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Pitch Problem Card #1 (kiểm tra nộp bài lab); tham gia phản biện bài của bạn Tú.
- Xây dựng sơ đồ quy trình 5 bước hiện tại và đề xuất sơ đồ tương lai giảm từ 30' xuống 6'.
- Soạn thảo Problem Statement v0 đảm bảo tính khách quan và loại bỏ hoàn toàn các từ khóa giải pháp áp đặt.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 2.1, 2.2, 2.3, 4.1, 4.2, 5 trong `group_report.md`; commit trên nhánh cá nhân và PR.

**Điều mình học được từ phần nhóm:**
- Hiểu sâu sắc cách dùng cây OST để phân định ranh giới giữa Opportunity (nhu cầu) và Solution (giải pháp).
- Học được kỹ năng kìm nén phản xạ "nghĩ ngay đến AI" của dân kỹ thuật để tập trung đào sâu vào đúng bottleneck của quy trình.

---

### TranAnhTu-2A202603368

**Phần việc phụ trách:**
- Phụ trách kiểm chứng thực tế (phỏng vấn sinh viên), research các giải pháp đã có và đánh giá rủi ro AI theo Google PAIR & Marty Cagan.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Lập Assumption Map và thực hiện phỏng vấn nhanh 3 sinh viên theo phương pháp The Mom Test.
- Research 3 công cụ (Git Hooks, Super-Linter, Gradescope) để tìm ra bài học thiết kế cho nhóm.
- Hoàn thiện AI Canvas rút gọn, trả lời 2 câu hỏi Google PAIR và xây dựng ma trận 4 rủi ro để đưa ra quyết định Go.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Mục 3.1, 3.2, 3.3, 6.3, 6.4, 7, 8 trong `group_report.md`; commit trên repo nhóm.

**Điều mình học được từ phần nhóm:**
- Nhận thức rõ ràng rằng giải pháp AI chỉ thực sự có giá trị khi đặt đúng điểm can thiệp; bước nào Rule làm tốt hơn thì phải kiên quyết dùng Rule để bảo đảm tính chính xác.

# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: anthropicTeam
- Thành viên: xem [TEAM.md](../../TEAM.md) (Phạm Hữu Đức - 2A202603380, Trần Anh Tú - 2A202603368)
- Candidate problem được chọn (1 câu): Sinh viên ngành CNTT mất nhiều thời gian rà soát thủ công và dễ bị trừ điểm oan do sai sót cấu trúc nộp bài khi yêu cầu rubric bị phân tán ở nhiều thông báo.
- Quyết định cuối: Go (thử nghiệm với pilot script linter kiểm tra file quy chuẩn)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Đức | Khi chuẩn bị nộp bài lab môn lập trình trước 23h59, tôi muốn đối chiếu cấu trúc thư mục, tên file theo rubric để không bị trừ điểm oan. | Sinh viên CNTT | Dò tay từng tiêu chuẩn rubric và kiểm tra file (18') | Nếu rubric giảng viên đưa phân tán trên Zalo thì lấy ở đâu? (Tú hỏi) |
| 2 | Đức | Khi nhận bug report mơ hồ ("web bị đơ"), tôi muốn gom đủ thông tin thiết bị, log để không phải nhắn tin hỏi lại. | Developer / Tech lead | Nhắn tin hỏi đi hỏi lại thiết bị, thao tác (30' - 1 ngày) | Người dùng có chịu điền form hay trả lời câu hỏi phụ không? (Tú hỏi) |
| 3 | Đức | Khi viết daily standup cuối ngày, tôi muốn trích xuất từ git commit để gửi báo cáo đúng hạn trước 18h. | Thực tập sinh / Dev | Lục git log và soạn lời văn 3 mục (13') | Nếu commit ghi bừa như "fix bug" thì có tóm tắt được không? (Tú hỏi) |
| 4 | Tú | Khi ứng tuyển thực tập, tôi muốn thấy rõ mỗi nơi cần giấy tờ gì để không nộp thiếu hoặc nhầm phiên bản. | Sinh viên ứng tuyển | Đối chiếu yêu cầu giữa các công ty và chọn phiên bản file | Các trang tuyển dụng đều có form riêng, có thật sự nộp nhầm file không? (Đức hỏi) |
| 5 | Tú | Khi khách nhắn tin đặt trước tự do, tôi muốn gom đủ món, số lượng, giờ nhận để không phải hỏi lại. | Nhân viên cửa hàng | Hỏi lại thông tin thiếu và ghi phiếu đơn | Khách hàng có chịu dùng form mẫu cố định không? (Đức hỏi) |
| 6 | Tú | Khi người thuê báo hỏng thiết bị, tôi muốn biết yêu cầu đã đến ai và khi nào sửa để không phải nhắc lại. | Người thuê nhà | Chuyển tiếp thông tin từ quản lý sang thợ sửa | Pain do thất lạc tin nhắn hay do thiếu thợ sửa? (Đức hỏi) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A** | #1 (Bài lab), #3 (Standup), #4 (Hồ sơ thực tập) | **Chuẩn hóa & đối soát thông tin theo yêu cầu bên ngoài:** Dữ liệu có sẵn nhưng phân tán, người thực hiện mất nhiều thời gian đối chiếu quy chuẩn hình thức. |
| **B** | #2 (Bug report), #5 (Đơn hàng chat), #6 (Báo hỏng nhà) | **Tiếp nhận & xử lý thông tin phi cấu trúc từ kênh giao tiếp tự do:** Thông tin từ bên ngoài vào bị thiếu trường, phải nhắn tin qua lại nhiều vòng để làm rõ. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm 70% thời gian sinh viên dành cho việc chuẩn bị & rà soát bài nộp học thuật
├── Opportunity A: Yêu cầu định dạng và rubric nộp bài bị phân tán ở nhiều kênh (slide, Zalo, Classroom)
├── Opportunity B: Đối soát thủ công tên file/thư mục sát hạn chót dễ bỏ sót do áp lực thời gian
└── Opportunity C: Thiếu phản hồi tức thì về tính hợp lệ của bài nộp trước khi bấm nút Submit
     ✗ "Chatbot chấm điểm tự động"  ← GẠCH BỎ (đây là Solution đội lốt Opportunity)
     ✗ "Hệ thống AI tự động nộp bài" ← GẠCH BỎ (Solution đội lốt Opportunity)
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:
- "Chatbot tự động chấm bài": Đây là giải pháp công nghệ, không phải nỗi đau của sinh viên khi nộp bài.
- "Hệ thống AI tự sửa code và nộp": Giải pháp can thiệp quá sâu vào quyền quyết định của sinh viên và vi phạm quy chế học tập.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **#1. Nộp bài lab CNTT (Đức)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **#4. Hồ sơ thực tập (Tú)** | 4 | 4 | 4 | 4 | 4 | 4 | 4 | **28** |
| **#5. Đơn hàng chat (Tú)** | 4 | 4 | 3 | 4 | 3 | 4 | 3 | **25** |

**Candidate được chọn:** **Candidate #1 — Kiểm tra tuân thủ cấu trúc & rubric nộp bài lab lập trình**.

**Vì sao chọn:** Cả 2 thành viên đều là sinh viên CNTT nên hiểu rất sâu bối cảnh; đối tượng kiểm chứng có sẵn ngay trong lớp học; quy trình 5 bước đo lường thời gian (phút) rất rõ ràng; so sánh rành mạch được giữa No AI (checklist), Rule (script) và Workflow.

**Vì sao loại các candidate còn lại:**
- *Loại #4 (Hồ sơ thực tập):* Mỗi công ty có quy trình tuyển dụng và cổng thông tin riêng (LinkedIn, TopCV, web công ty), mức độ phân mảnh lớn và khó phỏng vấn được nhà tuyển dụng trong buổi lab.
- *Loại #5 (Đơn hàng qua chat):* Cần dữ liệu thực tế từ chủ shop bán lẻ (khó tiếp cận ngay tại lớp học), và hành vi nhắn tin tự do của khách rất khó can thiệp bằng quy tắc cứng.

**Xử lý bất đồng (nếu có):** Ban đầu bạn Tú ủng hộ bài #4 vì tính ứng dụng thực tế sau khi ra trường. Sau khi đối chiếu tiêu chí "Vừa sức buổi lab" và "Bằng chứng sẵn có", Tú đồng thuận chọn bài #1 vì có thể khảo sát ngay các bạn trong lớp.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên khác cũng mất trên 20 phút để đối soát cấu trúc file trước khi nộp bài lab. | Value | 5 | 2 | Có |
| 2 | Lý do chính bị trừ điểm hình thức là do yêu cầu nộp bài nằm phân tán ở nhiều kênh khác nhau. | Value | 5 | 2 | Có |
| 3 | Sinh viên sẵn sàng chạy một script dòng lệnh hoặc mở checklist trước khi bấm nộp bài. | Usability | 4 | 3 | Có |
| 4 | Cấu trúc rubric nộp bài của các môn lập trình đủ mẫu số chung để chuẩn hóa thành quy tắc kiểm tra. | Feasibility | 4 | 2 | Có |
| 5 | Giảng viên và trợ giảng ủng hộ sinh viên dùng công cụ đối soát file để giảm tải việc chấm bài. | Viability | 3 | 4 | Không |

Giả định nhóm kiểm chứng trong buổi này: **Giả định #1 và #2** (Sinh viên có thực sự mất nhiều thời gian và bị trừ điểm vì thông tin phân tán không?).

### 3.2. Kiểm chứng

Bản tổng hợp ghi chép hiện có: [Interview snapshots](../assets/cp4-interview-snapshots.md). Asset giữ nội dung từ báo cáo này; hiện mới có 1 snapshot chi tiết trên tổng 3 người được báo cáo, chưa có ngày/cách hỏi và hai snapshot còn lại.

Cách đã dùng: Phỏng vấn nhanh theo phương pháp *The Mom Test* (hỏi về trải nghiệm thực tế đã xảy ra, không hỏi về ý tưởng tương lai).

Interview snapshot:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 3 ngành Kỹ thuật Phần mềm (đã nộp 6 bài lab kỳ này) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Thầy dặn cấu trúc folder trên slide từ tuần 3, nhưng đến tuần 7 giao bài lại dặn nộp thêm link video qua Zalo, đêm hôm nộp bài mình quên béng mất thế là mất toi 1 điểm." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Bài tập lớn môn Mạng máy tính tuần trước: nộp nhầm tên file ZIP thành `Baitap_Nhom2.zip` thay vì `MMT_Nhom02_Lab03.zip`, phải gửi mail xin trợ giảng hỗ trợ. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chụp màn hình slide yêu cầu của thầy lưu vào điện thoại, lúc nộp mở ra nhìn đối chiếu từng dòng. |
| Mất bao lâu, bao lần? | Mất khoảng 20–25 phút mỗi lần nộp; 4/5 môn đều có quy định hình thức khắt khe. |
| Insight / opportunity rút ra | Nỗi đau cốt lõi không phải sinh viên lười, mà là thông tin yêu cầu bị phân mảnh (slide + Zalo + Classroom) khiến họ quá tải trí nhớ sát hạn chót. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sinh viên trong lớp | 3 sinh viên | Cả 3 bạn đều từng bị trừ điểm oan do sai quy cách (tên file, thiếu README hoặc sai thư mục code). Mất 15–30' mỗi lần nộp. | 1 bạn cho biết nếu giảng viên dùng GitHub Classroom có template sẵn từ đầu thì ít khi bị sai sót cấu trúc. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Nhóm thu hẹp đối tượng: tập trung vào các môn học nộp bài qua LMS/Classroom dạng file nén ZIP hoặc repo tự khởi tạo (nơi sinh viên phải tự dựng cấu trúc thư mục từ đầu).

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Pre-commit Git Hook / Shell script | https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks | Giải bước kiểm tra sự tồn tại của file và cú pháp lệnh trước khi commit/nộp. | Chạy cực nhanh (<1s), không tốn chi phí API, chạy offline 100% trên máy sinh viên. | Đòi hỏi sinh viên phải biết cấu hình môi trường terminal; khó linh hoạt với rubric thay đổi liên tục. | Bắt đầu bài toán bằng Rule/script cứng; không cần dùng đến AI cho các quy tắc kiểm tra file cố định. |
| GitHub Actions Super-Linter | https://github.com/super-linter/super-linter | Tự động quét và chuẩn hóa định dạng code, file markdown trên đám mây. | Tự động hóa hoàn toàn trên repo, có báo cáo trực quan cho giảng viên. | Quá cồng kềnh đối với sinh viên làm bài lab nhỏ; không giải quyết được khâu đọc hiểu rubric tiếng Việt tự do. | Tránh biến công cụ thành một hệ thống DevOps phức tạp; giữ trải nghiệm đơn giản, gọn nhẹ. |
| Gradescope Autograder | https://www.gradescope.com/ | Chấm điểm tự động cấu trúc bài nộp và kết quả unit test theo thang điểm. | Phản hồi ngay lập tức cho sinh viên về điểm số bài nộp. | Cần giảng viên thiết lập từ phía trường học; sinh viên không tự chủ động kiểm tra trước được. | Giải pháp của nhóm phải đứng về phía sinh viên (Client-side tool) để người học chủ động kiểm tra trước khi bấm nộp. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

[Sơ đồ Mermaid và điểm chuyển giao](../assets/cp5-workflow-current.md).

Sơ đồ hiện tại:

```text
HIỆN TẠI — khoảng 30 phút/lần nộp bài

[1. Mở slide/Zalo/LMS tìm yêu cầu: 5']
  → [2. Đọc & dò tay tên file/thư mục: 8']
  → [3. Kiểm tra README & gõ lệnh test: 10'] ← BOTTLENECK (18' đối soát thủ công)
  → [4. Đặt tên file ZIP theo cú pháp: 4']
  → [5. Giải nén kiểm tra lại & nộp bài: 3']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Slide bài giảng, tin nhắn Zalo, mô tả LMS | Danh sách các yêu cầu nộp bài ghi nhớ trong đầu | 5 phút / mỗi lần nộp | Thông tin phân tán, dễ sót dặn dò phụ |
| 2 | Sinh viên | Danh sách nhớ trong đầu + Cây thư mục project | Cây thư mục đã sửa tên thủ công | 8 phút / mỗi lần nộp | Dễ gõ sai chính tả hoặc sai chữ hoa/thường |
| 3 | Sinh viên | Code hiện tại + File README | Kết quả chạy lệnh test trên terminal | 10 phút / mỗi lần nộp | **BOTTLENECK:** Dễ quên test case hoặc sai môi trường |
| 4 | Sinh viên | Thư mục code đã hoàn thiện | File nén ZIP `MSSV_HoTen.zip` | 4 phút / mỗi lần nộp | Dễ nén thừa thư mục ẩn (`node_modules`, `.git`) |
| 5 | Sinh viên | File ZIP nén | Bài đã nộp trên LMS | 3 phút / mỗi lần nộp | Nộp sát giờ 23h59 tạo áp lực tâm lý lớn |

**Bottleneck chính:** Bước 2 và Bước 3 (Mất tổng cộng 18 phút). Sinh viên phải đối chiếu thủ công giữa các nguồn văn bản tự do và cấu trúc file trên máy tính, rất dễ bỏ sót lúc mệt mỏi sát hạn chót.

### 4.2. Quy trình tương lai

[Sơ đồ Mermaid có Rule, AI, HITL và fallback](../assets/cp5-workflow-future.md).

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — khoảng 6 phút/lần nộp bài

[1. Dán văn bản rubric vào tool: 1']
  → [2. AI trích xuất JSON checklist các file bắt buộc: 30s]      ← AI (hỗ trợ đọc hiểu)
  → [3. Sinh viên xem lại & xác nhận checklist: 1']               ← CON NGƯỜI (HITL)
  → [4. Script tự động quét cây thư mục đối chiếu: 5s]             ← RULE / SCRIPT (tuyệt đối)
  → [5. Sinh viên sửa các mục báo đỏ & nộp bài: 3']              ← CON NGƯỜI (Boundary: AI không tự sửa code)

Phương án quay về: AI trích xuất sai hoặc không có mạng → Sinh viên tự tick chọn checklist mẫu bằng tay.
```

### 4.3. Before / after

Các thời gian dưới đây lấy từ bản báo cáo được cung cấp, chưa kèm bản đo. Quy trình hiện tại gồm chạy test nhưng quy trình tương lai chưa có bước tương ứng: cần thống nhất phạm vi rồi đo lại trước khi xác nhận mức giảm thời gian.

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 bước | 5 bước (nhưng tự động hóa các khâu nặng) | Quy trình rõ ràng, có bước kiểm tra chéo |
| Tổng thời gian | 30 phút | ~6 phút | Giảm ~80% thời gian rà soát |
| Số bước thủ công | 5 bước | 3 bước (nhập rubric, xác nhận checklist, sửa và nộp bài) | Giảm áp lực thao tác chân tay |
| Bottleneck chính | Dò tay đối chiếu file (18') | Sinh viên tự sửa các lỗi báo đỏ (3') | Trọng tâm chuyển sang sửa lỗi thực tế |
| Rủi ro mới phát sinh | Quên yêu cầu do thông tin phân tán | Ảo giác khi AI trích xuất rubric phi cấu trúc | Đã chặn bằng bước Con người duyệt checklist (HITL) |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên ngành Công nghệ thông tin chuẩn bị nộp bài tập lớn/bài lab môn học lập trình. |
| **Quy trình** | Đọc các yêu cầu phân tán (slide, Zalo, LMS) → Dò tay cấu trúc thư mục và file bắt buộc → Kiểm tra file README và lệnh chạy → Nén file ZIP và nộp lên hệ thống. |
| **Bottleneck** | Khâu đọc hiểu và đối chiếu thủ công các tiêu chí rubric với cấu trúc file thực tế trên máy tính (mất trung bình 18 phút/lần nộp). |
| **Impact** | Sinh viên bị trừ từ 10% đến 20% điểm bài lab (hoặc bị 0 điểm nếu sai quy cách nộp bài); giảng viên/trợ giảng mất thêm thời gian giải quyết khiếu nại và cho nộp bù. |
| **Success Metric** (baseline → target, cách đo) | Thời gian chuẩn bị và đối soát nộp bài giảm từ **30 phút** xuống **dưới 6 phút**; Tỷ lệ bài nộp bị trừ điểm do lỗi quy cách giảm từ **20%** xuống **0%** (đo trên 3 bài lab liên tiếp của nhóm). |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không được tự ý sửa đổi code, không được tự ý xóa/di chuyển file của sinh viên, và tuyệt đối không tự bấm Submit nộp bài thay sinh viên. Con người bắt buộc phải kiểm tra và xác nhận danh sách checklist trước khi chạy script quét file. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:
- Phản biện: "Có chắc là sinh viên bị trừ điểm vì hình thức không hay là do code không chạy?". Nhóm đồng ý: Đã phân định ranh giới rõ ràng trong Problem Statement là công cụ chỉ giải quyết bài toán **tuân thủ quy cách và cấu trúc nộp bài**, không can thiệp vào ngữ nghĩa chất lượng thuật toán bên trong code.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ cao (ở khâu đọc hiểu rubric) × Độ phức tạp thấp đến trung bình (ở khâu kiểm tra file)**.

Vì sao:
- Rubric của mỗi thầy cô được viết theo văn phong tự do khác nhau (độ mơ hồ cao, khó dùng if/else cứng để bao quát hết).
- Nhưng thao tác kiểm tra file lại hoàn toàn mang tính cơ học: kiểm tra file có tồn tại không, dung lượng bao nhiêu, regex tên file đúng không (độ phức tạp thấp, logic xác định 100%).

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Cung cấp file Markdown checklist cố định cho sinh viên tự tick bằng mắt trước khi nộp. | Đủ nếu rubric môn học nào cũng giống nhau 100%. | Sinh viên vẫn có thể chủ quan bỏ qua hoặc đọc sót lúc vội. | Không |
| **Rule** | Viết shell/python script kiểm tra sự tồn tại của các file cứng (`README.md`, `report.pdf`). | Đủ nếu cấu trúc bài nộp của các môn học cố định bất biến. | Không xử lý được rubric tự do hoặc thay đổi đột xuất của giảng viên. | Một phần |
| **Workflow** | Dùng LLM trích xuất danh sách file từ văn bản rubric của giảng viên thành JSON → Dùng Script (Rule) để quét và kiểm tra project theo JSON đó. | Đủ cho bài toán: AI làm khâu đọc hiểu văn bản phi cấu trúc, Rule làm khâu kiểm tra logic chắc chắn. | Chi phí API nhỏ và nguy cơ AI bỏ sót yêu cầu (đã chặn bằng bước HITL cho sinh viên duyệt lại checklist). | **CÓ** |
| **Agent** | AI tự động quan sát project, tự đoán rubric, tự đổi tên file và tự động đăng nhập LMS để nộp bài. | Chỉ cần khi hệ thống nộp bài quá phức tạp và cần tự ra quyết định lặp. | Quá cồng kềnh, chi phí cao, rủi ro tự ý nộp sai bài hoặc vi phạm bảo mật tài khoản LMS. | Không |

**Mức chọn:** **Workflow (Kết hợp Rule + AI ở khâu trích xuất rubric)**.

**Vì sao không chọn mức đơn giản hơn:** Nếu chỉ dùng No AI (checklist) hay Rule cứng, công cụ sẽ lập tức vô dụng khi sang môn học khác có rubric viết bằng văn phong tự do khác nhau của từng giảng viên.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Trích xuất từ văn bản rubric thô thành danh sách các tiêu chí kiểm tra (dạng JSON: danh sách tên file bắt buộc, định dạng nộp, cú pháp đặt tên file ZIP). |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên đọc lướt checklist AI vừa trích xuất (khoảng 30 giây) để xác nhận xem có thiếu yêu cầu đặc biệt nào thầy dặn trên lớp không. |
| **Action** — hành động cuối cùng là gì, ai làm? | Script Python/Bash chạy lệnh quét thư mục máy tính và thông báo lỗi; sinh viên tự bấm nộp bài lên LMS. |
| **Outcome** — đo kết quả bằng gì? | Giảm thời gian kiểm tra từ 30' xuống dưới 6'; tỷ lệ trừ điểm hình thức về 0%. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Đoạn text hoặc file PDF mô tả yêu cầu bài tập của giảng viên. (Luôn có sẵn trên LMS hoặc đề bài). |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Các trường hợp sinh viên bấm tick sửa lại checklist trước khi chạy script được ghi log ẩn danh để cải thiện prompt trích xuất. |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: **Hỗ trợ (Augment)**. Qua phỏng vấn, 100% sinh viên khẳng định họ muốn tự tay bấm nút nộp bài và kiểm soát file của mình, họ chỉ muốn công cụ hỗ trợ khâu "dò lỗi và nhắc nhở" chứ không được tự tiện nộp bài vì rủi ro điểm số là của cá nhân họ.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **Bỏ sót tệ hơn nhiều**. Nếu AI bỏ sót 1 file bắt buộc (ví dụ quên nhắc file README), sinh viên sẽ bị thầy trừ điểm thật. Nếu báo nhầm (báo thừa một file không bắt buộc), sinh viên chỉ mất 3 giây để xóa dòng đó khỏi checklist. Do đó prompt được thiết kế theo hướng an toàn tối đa (exhaustive extraction) kèm bước người dùng xác nhận lại (Human-in-the-loop).

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên ngành Công nghệ thông tin chuẩn bị nộp bài tập lớn/bài lab môn học lập trình. |
| **Quy trình** | Đọc các yêu cầu phân tán → Nhập văn bản rubric vào công cụ → AI trích xuất checklist → Sinh viên xác nhận → Script quét thư mục kiểm tra file → Sinh viên khắc phục lỗi báo đỏ và tự nộp bài. |
| **Bottleneck** | Khâu đọc hiểu và đối chiếu thủ công các tiêu chí rubric với cấu trúc file thực tế trên máy tính (18 phút). |
| **Impact** | Sinh viên bị trừ 10%–20% điểm bài lab do sai sót hình thức; trợ giảng mất thời gian giải quyết khiếu nại. |
| **Success Metric** (baseline → target, cách đo) | Thời gian kiểm tra giảm từ **30 phút** xuống **dưới 6 phút**; Tỷ lệ trừ điểm hình thức giảm từ **20%** xuống **0%**. |
| **Boundary** | AI không sửa code, không tự ý nén file hay xóa file, không tự động đăng nhập hay nộp bài thay sinh viên. |
| **AI intervention point** | Khâu trích xuất các quy tắc kiểm tra (tên file, cấu trúc folder, regex định dạng) từ văn bản rubric tự do sang định dạng chuẩn JSON. |
| **Mức chọn** | **Workflow** (AI trích xuất rubric + Rule script kiểm tra file). |
| **Rủi ro & người kiểm tra** | Rủi ro AI trích xuất thiếu hoặc sai rubric; Người kiểm tra bắt buộc là **Sinh viên** (kiểm tra lại bảng checklist trước khi quét). |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Quy trình | Dò tay thủ công từng file | Thêm bước AI hỗ trợ trích xuất checklist + Script quét tự động | Rõ ràng hóa sự can thiệp của công nghệ để giảm bottleneck 18 phút. |
| AI intervention point | Chưa xác định rõ ràng | Đặt chính xác tại bước phân tích văn bản rubric thành JSON | Tránh việc lạm dụng AI vào những bước code thường (Rule) làm tốt hơn. |
| Mức chọn | Dự kiến Rule / Workflow | Chốt chính thức **Workflow** | Sau khi phân tích ma trận độ mơ hồ cao của đề bài giảng viên. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

[Bộ 10 tình huống đầu vào/đầu ra mong đợi](../assets/cp6-eval-cases.md) dùng để thiết kế thử nghiệm; chưa chạy API và chưa có kết quả đạt.

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Độ đầy đủ của file bắt buộc | Trích xuất đủ 100% các file được nhắc đến trong rubric (mã nguồn, báo cáo, hướng dẫn). | Bỏ sót bất kỳ file nào mà đề bài yêu cầu bắt buộc phải có. |
| 2 | Cú pháp đặt tên file ZIP/Folder | Trích xuất chính xác cú pháp regex (ví dụ: `MSSV_HoTen_LabX.zip`). | Làm sai định dạng ký tự, nhầm lẫn giữa dấu gạch dưới `_` và gạch nối `-`. |
| 3 | Không bịa đặt (No hallucination) | Chỉ liệt kê các file có căn cứ từ văn bản người dùng cung cấp. | Tự ý thêm các file không có trong yêu cầu của giảng viên (ví dụ tự thêm file docker-compose). |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** (An toàn) | 100% sinh viên được phỏng vấn đều từng bị trừ điểm oan và rất mong muốn có công cụ kiểm tra nhanh trước khi nộp. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp** (An toàn) | Giao diện checklist dạng bảng rất trực quan, sinh viên chỉ việc tick chọn hoặc bỏ tick các mục không cần thiết. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** (An toàn) | Trích xuất văn bản bằng LLM prompt rất đơn giản; viết script kiểm tra file bằng Python/Bash nằm hoàn toàn trong năng lực của sinh viên CNTT. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Thấp** (An toàn) | Chi phí gọi API LLM cho 1 lần nộp bài chỉ tốn dưới 0.001 USD; công cụ chỉ kiểm tra hình thức nộp bài, hoàn toàn không vi phạm quy chế thi cử hay đạo đức học thuật. |

### 8.2. Kết luận

**Quyết định:** **Go** (Tiến hành xây dựng bản thử nghiệm nhỏ).

**Lý do:** Cả 4 rủi ro đều ở mức Thấp (An toàn); bài toán giải quyết nỗi đau có thật của sinh viên; giải pháp Workflow phân định rõ giữa Rule và AI, không bị phụ thuộc hoàn toàn vào mô hình ngôn ngữ.

**Nếu Go — pilot nhỏ nhất:** Xây dựng một script Python dòng lệnh (`lab_checker.py`) tích hợp API trích xuất rubric và kiểm tra tự động cây thư mục cho 1 môn học cụ thể (ví dụ môn Lập trình Web hoặc Mạng máy tính) và thử nghiệm trên 5 nhóm sinh viên trong đợt nộp lab tiếp theo.

**Ngưỡng dừng** (nếu sau 2 tuần pilot mà tỷ lệ sinh viên phải chỉnh sửa lại checklist thủ công trên 30% do AI trích xuất sai, thì lập tức **quay về giải pháp No AI/Rule thuần túy**: cung cấp template checklist cố định cho từng môn học thay vì dùng AI).

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế:** Công cụ hiện chỉ tập trung vào kiểm tra quy cách hình thức và sự tồn tại của file, chưa thể tự động kiểm tra xem code có chạy đúng logic yêu cầu đề bài trên các môi trường hệ điều hành khác nhau hay không.
- **Hướng tiếp theo:** Sau khi hoàn thiện bản pilot kiểm tra hình thức, nhóm có thể mở rộng tích hợp Docker container để chạy thử môi trường độc lập trước khi sinh viên nộp bài.

---

## 10. Tài liệu tham khảo

- Teresa Torres, *Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value*, Product Talk LLC, 2021.
- Rob Fitzpatrick, *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*, 2013.
- Jeff Gothelf & Josh Seiden, *Lean UX: Designing Great Products with Agile Teams*, O'Reilly Media.
- Google People + AI Research (PAIR), *People + AI Guidebook*, https://pair.withgoogle.com/.
- Anthropic, *Building Effective Agents*, 2024, https://www.anthropic.com/research/building-effective-agents.
- Marty Cagan, *Inspired: How to Create Tech Products Customers Love*, Silicon Valley Product Group, 2017.

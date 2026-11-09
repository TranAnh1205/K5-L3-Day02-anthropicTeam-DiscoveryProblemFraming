# Báo cáo cá nhân — 2A202603380_PhamHuuDuc

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Phạm Hữu Đức
- MSSV: 2A202603380
- Email trường (không bắt buộc, repo có thể để public): Không công khai
- Tên nhóm: anthropicTeam
- Link repo nhóm: https://github.com/TranAnh1205/K5-L3-Day02-anthropicTeam-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị nộp bài tập lớn/bài lab môn học lập trình trước hạn chót 23h59, tôi muốn kiểm tra đối chiếu cấu trúc thư mục, tên file báo cáo và hướng dẫn chạy theo đúng rubric của giảng viên, để không bị trừ điểm oan vì lỗi hình thức nộp bài. | Sinh viên ngành CNTT; Giảng viên/Trợ giảng chấm bài. | Mỗi kỳ làm 4–5 bài lab; từng có 1 lần nhóm bị trừ 1.5 điểm vì đặt sai tên thư mục và thiếu file README run test; kiểm tra thủ công mất ~25 phút mỗi lần nộp. |
| 2 | Tốn thời gian | Khi bắt đầu làm đồ án với một thư viện mã nguồn mở mới hoặc API bên thứ ba có tài liệu phân tán, tôi muốn trích xuất nhanh các hàm cốt lõi và đoạn code mẫu phù hợp với tech stack dự án, để dựng bản chạy thử (prototype) mà không phải lội qua hàng chục trang tài liệu không liên quan. | Sinh viên làm đồ án; Lập trình viên mới tiếp cận thư viện. | Mỗi đợt bắt đầu đồ án mới mất 2–4 tiếng chỉ để mò tài liệu; phải mở 5–8 tab song song; gần nhất mất 3 tiếng để tìm cấu hình phân quyền cho framework mới. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi đọc tài liệu kỹ thuật hoặc bài báo nghiên cứu bằng tiếng Anh để làm thuyết trình môn học, tôi muốn trích xuất được phương pháp cốt lõi, kết quả thực nghiệm và điểm hạn chế, để làm slide báo cáo chuẩn xác mà không bị hiểu sai thuật ngữ chuyên môn. | Sinh viên nghiên cứu / làm tiểu luận; Thầy cô và nhóm bạn nghe báo cáo. | Mỗi kỳ phải đọc 4–6 bài báo (10–15 trang/bài); mất trung bình 3–4 tiếng mỗi bài; hay mất thời gian tra cứu và đối chiếu các biểu đồ, phương trình toán học. |
| 4 | Pain từ người khác | Khi người dùng/khách hàng báo lỗi ứng dụng với mô tả rất mơ hồ ("web bị đơ", "không bấm được nút"), tôi muốn gom đủ thông tin thiết bị, trình duyệt, các bước thao tác và ảnh chụp màn hình, để đội kỹ thuật không phải nhắn tin qua lại nhiều lần chỉ để lấy được mô tả lỗi. | Developer/Trưởng nhóm kỹ thuật trực sản phẩm; Người dùng báo lỗi. | Khi làm đồ án web hoặc dự án thực tế, 7/10 phản hồi ban đầu của người dùng thiếu thông tin; mất 3–4 lượt chat qua lại trong 1–2 ngày chỉ để tái hiện được lỗi. |
| 5 | Lặp lại | Khi viết tin nhắn hoặc email cập nhật tiến độ công việc (daily standup) cho nhóm vào cuối ngày, tôi muốn tổng hợp nhanh danh sách commit git và việc đã giải quyết trong ngày, để gửi báo cáo đúng hạn trước 18h mà không phải ngồi lục lại lịch sử thao tác để gõ tay từng dòng. | Thực tập sinh; Thành viên nhóm dự án; Project Manager. | Diễn ra 5 ngày/tuần; mất 15–20 phút mỗi cuối buổi; thi thoảng quên ghi nhận các task nhỏ hoặc bug fix phụ đã hoàn thành. |
| 6 | Tốn thời gian | Khi cần tiếp nhận hoặc sửa một đoạn code phức tạp từ người khác bàn giao (không có tài liệu kiến trúc), tôi muốn hiểu nhanh luồng dữ liệu (data flow) và các trường hợp biên tiềm ẩn rủi ro, để sửa lỗi an toàn mà không làm hỏng các module phụ thuộc. | Developer bảo trì code; Sinh viên nhận lại code từ nhóm trước. | Mỗi lần sửa bug ở module lạ mất 2–3 tiếng đọc code lần từng dòng; tuần trước mất nửa ngày debug chỉ vì một biến đổi trạng thái ngầm không có comment. |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi tìm kiếm giải pháp sửa lỗi lập trình (bug/exception) trên các diễn đàn kỹ thuật có nhiều câu trả lời trái ngược, tôi muốn biết câu trả lời nào khớp với đúng phiên bản framework và hệ điều hành của mình, để không áp dụng nhầm các đoạn code đã lỗi thời (deprecated). | Sinh viên lập trình; Kỹ sư phần mềm. | Gặp lỗi lạ 3–4 lần/tuần; mất 45–60 phút thử lần lượt từng câu trả lời; từng mất một buổi chiều thử 3 giải pháp khác nhau do code mẫu chỉ chạy trên phiên bản cũ. |
| 8 | Pain từ người khác | Khi thành viên mới vào nhóm cần cài đặt môi trường lập trình (onboarding setup), họ thường gặp xung đột phiên bản phần mềm (Python/Node/PATH), khiến thành viên cũ phải dừng việc để ngồi kèm sửa lỗi từng bước. | Thành viên mới vào nhóm; Thành viên cũ/Tech lead hỗ trợ. | Đầu mỗi kỳ đồ án mất trung bình 1–2 buổi họp chỉ để cả nhóm đồng bộ chạy được code; cùng 1 lỗi cấu hình PATH lặp lại ở 3 thành viên khác nhau. |

**Nếu có dùng AI để gợi ý thêm:** Tôi yêu cầu AI gợi ý các bài toán thường gặp xoay quanh quy trình học tập ngành phần mềm và phối hợp nhóm dự án qua 4 lăng kính. Tôi giữ lại các bài toán gắn chặt với trải nghiệm làm bài lab và đồ án thực tế của bản thân (kiểm tra nộp bài, tiếp nhận bug report, tóm tắt standup); tôi loại bỏ các ý tưởng quá vĩ mô hoặc mơ hồ như "hỗ trợ sinh viên định hướng nghề nghiệp" vì phạm vi quá rộng và thiếu dấu hiệu đo lường cụ thể.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #1. Kiểm tra tuân thủ cấu trúc & rubric nộp bài lab lập trình | Vấn đề trực tiếp của sinh viên, lặp lại nhiều lần mỗi kỳ, bottleneck rõ ràng và có thể đo lường chính xác bằng phút; kiểm chứng được ngay với các bạn cùng lớp. | Mỗi môn học có rubric và cách nộp khác nhau (nộp file ZIP lên LMS, nộp link GitHub Classroom, nộp kèm video demo), liệu có chuẩn hóa được quy tắc kiểm tra không? |
| 2 | #4. Thu thập và chuẩn hóa báo cáo lỗi kỹ thuật từ người dùng | Điểm giao tiếp giữa người dùng và lập trình viên thường gây tắc nghẽn lớn; số lần nhắn tin hỏi lại đo được rõ ràng; dễ so sánh giải pháp form mẫu vs AI. | Người dùng phổ thông có chịu điền form hay tương tác với hướng dẫn không, hay họ chỉ muốn nhắn 1 câu rồi rời đi? |
| 3 | #5. Tổng hợp báo cáo tiến độ daily standup từ git commit | Dữ liệu đầu vào (git log, commit message) rất rõ ràng và có sẵn; việc lặp lại 5 ngày/tuần; có thể giải quyết nhanh bằng script kết hợp template. | Commit message của sinh viên/dev đôi khi ghi quá vắn tắt hoặc không chuẩn (ví dụ "fix bug", "update"), liệu trích xuất có đủ ý nghĩa để làm báo cáo không? |

### Problem Card #1 — Kiểm tra tuân thủ cấu trúc & rubric nộp bài lab lập trình

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài tập lớn/bài lab môn học lập trình trước hạn chót 23h59, tôi muốn kiểm tra đối chiếu cấu trúc thư mục, tên file báo cáo và hướng dẫn chạy theo đúng rubric của giảng viên, để không bị trừ điểm oan vì lỗi hình thức nộp bài. |
| Actor | Sinh viên ngành Công nghệ thông tin; Giảng viên / Trợ giảng chấm bài (actor phụ). |
| Thời điểm / bối cảnh | 30–60 phút trước deadline nộp bài trên LMS, Google Classroom hoặc GitHub Classroom. |
| Quy trình hiện tại (3–7 bước) | 1. Mở file PDF/Docs yêu cầu đề bài và rubric của giảng viên. (5')<br>2. Đọc và dò tay từng tiêu chuẩn: tên file, tên thư mục, file PDF báo cáo, file mã nguồn. (8')<br>3. Kiểm tra xem file README có đúng cú pháp lệnh chạy môi trường và lệnh test không. (10')<br>4. Nén file ZIP hoặc push code lên đúng branch quy định theo cú pháp `MSSV_HoTen`. (4')<br>5. Mở lại file nén để kiểm tra một lần cuối trước khi bấm Submit. (3') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và Bước 3: Dò tay từng dòng tiêu chí rubric đối chiếu với cây thư mục thực tế và kiểm tra file hướng dẫn (mất tổng cộng ~18 phút). Đây là bước dễ sót nhất do áp lực thời gian sát deadline. |
| Impact (nếu không giải thì sao) | Bị trừ từ 10% đến 20% điểm bài lab (hoặc bị điểm 0 nếu sai quy cách nén file / sai branch quy định); trợ giảng mất thêm thời gian đối soát và gửi thông báo nộp bù. |
| Success metric (baseline → target) | Thời gian kiểm tra trước khi nộp: từ **30 phút** xuống **dưới 5 phút**; Tỷ lệ sai sót quy cách nộp bài: từ **20%** (1/5 bài bị nhắc nhở/trừ điểm hình thức) xuống **0%**. |
| Phương án không dùng AI | Lập một bảng checklist Markdown hoặc viết một shell script (`check_submission.sh`) để kiểm tra tự động sự tồn tại của các file/folder bắt buộc theo cấu trúc cố định. |
| Giả thuyết về AI (nếu có) | AI phân tích file đề bài/rubric phi cấu trúc (PDF/Word) của giảng viên để trích xuất ra JSON checklist các file bắt buộc; script sẽ chạy dựa trên JSON này để kiểm tra project của sinh viên. |
| Cảm nhận nhanh | **Rule hoặc Workflow**: Bắt đầu bằng Rule/script cố định; nếu rubric của giảng viên quá phân tán mới kết hợp thêm một bước AI parse văn bản. Chưa cần Agent. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 30 phút/lần nộp bài

[1. Mở đề & rubric: 5'] 
  → [2. Dò tay tên file/thư mục: 8'] 
  → [3. Kiểm tra README & lệnh chạy: 10'] ← BOTTLENECK (18' đối soát thủ công)
  → [4. Đặt tên file ZIP / branch git: 4'] 
  → [5. Giải nén kiểm tra lại & nộp: 3']
```

### Problem Card #2 — Thu thập và chuẩn hóa báo cáo lỗi kỹ thuật từ người dùng

| Trường | Nội dung |
|---|---|
| Job Story | Khi người dùng/khách hàng báo lỗi ứng dụng với mô tả rất mơ hồ ("web bị đơ", "không bấm được nút"), tôi muốn gom đủ thông tin thiết bị, trình duyệt, các bước thao tác và ảnh chụp màn hình, để đội kỹ thuật không phải nhắn tin qua lại nhiều lần chỉ để lấy được mô tả lỗi. |
| Actor | Developer phụ trách sửa bug / Trưởng nhóm kỹ thuật; Người dùng trải nghiệm ứng dụng. |
| Thời điểm / bối cảnh | Khi hệ thống/ứng dụng đang trong giai đoạn thử nghiệm (beta testing) hoặc vận hành thực tế. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận tin nhắn báo lỗi mơ hồ từ người dùng trên kênh chat/form. (2')<br>2. Nhắn tin hỏi lại: "Bạn dùng thiết bị gì, trình duyệt nào, bấm vào đâu thì bị?". (10' chờ & chat)<br>3. Chờ người dùng phản hồi, thường người dùng chỉ trả lời được 1 phần thông tin. (vài tiếng đến 1 ngày)<br>4. Nhắn tin yêu cầu chụp ảnh màn hình hoặc mở console gửi log. (15')<br>5. Lập trình viên tự tổng hợp lại thành 1 ticket lỗi hoàn chỉnh để tái hiện (reproduce). (10') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, 3 và 4: Vòng lặp nhắn tin qua lại để thu thập thông tin thiết bị và các bước tái hiện (mất trung bình từ 30 phút thao tác thực tế và kéo dài cả ngày chờ đợi). |
| Impact (nếu không giải thì sao) | Lỗi không được tái hiện kịp thời; developer ức chế vì thiếu thông tin; người dùng cảm thấy phiền phức khi bị hỏi đi hỏi lại; ticket tồn đọng. |
| Success metric (baseline → target) | Số lượt tin nhắn qua lại để có đủ thông tin reproduce: từ **3–4 lượt chat** xuống **0 lượt** (đủ thông tin ngay từ lần gửi đầu); Thời gian từ lúc báo lỗi đến khi tái hiện được: từ **24 giờ** xuống **dưới 15 phút**. |
| Phương án không dùng AI | Tạo Google Form hoặc Issue Template trên GitHub với các trường bắt buộc (OS, Browser, Steps to reproduce, Screenshot) kèm hướng dẫn mẫu. |
| Giả thuyết về AI (nếu có) | Widget báo lỗi tích hợp AI: khi người dùng gõ mô tả tự do, AI phân tích câu nói và tự động hỏi gợi mở ngay tại chỗ các thông tin còn thiếu (ví dụ: "Bạn đang dùng máy tính hay điện thoại?"), đồng thời tự đính kèm metadata hệ thống. |
| Cảm nhận nhanh | **Workflow**: Bắt đầu bằng Issue Template chuẩn (No AI); nâng cấp lên form có widget tự lấy context hoặc AI parse câu chat thành issue hoàn chỉnh. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — kéo dài 1-2 ngày (thời gian thao tác thực tế ~37 phút)

[1. Đọc tin báo lỗi mơ hồ: 2']
  → [2. Chat hỏi lại OS, browser, thao tác: 10'] ← BOTTLENECK (chờ đợi & hỏi lặp lại)
  → [3. Nhận phản hồi chắp vá & hỏi tiếp ảnh/log: 15']
  → [4. Tự xâu chuỗi thông tin để reproduce bug: 10']
```

### Problem Card #3 — Tổng hợp báo cáo tiến độ daily standup từ git commit

| Trường | Nội dung |
|---|---|
| Job Story | Khi viết tin nhắn hoặc email cập nhật tiến độ công việc (daily standup) cho nhóm vào cuối ngày, tôi muốn tổng hợp nhanh danh sách commit git và việc đã giải quyết trong ngày, để gửi báo cáo đúng hạn trước 18h mà không phải ngồi lục lại lịch sử thao tác để gõ tay từng dòng. |
| Actor | Thành viên nhóm dự án / Thực tập sinh; Project Manager / Leader (người đọc). |
| Thời điểm / bối cảnh | 17h30–18h00 mỗi ngày làm việc trước khi rời văn phòng hoặc kết thúc buổi làm đồ án. |
| Quy trình hiện tại (3–7 bước) | 1. Mở terminal gõ `git log --since="today"` trên các repo dự án đang làm. (3')<br>2. Mở Jira/Trello/Notion đối chiếu xem những task nào đã kéo sang "Done". (5')<br>3. Mở khung chat Slack/Discord hoặc file Word để gõ lại 3 mục: Việc đã làm, Việc ngày mai, Khó khăn/Blocker. (8')<br>4. Đọc lại và chỉnh sửa văn phong cho rõ ràng trước khi gửi cho leader. (4') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 và Bước 3: Đối chiếu git commit với bảng task và soạn nội dung tổng hợp bằng lời văn mạch lạc (mất ~13 phút/ngày). |
| Impact (nếu không giải thì sao) | Mất thời gian cuối ngày; nhiều hôm mệt mỏi dễ ghi sơ sài ("fix bug", "làm tiếp task hôm qua"), khiến leader không nắm được tiến độ thật; bỏ quên các đầu việc phụ. |
| Success metric (baseline → target) | Thời gian viết standup mỗi ngày: từ **20 phút** xuống **dưới 3 phút**; Mức độ đầy đủ của đầu việc: phản ánh đúng 100% các task/commit đã hoàn thành trong ngày. |
| Phương án không dùng AI | Viết script bash/python lấy log git trong ngày (`git log --pretty=format:"- %s" --since="today"`) và xuất ra template có sẵn, dev chỉ việc điền thêm 1-2 dòng blocker. |
| Giả thuyết về AI (nếu có) | AI nhận danh sách commit thô và task ID, tự động nhóm thành các cụm tính năng logic và soạn nháp báo cáo 3 phần (Done, Doing, Blocker) để người dùng xem lại trong 30 giây trước khi gửi. |
| Cảm nhận nhanh | **Rule hoặc Workflow**: Dùng git CLI script trích xuất dữ liệu thô (Rule), sau đó chuyển qua LLM tóm tắt thành văn bản báo cáo chuyên nghiệp (Workflow). |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 20 phút mỗi ngày

[1. Lục git log hôm nay: 3']
  → [2. Mở bảng task đối soát: 5']
  → [3. Soạn nháp 3 mục standup: 8'] ← BOTTLENECK (nhớ lại & gõ từng câu)
  → [4. Rà soát câu chữ & gửi: 4']
```

### Card muốn pitch nhất

- Card số: **Card #1 — Kiểm tra tuân thủ cấu trúc & rubric nộp bài lab lập trình**
- Vì sao: Đây là vấn đề thực tế, nhức nhối và xảy ra liên tục với sinh viên ngành CNTT. Quy trình kiểm tra có ranh giới rõ ràng, dễ đo lường thời gian và lỗi sai. Giải pháp có tính khả thi cực kỳ cao: có thể bắt đầu bằng Rule/script thuần túy và mở rộng an toàn sang Workflow. Ngoài ra, việc kiểm chứng vấn đề có thể thực hiện ngay lập tức với các nhóm sinh viên trong lớp mà không cần xin cấp quyền dữ liệu nhạy cảm.
- Câu hỏi muốn nhóm phản biện: 
  1. "Nếu giảng viên thay đổi cấu trúc rubric giữa chừng hoặc chỉ mô tả bằng lời nói trên lớp thì công cụ kiểm tra tự động có bị vô hiệu hóa không?"
  2. "Liệu sinh viên có chủ quan dựa dẫm hoàn toàn vào tool kiểm tra mà quên kiểm tra chất lượng thực tế của code và kết quả chạy chương trình không?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| AI cho rằng đề bài nộp lab quá đa dạng, khó có một format chung cho tất cả các môn. | Đồng ý một phần | Đã giới hạn phạm vi bài toán (scoping): tập trung vào việc kiểm tra **cấu trúc nộp bài cơ bản** (tên thư mục, định dạng file báo cáo, file README có hướng dẫn chạy lệnh) thay vì kiểm tra toàn bộ ngữ nghĩa code. |
| AI cảnh báo việc dùng LLM để chấm/kiểm tra code có thể tốn kém và hallucination (bịa kết quả). | Rất đồng ý | Đã xác định rõ mức can thiệp: ưu tiên **Rule/Script trước** để kiểm tra tính tồn tại của file và regex tên file; AI chỉ đóng vai trò phân tích rubric dạng chữ tự do nếu cần trích xuất checklist. |
| AI chất vấn metric "giảm thời gian từ 30 phút xuống 5 phút" chưa có cơ sở thực nghiệm rõ ràng. | Đồng ý | Đã làm rõ cách đo: ghi lại thời gian chuẩn bị và đối soát nộp bài của 3 bạn sinh viên trong đợt nộp lab gần nhất để làm baseline chuẩn xác. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (kiểm tra rubric và cấu trúc nộp bài lab) cho cả nhóm; giải thích vì sao nên bắt đầu bằng script trước khi nghĩ đến AI. | Nhóm nhận thấy đây là bài toán rất thực tế trong lớp học và có thể kiểm chứng ngay tại chỗ. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: Với bài toán theo dõi hồ sơ thực tập của bạn Tú: "Khi các nền tảng tuyển dụng như TopCV, LinkedIn đều có form nộp riêng, sinh viên có thực sự cần lưu nhiều file rời rạc trên máy không hay pain lớn nhất là quên hạn nộp?". | Giúp bạn làm rõ phạm vi: sinh viên IT thường nộp CV kèm link GitHub/Portfolio và bài test riêng cho từng công ty, nên việc chuẩn hóa file nộp vẫn là pain thật. |
| Nhận phản biện | Câu hỏi tôi nhận được: "Nếu giảng viên đưa yêu cầu bằng tin nhắn Zalo vắn tắt hoặc chỉ nói miệng trên lớp thì công cụ lấy rubric ở đâu để kiểm tra?". | Tôi đã sửa: Bổ sung phương án fallback, cho phép sinh viên tự tick chọn các tiêu chí phổ thông (README, cấu trúc thư mục chuẩn) nếu không có file rubric PDF chính thức. |
| Gom cluster / cây OST | Cùng nhóm thảo luận gom các bài toán nộp bài lab, hồ sơ xin việc và đơn đặt hàng vào cụm "Chuẩn hóa và đối soát tài liệu theo yêu cầu bên ngoài". | Xây dựng được nhánh Opportunity rõ ràng: "Người nộp không nhớ hết các quy định hình thức phân tán ở nhiều văn bản". |
| Chọn candidate problem | Cùng chấm điểm 3 candidate theo 7 tiêu chí trong worksheet; bảo vệ quan điểm chọn bài toán có actor và quy trình đo lường được ngay. | Nhóm đạt đồng thuận cao khi chọn bài toán kiểm tra và chuẩn hóa tài liệu nộp/ứng tuyển. |
| Kiểm chứng / research | Phỏng vấn nhanh 3 bạn sinh viên trong lớp về trải nghiệm nộp bài lab; tìm kiếm các giải pháp linter và rubric checker hiện có trên GitHub. | Phát hiện ra hầu hết sinh viên đều từng bị trừ điểm hình thức ít nhất 1 lần; các công cụ hiện có quá phức tạp để cài đặt cho từng môn học. |
| Quy trình nhóm | Đóng góp xây dựng quy trình trước/sau; phân định rõ bước chạy script kiểm tra định dạng và bước con người xác nhận trước khi nộp. | Quy trình tương lai rõ ràng, tránh việc AI tự động nộp bài mà không có sự kiểm tra cuối cùng của sinh viên. |
| Problem Statement | Rà soát từng câu trong Problem Statement v0 để loại bỏ hoàn toàn các từ ngữ mang hàm ý giải pháp kỹ thuật (như "tự động hóa", "dùng AI"). | Bản Problem Statement v0 tập trung 100% vào nỗi đau của người dùng và các chỉ số đo lường cụ thể. |
| Mức can thiệp AI | Đề xuất giải pháp theo bậc thang: No AI / Rule cho kiểm tra file cứng; Workflow (kết hợp LLM) cho bước trích xuất tiêu chí từ văn bản rubric tự do. | Nhóm tránh được bẫy vội vàng làm Agent tự hành phức tạp khi bài toán chưa thực sự cần thiết. |
| Quyết định | Cùng phân tích ma trận 4 rủi ro (Value, Usability, Feasibility, Viability); đề xuất ngưỡng dừng (kill switch) nếu tỷ lệ trích xuất rubric sai quá 20%. | Đưa ra quyết định Go có điều kiện (Not Yet / Go với phạm vi pilot hẹp) kèm tiêu chí nghiệm thu rõ ràng. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Yêu cầu AI gợi ý các góc nhìn vấn đề trong môi trường học tập và làm việc IT theo 4 lăng kính. | Mở rộng góc nhìn sang các vấn đề giao tiếp nhóm và quản lý code cũ mà ban đầu tôi chưa nghĩ tới. | Gợi ý nhiều ý tưởng quá chung chung như "sinh viên bị mất tập trung khi học", không có actor và cách đo lường cụ thể. | Tự viết lại toàn bộ 8 bài toán theo chuẩn Job Story dựa trên chính trải nghiệm nộp bài và debug thực tế của mình. |
| CP2 Problem Card | Đóng vai một Product Manager hoài nghi để phản biện và chỉ ra điểm yếu trong Problem Card #1. | Cảnh báo rất chuẩn xác về việc LLM có thể bị ảo giác (hallucination) nếu để nó tự động phân tích và chấm điểm bài tập. | AI giả định rằng sinh viên luôn có rubric chuẩn dạng file text, bỏ qua thực tế rubric thường nằm rải rác trong slide hoặc tin nhắn. | Bổ sung phương án kiểm tra bằng Rule trước và thêm cơ chế fallback nhập checklist thủ công. |
| CP4 Research | Tra cứu các công cụ mã nguồn mở và pattern giải quyết bài toán kiểm tra quy cách file/code. | Liệt kê nhanh các từ khóa công nghệ liên quan như Git hooks, Markdown linter, GitHub Classroom autograder. | Trích dẫn một số tính năng của công cụ trả phí mà sinh viên không thể tiếp cận được trong phạm vi bài lab. | Lọc lại và chỉ giữ 2 giải pháp phù hợp: pre-commit hook đơn giản và checklist template dễ sử dụng. |
| CP5 Quy trình | Chuyển đổi mô tả các bước thành sơ đồ dạng text/ASCII và Mermaid. | Vẽ sơ đồ nhanh, định dạng trực quan, tiết kiệm thời gian căn chỉnh. | AI tự ý gộp bước "dò rubric" và "chạy lệnh test" làm một bước, làm mất đi bottleneck chính của quy trình. | Tách lại thành 2 bước độc lập kèm thời gian đo lường cụ thể cho từng bước nghẽn. |
| CP5–6 Problem Statement | Quét và phát hiện các từ khóa mang hơi hướng giải pháp (solution-first) trong bản thảo Problem Statement. | Phát hiện ra từ "tự động kiểm tra bằng công cụ" đang áp đặt giải pháp vào phần mô tả vấn đề. | Đôi khi sửa câu chữ trở nên quá học thuật, rườm rà và khó hiểu. | Giữ văn phong cô đọng, bám sát mẫu Lean UX với 6 trường thông tin rõ ràng. |
| CP6 Mức can thiệp / quyết định | Tham khảo góc nhìn về rủi ro Usability và Feasibility theo framework của Marty Cagan. | Cung cấp danh sách câu hỏi kiểm tra sắc bén về việc người dùng có chấp nhận sửa đổi quy trình quen thuộc hay không. | Thiên vị việc đề xuất xây dựng Agent đa tác vụ để giải quyết bài toán trọn gói. | Kiên quyết giữ kết luận ở mức Rule/Workflow, từ chối Agent vì bài toán có cấu trúc rõ và không đòi hỏi AI tự ra quyết định. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi lắng nghe phần trình bày top 3 problem cards của bạn Tú và các thành viên khác trong nhóm, điều lớn nhất tôi học được là sự đa dạng của góc nhìn thực tế và cách một vấn đề được nhận diện. Ban đầu, tôi có xu hướng chỉ nhìn quanh chiếc máy tính của mình: code lỗi, bài lab muộn, tài liệu kỹ thuật dài. Nhưng khi nghe bạn trình bày về nỗi đau của người thuê nhà khi báo thiết bị hỏng hay sự hỗn loạn của một cửa hàng nhỏ nhận đơn hàng qua tin nhắn mạng xã hội, tôi nhận ra rằng những quy trình phi cấu trúc trong đời sống thực tế tạo ra sự lãng phí thời gian khủng khiếp hơn rất nhiều. Bài học thứ hai là cách đặt câu hỏi về actor: nếu actor không phải là người chịu nỗi đau trực tiếp, giải pháp đưa ra sẽ không ai dùng. Việc nghe các bạn khác pitch giúp tôi nhận ra bài toán của mình cần phải làm rõ đối tượng thụ hưởng là sinh viên muốn bảo vệ điểm số hay là giảng viên muốn tiết kiệm thời gian chấm bài.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm tôi đã bị rơi vào cái bẫy "solution-first" ngay từ những phút đầu tiên khi bước vào CP3. Vừa mới chốt xong danh sách candidate, một bạn trong nhóm đã hào hứng đề xuất: "Hay là nhóm mình làm một con Chatbot Agent tích hợp vào Telegram, sinh viên chỉ cần quăng file zip vào là bot tự giải nén, tự chạy test rồi báo cáo điểm luôn!". Cả nhóm suýt nữa bị cuốn theo ý tưởng công nghệ hấp dẫn đó. Rất may mắn là nhờ quy tắc của cây OST và hướng dẫn trong worksheet, chúng tôi đã kịp dừng lại và tự hỏi: "Thực chất sinh viên đang đau ở bước nào? Họ đau vì không có bot hay đau vì không nhớ hết các quy định nộp bài nằm rải rác ở 3 file thông báo khác nhau?". Khi nhận ra mình đang cố nhét AI vào một bài toán mà có khi chỉ cần một file checklist Markdown là giải quyết được 80% vấn đề, nhóm đã chủ động gạch bỏ chữ "Chatbot" khỏi tầng Opportunity và quay trở lại phân tích đúng bước nghẽn thời gian.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã thực sự đổi ý một cách căn bản sau lượt phản biện từ nhóm đối với Card #1 của tôi. Ban đầu, trong bản nháp cá nhân, tôi rất tự tin rằng công cụ phải kiểm tra được cả việc code có chạy đúng test case của giảng viên hay không trước khi nộp. Tuy nhiên, khi tôi vừa pitch xong, một bạn trong nhóm đã đặt ngay câu hỏi phản biện: "Mỗi sinh viên dùng một hệ điều hành khác nhau, có bạn dùng Windows, có bạn dùng Mac, làm sao một script hay công cụ AI có thể đảm bảo chạy môi trường chuẩn xác 100% trên máy họ mà không gây xung đột dependency? Nếu tool báo xanh mà lên máy thầy bị đỏ thì ai chịu trách nhiệm?". Câu hỏi này đánh trúng vào điểm yếu chết người về Feasibility mà tôi đã chủ quan bỏ qua. Ngay sau đó, tôi đã lập tức thu hẹp phạm vi của bài toán: chỉ tập trung 100% vào việc kiểm tra tính tuân thủ quy cách hình thức (tên thư mục, tên file, định dạng báo cáo, sự tồn tại của file hướng dẫn) – nơi mà quy luật kiểm tra là bất biến và an toàn tuyệt đối.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi bất ngờ nhất khi thực hiện phỏng vấn nhanh 3 bạn sinh viên trong lớp là: lý do chính khiến các bạn bị trừ điểm nộp bài không phải vì các bạn không biết cách đặt tên file, mà là vì **thông báo yêu cầu nộp bài của giảng viên bị phân tán quá nhiều nơi**. Một bạn chia sẻ rằng thầy dặn cấu trúc thư mục trên slide bài giảng tuần 3, nhưng đến tuần 7 khi giao đề thì thầy lại dặn bổ sung thêm video demo trên Zalo, và đến sát ngày nộp trợ giảng lại đăng một thông báo khác trên Classroom yêu cầu đặt tên file ZIP theo cú pháp mới. Kết quả là sinh viên nhớ được quy định này thì quên mất quy định kia lúc nửa đêm sát deadline. Sự thật này làm tôi bất ngờ vì trước đó tôi nghĩ sinh viên chỉ đơn giản là ẩu đoảng. Phát hiện này củng cố thêm rằng việc tổng hợp và đối soát tiêu chuẩn từ các nguồn phân tán mới là giá trị cốt lõi cần giải quyết, chứ không đơn thuần là việc kiểm tra file.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó khăn nhất khi viết Problem Statement chính là việc **kìm nén ham muốn đưa giải pháp vào câu chữ**. Theo thói quen của dân kỹ thuật, mỗi khi nhìn thấy một vấn đề, phản xạ đầu tiên của tôi là lập tức nghĩ đến công nghệ: "cần xây dựng hệ thống", "cần áp dụng mô hình ngôn ngữ lớn để tự động hóa", "cần tạo web app". Khi viết bản v0, tôi liên tục bị sửa vì câu cú cứ vô thức xuất hiện chữ "tự động hóa bằng công cụ". Để diễn đạt được một Problem Statement chuẩn mực – chỉ thuần túy mô tả bối cảnh của Actor, quy trình hiện tại, con số đo lường bước nghẽn và hậu quả thực tế mà không hề nhắc tới bất kỳ công cụ nào – đòi hỏi sự kỷ luật tư duy rất cao. Ngoài ra, việc xác định một Boundary (ranh giới) rõ ràng để ngăn giải pháp phình to ra cũng là một thử thách không nhỏ.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu có cơ hội làm lại buổi lab từ đầu, tôi sẽ dành thêm thời gian ngay từ bước CP1 để đi tìm bằng chứng thực tế định lượng (chụp lại ảnh thông báo bị trừ điểm, bấm giờ chính xác 3 lần nộp bài) thay vì chỉ ước lượng số phút dựa trên trí nhớ. Còn trong quá trình làm việc nhóm, tôi sẽ phản biện nhóm mạnh mẽ hơn ở khâu xây dựng bảng chấm điểm shortlist tại CP3. Lúc chấm điểm, các thành viên đôi khi vẫn chấm theo cảm tính hoặc dựa vào việc ý tưởng đó nghe có vẻ "thời thượng" và "dùng nhiều AI" hay không, thay vì bám sát tiêu chí "Vừa sức một buổi lab" và "Độ hiểu sâu về domain". Lần tới, tôi sẽ yêu cầu mỗi thành viên khi cho điểm 4 hay 5 phải đưa ra được ít nhất một bằng chứng cụ thể chứng minh tại sao bài toán đó khả thi hơn bài toán khác.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm xuất phát từ việc sinh viên thường xuyên bị trừ điểm oan do sai sót quy cách và cấu trúc nộp bài khi thông tin rubric của giảng viên bị phân tán rải rác nhiều nơi. Quy trình hiện tại đòi hỏi người học phải lội qua nhiều thông báo, dò thủ công từng file và nén thư mục trong trạng thái căng thẳng sát giờ nộp, gây tắc nghẽn trung bình 18 phút mỗi lần. Chỉ số thành công được định nghĩa rõ ràng là giảm thời gian đối soát xuống dưới 5 phút và đưa tỷ lệ sai sót hình thức về mức 0% tuyệt đối. Ranh giới (boundary) bắt buộc là công cụ không được phép can thiệp hay sửa đổi nội dung code bên trong và tuyệt đối không tự ý submit bài thay cho sinh viên. Về mức can thiệp, nhóm lựa chọn giải pháp dạng Workflow: sử dụng Script/Rule cố định để kiểm tra tính hợp lệ của cây thư mục và chỉ dùng AI hỗ trợ đọc hiểu văn bản rubric tự do khi cần thiết. Cuối cùng, nhóm đưa ra quyết định Go có điều kiện cho một bản thử nghiệm nội bộ nhỏ, kèm ngưỡng dừng rõ ràng nếu hệ thống gây thêm phiền toái hoặc trích xuất sai lệch yêu cầu của giảng viên.

---

## 7. Tài liệu tham khảo

- Teresa Torres, *Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value*, 2021.
- Rob Fitzpatrick, *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*, 2013.
- Jeff Gothelf & Josh Seiden, *Lean UX: Designing Great Products with Agile Teams*, O'Reilly Media.
- Google People + AI Research (PAIR), *People + AI Guidebook*, https://pair.withgoogle.com/.
- Anthropic, *Building Effective Agents*, 2024, https://www.anthropic.com/research/building-effective-agents.
- Marty Cagan, *Inspired: How to Create Tech Products Customers Love*, Silicon Valley Product Group, 2017.

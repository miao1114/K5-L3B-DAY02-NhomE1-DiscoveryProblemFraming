# Báo cáo nhóm — Day 02 Discovery & Problem Framing

## 1. Thông tin nhóm

- Tên nhóm: Nhóm E1
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Sinh viên mất thời gian tìm lại đúng phần giải thích kiến thức trong video bài giảng dài, nhất là khi công thức chỉ xuất hiện trên bảng/slide và transcript không chứa đầy đủ nội dung.
- Quyết định cuối: **Not Yet** — kiểm chứng nhu cầu và khả năng tìm đúng đoạn trước khi xây dựng giải pháp AI.

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Nhóm 4 người, 12 candidate. Thời gian là ước lượng từ CP2.

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Phản biện nhận được (người góp ý) |
|---:|---|---|---|---|---|
| 1 | Nguyễn Đức Minh — Card #1 | Khi chấm bài toán viết tay, tôi muốn xác định bước sai đầu tiên và loại lỗi, để hướng dẫn học sinh sửa đúng nguyên nhân. | Giáo viên Toán THCS | Kiểm tra từng phép biến đổi, tìm bước sai và phân loại lỗi: 2/5 phút/bài. | Nhóm: có ích nhưng lo chi phí xây dựng/huấn luyện và vận hành AI. |
| 2 | Nguyễn Đức Minh — Card #2 | Khi làm bài tập từ video 90 phút, tôi muốn tìm đúng đoạn giải thích công thức, để tiếp tục làm bài mà không phải tua nhiều đoạn. | Sinh viên học qua video | Tua và quan sát bảng/slide khi transcript không đủ: 4/7 phút/lần tìm. | Nhóm cân nhắc cùng Card #3 của Minh và cuối cùng chọn card này. |
| 3 | Nguyễn Đức Minh — Card #3 | Khi nhận đơn bán sỉ qua tin nhắn, ảnh và ghi âm, tôi muốn xác định đúng mã hàng, số lượng và đơn vị, để nhập đơn và tránh giao nhầm. | Nhân viên nhập đơn nhà phân phối thực phẩm | Tra SKU, đơn vị và lịch sử: 1,5/4 phút thao tác/đơn; chưa tính chờ xác nhận. | Nhóm cân nhắc cùng Card #2 của Minh trước khi chốt. |
| 4 | Phạm Thế Hùng — Card #1 | Khi đánh giá CV, tôi muốn biết kinh nghiệm và kỹ năng đáp ứng tiêu chí nào trong mô tả công việc, để chọn hồ sơ phù hợp. | Chuyên viên tuyển dụng | Đối chiếu từng tiêu chí: 1,1/2 phút/CV. | Nhóm: TopCV đã giải quyết bài toán tương tự; cần kiểm tra phạm vi ở CP4. |
| 5 | Phạm Thế Hùng — Card #2 | Khi tài liệu nằm ở nhóm chat, email và hệ thống học tập, tôi muốn tìm đúng tài liệu, để bắt đầu làm bài kịp thời. | Sinh viên | Tìm từ khóa, đọc tin và mở liên kết qua nhiều kênh: 4/8 phút/lần. | Phản biện tham khảo: thư mục chung và danh mục liên kết đã đủ chưa? Làm sao bảo đảm đúng phiên bản và quyền truy cập? Chưa có căn cứ cần Agent. |
| 6 | Phạm Thế Hùng — Card #3 | Khi có danh sách căn hộ, tôi muốn biết từng căn đáp ứng yêu cầu nào của khách, để chọn phương án phù hợp ngân sách và nhu cầu. | Nhân viên môi giới căn hộ | Đối chiếu 6 căn theo 5 tiêu chí: 6/12 phút/yêu cầu. | Phản biện tham khảo: bộ lọc Sheets theo 5 tiêu chí đã đủ chưa? Giá và tình trạng giao dịch có được cập nhật không? Cần tách tiêu chí bắt buộc với ưu tiên. |
| 7 | Trương Thị Thu Hà — Card #1 | Khi notebook báo lỗi, tôi muốn xác định dòng lỗi và nguyên nhân, để sửa nhanh thay vì thử nhiều lần. | Học viên AI20K làm lab Python/notebook | Xác định nguyên nhân và tìm hướng xử lý ở bước 2–3: 55/90 phút/lần. | Nhóm: chatbot AI hiện có có thể hỗ trợ tốt, chưa thấy lý do tự xây AI mới. |
| 8 | Trương Thị Thu Hà — Card #2 | Khi nhận đề lab, tôi muốn xác định đủ yêu cầu và thứ tự thực hiện, để không bỏ sót tiêu chí. | Học viên AI20K | Đọc và tổng hợp yêu cầu nằm ở nhiều file, bước 2–3: 35/50 phút/đề. | Nhóm: chatbot AI hiện có có thể hỗ trợ tốt, chưa thấy lý do tự xây AI mới. |
| 9 | Trương Thị Thu Hà — Card #3 | Khi nộp bài lab, tôi muốn xác định đúng tên repo và file, để tránh sai quy định nộp bài. | Học viên AI20K; coach | Xác minh cách đặt tên giữa các nguồn ở bước 3: khoảng 15 phút. | Nhóm: chatbot AI hiện có có thể hỗ trợ tốt, chưa thấy lý do tự xây AI mới. |
| 10 | Đào Thị Ngọc Ánh — Card #1 | Khi bệnh nhân thanh toán, tôi muốn có đủ dịch vụ đã dùng và phần bảo hiểm chi trả, để xuất hóa đơn nhanh và đúng. | Nhân viên thanh toán viện phí | Gom dịch vụ, đối chiếu và kiểm tra điều kiện bảo hiểm ở bước 2–4: 8/12 phút/hồ sơ. | Nhóm: AI chỉ hỗ trợ một phần; con người vẫn phải xác nhận do dữ liệu và thanh toán nhạy cảm. |
| 11 | Đào Thị Ngọc Ánh — Card #2 | Khi nhận nhiều hóa đơn cuối tháng, tôi muốn có đủ trường dữ liệu trong phần mềm kế toán, để chốt sổ đúng hạn mà không gõ lại từng dòng. | Kế toán viên doanh nghiệp vừa và nhỏ | Đọc và gõ tay từng trường: khoảng 3 phút/hóa đơn. | Nhóm: đã có công cụ chuyển dữ liệu hóa đơn vào phần mềm; cần kiểm tra phạm vi ở CP4. |
| 12 | Đào Thị Ngọc Ánh — Card #3 | Khi nhận yêu cầu xác minh tốt nghiệp, tôi muốn tìm hồ sơ đầy đủ, để trả lời đúng hạn mà không lục nhiều nguồn. | Chuyên viên Phòng Đào tạo/Công tác sinh viên | Tìm Excel, sổ gốc và đối chiếu định dạng ở bước 3–5: 20–60 phút/yêu cầu khóa cũ. | Nhóm: trọng tâm là lưu trữ, chuẩn hóa và truy xuất cơ sở dữ liệu. |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Tìm lại thông tin đã có | #2 Tìm đoạn kiến thức trong video; #5 Tìm tài liệu học tập; #12 Tra cứu hồ sơ tốt nghiệp | Biết thông tin đã tồn tại nhưng khó tìm đúng vị trí hoặc bản ghi vì nội dung dài, phân tán hoặc thiếu chỉ mục thống nhất. |
| B — Hiểu nội dung và xác định điểm vướng | #1 Tìm bước giải sai; #7 Debug notebook; #8 Đọc hiểu đề lab | Phải đọc nội dung, hiểu ngữ cảnh và xác định lỗi hoặc yêu cầu trước khi có thể tiếp tục công việc. |
| C — Chuẩn hóa và đối chiếu dữ liệu | #3 Chuẩn hóa đơn bán sỉ; #4 Đối chiếu CV; #6 Đối chiếu căn hộ; #10 Thanh toán viện phí; #11 Nhập hóa đơn | Chuyển thông tin nhiều định dạng thành trường/tiêu chí rõ rồi kiểm tra với danh mục, yêu cầu hoặc hồ sơ liên quan. |
| D — Kiểm tra quy định trước khi nộp | #9 Đặt tên repo và file | Phải xác minh và áp dụng đúng quy tắc để tránh sai sót khi nộp bài; có khả năng giải bằng checklist hoặc kiểm tra theo rule. |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm thời gian sinh viên tìm lại kiến thức trong video bài giảng dài,
         đồng thời tìm đúng phần giải thích cần xem.
├── Opportunity: Không nhớ mốc thời gian nên phải tua và xem nhiều đoạn.
├── Opportunity: Công thức trên bảng/slide không có đầy đủ trong transcript.
└── Opportunity: Công thức xuất hiện nhiều lần, khó tìm đúng phần giải thích.
     ✗ "Chatbot hỏi đáp video"       ← solution, gạch khỏi tầng này
     ✗ "Tự động tạo mục lục video"   ← solution, gạch khỏi tầng này
```

### 2.4. Chấm điểm shortlist (1–5)

Điểm tham khảo dựa trên CP2, có hỗ trợ AI, tối đa 35 điểm. Bằng chứng pain còn hạn chế vì chưa đo thời gian thực tế.

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Tìm kiến thức trong video — Minh, Card #2 | 5 | 5 | 2 | 4 | 4 | 5 | 4 | **29** |
| Xử lý hóa đơn — Ngọc Ánh, Card #2 | 5 | 5 | 2 | 4 | 4 | 4 | 2 | **26** |
| Đọc tin khóa học, tìm tài liệu — Hùng, Card #2 | 5 | 4 | 2 | 4 | 4 | 4 | 4 | **27** |

**Chọn:** Tìm lại đoạn kiến thức trong video bài giảng dài — Card #2 của Nguyễn Đức Minh.

**Vì sao chọn:** Actor rõ, phạm vi giới hạn trong một video 90 phút; đo được thời gian tìm và độ đúng của đoạn trả về. Có thể so sánh tìm thủ công, mục lục/bookmark và tìm kiếm có AI.

**Vì sao chưa chọn hai candidate còn lại:** Xử lý hóa đơn có quy trình nhiều bước, đòi hỏi kiến thức chuyên sâu về kế toán mà nhóm chưa đáp ứng đủ. Đọc tin khóa học để tìm tài liệu phải gom thông tin nhiều kênh, có thể cải thiện trước bằng danh mục liên kết, thư mục chung và quy tắc phiên bản.

**Bất đồng:** Ban đầu có ý kiến muốn chọn xử lý hóa đơn. Sau khi thảo luận, nhóm nhận thấy quy trình nhiều bước và cần kiến thức chuyên sâu về kế toán nên thống nhất không chọn, chuyển sang tìm lại đoạn kiến thức trong video bài giảng dài.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách kiểm chứng:

Interview snapshot:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

**Bài toán:** Khi làm bài tập từ một video bài giảng Toán dài 90 phút, sinh viên cần tìm lại đúng đoạn có công thức và phần giải thích liên quan để tiếp tục làm bài.

**Phạm vi:** Một video có transcript nhưng chưa có mục lục chi tiết, người học có quyền sử dụng; công thức có thể chỉ xuất hiện trên bảng/slide và không được đọc đầy đủ. Quy trình bắt đầu khi người học xác định nhu cầu tìm lại kiến thức và kết thúc khi đã xác nhận đúng đoạn, lưu mốc rồi quay lại bài tập.

### 4.1. Quy trình hiện tại

![Quy trình As-Is: tìm transcript, tua video nếu chưa tìm thấy, xác nhận đoạn và ghi mốc; có vòng lặp khi đoạn chưa đúng](../assets/cp5-workflow-current.png)

| Bước | Actor | Input | Output | Thời gian phân bổ / lần tìm | Ghi chú |
|---:|---|---|---|---|---|
| 1. Xác định nội dung cần tìm | Sinh viên | Bài tập đang làm; công thức hoặc nội dung nhớ được | Từ khóa, công thức hoặc mô tả cần tìm | 30 giây | Xác định cả phần giải thích cần xem, không chỉ hình công thức. |
| 2. Tìm từ khóa trong transcript | Sinh viên | Mô tả từ bước 1; transcript của video | Mốc nghi ngờ hoặc xác định chưa tìm thấy đoạn phù hợp | 1 phút | Có mốc phù hợp thì sang bước 4; không tìm ra hoặc chỉ thấy từ khóa thiếu ngữ cảnh thì sang bước 3. |
| 3. Tua video, quan sát bảng/slide | Sinh viên | Video; công thức cần tìm; các mốc đã kiểm tra | Đoạn nghi ngờ có công thức và phần giải thích | 4 phút | **Bottleneck phân tích.** Phải mở và quan sát nhiều mốc khi transcript không chứa đủ nội dung trên hình. |
| 4. Xem và xác nhận đoạn giải thích | Sinh viên | Đoạn nghi ngờ từ bước 2 hoặc 3 | Xác nhận đúng công thức và đúng phần giải thích; hoặc xác định chưa đúng | 1 phút | Đúng thì sang bước 5; chưa đúng thì quay lại bước 3. Chỉ thấy công thức chưa được tính là tìm thành công. |
| 5. Ghi mốc và quay lại bài tập | Sinh viên | Đoạn đã xác nhận; mốc bắt đầu–kết thúc | Bookmark/ghi chú có mốc thời gian; tiếp tục làm bài | 30 giây | Cùng một sinh viên thực hiện cả 5 bước, không có chuyển giao giữa người. |

**Tổng thời gian phân bổ:** 30 giây + 1 phút + 4 phút + 1 phút + 30 giây = **7 phút/lần tìm**, cho luồng đi qua bước tua video và xác nhận đúng sau một lượt.

**Bottleneck chính:** Bước 3 — tua video và quan sát bảng/slide. Khi công thức trên hình không được đọc đầy đủ, tìm từ khóa trong transcript không đủ để định vị; người học phải mở và kiểm tra nhiều mốc trước khi đến được phần giải thích cần xem.

**Cách đọc sơ đồ:** Nếu tìm được ngay bằng transcript thì bỏ qua bước 3; nếu đoạn chưa đúng thì quay lại bước 3. Các lượt phải lặp lại hoặc không tìm được được ghi riêng khi theo dõi quy trình.

### 4.2. Quy trình tương lai

**Phương án đề xuất:** Workflow có AI hỗ trợ tìm đoạn; người học vẫn xác nhận kết quả. Đây là bản đề xuất CP5 để nhóm so sánh với No AI/Rule và chốt mức can thiệp tại CP6.

![Quy trình To-Be: chuẩn bị chỉ mục một lần, người học nhập yêu cầu, AI và Rule trả đoạn có căn cứ, người học kiểm tra; lỗi hoặc kết quả sai thì quay về As-Is](../assets/cp5-workflow-future.png)

**Chuẩn bị một lần, ngoài thời gian mỗi lượt tìm:** Người phụ trách học liệu cung cấp video và transcript được phép sử dụng; hệ thống đối chiếu transcript với khung hình bảng/slide để lập chỉ mục theo thời gian. Người phụ trách học liệu kiểm tra mẫu mốc thời gian và căn cứ; có lỗi thì sửa trước khi dùng. Khi đổi video/transcript, cập nhật và kiểm tra lại chỉ mục. Ghi riêng thời gian, chi phí và công sức chuẩn bị khi thử nghiệm.

| Bước | Actor / loại xử lý | Input | Output | Thời gian mục tiêu / lần tìm | Ghi chú |
|---:|---|---|---|---|---|
| 1. Nhập công thức hoặc mô tả | **Con người:** sinh viên | Bài tập; công thức hoặc mô tả phần giải thích cần xem | Yêu cầu tìm trong video đã lập chỉ mục | 30 giây (0,5 phút) | Có thể dùng mô tả khi không nhớ chính xác cách viết công thức. |
| 2. Tìm và hiển thị đoạn có căn cứ | **AI + Rule:** hệ thống | Yêu cầu; chỉ mục transcript và hình bảng/slide | Tối đa 3 đoạn, mỗi đoạn có mốc bắt đầu–kết thúc, liên kết mở video và khung hình liên quan; hoặc báo chưa tìm thấy | 15 giây (0,25 phút), gồm thời gian chờ hệ thống | AI đối chiếu nội dung; Rule kiểm tra mốc trong phạm vi video, tạo liên kết và giới hạn số kết quả. Có kết quả hợp lệ thì sang bước 3; không có căn cứ hoặc hệ thống lỗi thì quay về As-Is. |
| 3. Mở và xác nhận phần giải thích | **Con người:** sinh viên | Các đoạn và căn cứ từ bước 2 | Xác nhận có đúng công thức và phần giải thích cần tìm; hoặc bác bỏ kết quả | 60 giây (1 phút), ngân sách cho việc mở và kiểm tra các kết quả | Chỉ chấp nhận sau khi xem nguồn video. Nếu mọi kết quả đều sai, thiếu ngữ cảnh hoặc không mở được thì quay về As-Is. |
| 4. Lưu mốc và tiếp tục bài tập | **Con người:** sinh viên | Đoạn đã được xác nhận | Bookmark/ghi chú có mốc thời gian; quay lại bài tập | 15 giây (0,25 phút) | Người học quyết định có sử dụng đoạn đó. |

**Tổng thời gian mục tiêu:** 30 + 15 + 60 + 15 = **120 giây = 2 phút/lần tìm thành công**. Thời gian tìm và xác nhận đúng đoạn ở bước 1–3 nằm trong ngân sách 105 giây; 15 giây còn lại dành cho lưu mốc và quay lại bài. Nếu kiểm tra lâu hơn thì ghi thời gian thực tế, không cắt ngắn việc kiểm tra để đạt mục tiêu.

**Boundary:**

- Chỉ xử lý video/transcript được cung cấp và được phép sử dụng; không tìm sang nguồn khác ngoài phạm vi đã thống nhất.
- Không tự tạo công thức, mốc thời gian, căn cứ hoặc phần giải thích thay cho nội dung gốc. Không có căn cứ trong video thì báo **chưa tìm thấy**.
- Kết quả là gợi ý đoạn để mở xem; AI không tự xác nhận người học đã tìm đúng hoặc hiểu đúng kiến thức. Người học kiểm tra video trước khi sử dụng; người phụ trách học liệu kiểm tra chỉ mục trước khi đưa vào dùng.

**Phương án quay về:**

| Tình huống | Xử lý | Người thực hiện |
|---|---|---|
| Chưa có chỉ mục, chỉ mục lỗi, không có kết quả có căn cứ hoặc hệ thống ngừng hoạt động | Báo rõ chưa tìm thấy/lỗi; quay lại bước 2 của As-Is để tìm transcript, sau đó tua video nếu cần | Sinh viên; người phụ trách học liệu xử lý chỉ mục riêng |
| Mọi kết quả được trả về (tối đa 3) đều sai, thiếu phần giải thích hoặc mốc/liên kết không dùng được | Bỏ kết quả gợi ý; quay lại bước 2–3 của As-Is, xem và xác nhận trước khi lưu mốc | Sinh viên |
| Đã tìm được mốc hữu ích nhưng phần giải thích chưa đủ | Dùng mốc đó làm điểm bắt đầu để tua quanh đoạn, tiếp tục bước 3–4 của As-Is | Sinh viên |

Lượt phải quay về được ghi là **lượt dùng phương án thủ công**; đo tổng thời gian từ lúc bắt đầu tìm, gồm cả thời gian thử Workflow và tìm lại, tránh chỉ báo cáo những lượt thành công nhanh.

### 4.3. Before / after

| Chỉ số | Trước — phân bổ thời gian | Sau — mục tiêu | Ghi chú / cách kiểm soát |
|---|---|---|---|
| Số bước trên luồng tìm thành công | 5, khi phải tua video | 4 | Đếm theo các bước đánh số trên sơ đồ, không tính nút rẽ nhánh hoặc công chuẩn bị một lần. Luồng transcript tìm được ngay có 4 bước; lượt lặp/quay về ghi riêng. |
| Tổng thời gian/lần tìm | 7 phút | Không quá 2 phút, gồm mở và kiểm tra đoạn, lưu mốc, quay lại bài tập | Khi kiểm tra, bấm giờ từ lúc bắt đầu tìm đến khi lưu được đoạn đúng và quay lại bài tập, tính cả thời gian chờ và tìm lại. Nếu transcript tìm được ngay thì bỏ thời gian tua video. |
| Số bước thủ công | 5/5 | 3/4 | Nhập yêu cầu, kiểm tra và lưu mốc vẫn do người học thực hiện. Nếu quay về As-Is thì ghi thêm thao tác thực tế. |
| Bottleneck chính | Tua video và quan sát bảng/slide | Người học kiểm tra đoạn: mục tiêu 1 phút | Giữ bước kiểm tra để tránh nhận nhầm công thức hoặc thiếu ngữ cảnh. |
| Rủi ro tìm sai hoặc thiếu phần giải thích | Người học có thể bỏ sót đoạn khi tua | AI có thể gợi ý sai đoạn hoặc chỉ tìm thấy hình công thức | Hiển thị khung hình và mốc thời gian; người học mở video để xác nhận cả phần giải thích. |
| Rủi ro mới phát sinh | Chưa phụ thuộc chỉ mục hoặc hệ thống tìm đoạn | Nhận dạng sai công thức, mốc thời gian sai, chỉ mục cũ hoặc hệ thống lỗi | Kiểm tra mẫu chỉ mục; Rule kiểm tra mốc; cập nhật khi đổi học liệu; luôn có đường quay về As-Is. |
| Công chuẩn bị một lần | Mở video và transcript; chuẩn bị ghi chú hoặc bookmark để lưu mốc | Cung cấp video/transcript; lập chỉ mục transcript kết hợp hình bảng/slide; kiểm tra mẫu mốc thời gian và cập nhật khi đổi học liệu | Ghi riêng thời gian và chi phí chuẩn bị/cập nhật, không tính bằng 0 và không gộp vào 2 phút/lần tìm. |
| Xử lý khi tìm chưa đúng | Tiếp tục tua và quan sát bảng/slide; lặp bước tìm đoạn và xác nhận cho đến khi tìm đúng hoặc dừng tìm | Quay về tìm transcript và tua thủ công khi không có kết quả có căn cứ, mọi đoạn gợi ý đều sai, liên kết lỗi hoặc hệ thống ngừng hoạt động | Nếu có mốc hữu ích thì tua quanh mốc đó. Ghi số lượt, lý do và tổng thời gian gồm cả thử Workflow lẫn thao tác thủ công. |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Cao** | Chưa có phỏng vấn hay quan sát trực tiếp trong CP4; 7 phút/lần và 6 lần/tháng vẫn là giả định. Chưa chứng minh tìm kiếm có AI mang lại lợi ích hơn mục lục, bookmark và tìm transcript. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **TB** | Chưa thử với người học. Kết quả có thể trỏ tới nơi chỉ xuất hiện công thức, thiếu phần giải thích; người học phải mở nhiều đoạn để xác nhận. Cần mốc thời gian, khung hình và nguồn video để kiểm tra, cùng cách báo chưa tìm thấy. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Cao** | Chưa có mẫu thử chứng minh khả năng ghép nội dung bảng/slide với transcript và mốc thời gian. [EduVidQA](https://aclanthology.org/2025.emnlp-main.1760/) đánh giá 6 mô hình đa phương thức trên 5.252 cặp hỏi–đáp từ 296 video khoa học máy tính và chỉ ra tính thách thức của tác vụ. Đây là tín hiệu rủi ro, chưa phải kết quả đánh giá bài toán tìm đoạn video của nhóm. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **TB** | Chưa đo chi phí xử lý/lập chỉ mục mỗi video, số lượt tìm để bù chi phí và công sức cập nhật. Cần video được phép sử dụng, xác định dữ liệu được gửi cho công cụ bên ngoài và người phụ trách vận hành. |

### 8.2. Kết luận

**Quyết định:** **Not Yet**.

**Lý do:**

Value và Feasibility còn ở mức Cao, trong khi CP4–CP5 chưa có kết quả kiểm chứng và baseline đo thật. EduVidQA nghiên cứu tạo câu trả lời dài dựa trên video, rộng hơn phạm vi tìm đúng đoạn của nhóm; việc đã có nghiên cứu và tác vụ khó chưa đủ để kết luận No-Go. Nhóm tạm dừng xây sản phẩm, chỉ thực hiện kiểm chứng phạm vi nhỏ bằng công cụ sẵn có, chưa tự huấn luyện mô hình.

**Bước tiếp theo — trong 1 tuần:**

1. Phỏng vấn và quan sát 3 sinh viên ngoài nhóm từng tìm lại kiến thức trong video; ghi lần gần nhất, tần suất, thời gian và cách xử lý hiện tại.
2. Chọn một video 90 phút được phép sử dụng, có transcript và bảng/slide rõ. Chuẩn bị 20 yêu cầu tìm kiếm có đoạn tham chiếu do người xem xác nhận, gồm cả nội dung chỉ có trên hình.
3. So sánh tìm thủ công, dùng mục lục/bookmark và mẫu thử tìm kiếm có AI trên các nhiệm vụ tương đương; tính đến lúc người học xác nhận đúng phần giải thích. Ghi riêng thời gian lập chỉ mục, chi phí và số kết quả sai; không dùng câu hỏi đánh giá để điều chỉnh mẫu thử.
4. Rà soát lại 4 rủi ro. Chỉ cân nhắc Go cho pilot nhỏ nếu không còn rủi ro Cao và đạt các ngưỡng đề xuất dưới đây.

**Ngưỡng dừng đề xuất:** Sau 1 tuần, dừng hướng AI nếu dưới 2/3 người được hỏi có nhu cầu lặp lại ít nhất hằng tuần; hoặc mẫu thử tìm đúng dưới 18/20 yêu cầu trong 3 kết quả đầu; hoặc thời gian tìm trung vị vượt 2 phút/lần; hoặc không giảm ít nhất 30% thời gian so với mục lục/bookmark. Các ngưỡng là tiêu chí cho thử nghiệm, chưa phải kết quả đã đạt.

**Phương án quay về:** Dùng mục lục theo thời gian, danh mục công thức và bookmark. Nếu cách này đã đủ đáp ứng nhu cầu, hoặc thử nghiệm không đạt ngưỡng và nhóm không có cách giảm rủi ro trong nguồn lực hiện có, chuyển **No-Go đối với hướng xây giải pháp AI**.

---

## 9. Hạn chế và hướng tiếp theo

- Chưa có dữ liệu phỏng vấn, baseline đo thực tế và kết quả thử nghiệm; chưa xác nhận lợi ích so với mục lục/bookmark.
- EduVidQA cung cấp bằng chứng về độ khó của hỏi–đáp video, chưa chứng minh độ chính xác tìm đoạn trên video Toán của nhóm. Tiếp tục kiểm chứng phạm vi nhỏ theo mục 8.2.

## 10. Tài liệu tham khảo

- Ray, S. và cộng sự (2025). [EduVidQA: Generating and Evaluating Long-form Answers to Student Questions based on Lecture Videos](https://aclanthology.org/2025.emnlp-main.1760/). EMNLP 2025. Tham khảo cho đánh giá rủi ro kỹ thuật tại mục 8.1.

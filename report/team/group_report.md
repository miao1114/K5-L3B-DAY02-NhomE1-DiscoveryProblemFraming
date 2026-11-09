# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

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

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

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


Quy trình hiện tại của sinh viên (để đối chiếu cột "Giải bước nào"): **1** Mở lại video 90' → **2** Nhớ mơ hồ nội dung cần tìm → **3** Tìm từ khóa trong transcript → **4** Không ra (công thức chỉ có trên bảng/slide) → tua và quan sát từng đoạn → **5** Xem lại đoạn tìm được, làm bài tập.

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Panopto Smart Search (nền tảng video bài giảng) | https://www.panopto.com/features/video-search/ | Bước 3–4: index cả lời nói (ASR), chữ trên màn hình (OCR) và nội dung slide; bấm kết quả để nhảy tới đúng thời điểm | Giải đúng ca "công thức chỉ xuất hiện trên màn hình" mà **không cần AI tạo sinh**; đã có sẵn ở nhiều trường | Chỉ tìm theo **từ khóa**, không hiểu câu hỏi kiểu "đoạn thầy chứng minh đạo hàm"; công thức toán viết tay khó OCR; trường phải trả phí nền tảng | **Mức Rule (OCR + keyword) giải được một phần lớn bài toán.** Phải kiểm chứng xem sinh viên có tìm được bằng keyword không trước khi chọn AI |
| Google NotebookLM (thêm nguồn là link YouTube) | https://blog.google/innovation-and-ai/products/notebooklm-audio-video-sources/ | Bước 3: hỏi đáp trên transcript, câu trả lời có trích dẫn tới transcript của video | Miễn phí, hỏi bằng ngôn ngữ tự nhiên, có trích dẫn nguồn | Bài viết chỉ nói trích dẫn "linked directly to the video's transcript", không nói phân tích hình ảnh; chỉ nhận video YouTube công khai. Với ca P4 (công thức không được đọc thành lời) thì **khả năng cao vẫn không tìm ra** | Công cụ chỉ dựa transcript **không giải được bottleneck** của nhóm. Bottleneck nằm ở phần hình ảnh |
| Gemini API: video understanding | https://aistudio.google.com/docs/video-understanding | Bước 3–4: xử lý cả âm thanh và hình ảnh của video, trả lời và tham chiếu mốc thời gian dạng MM:SS | Nhận link YouTube công khai trực tiếp, không phải tự xây pipeline; dùng được ngay để chạy thử (pilot) | Mặc định lấy mẫu **1 khung hình/giây** nên có thể sót chi tiết; gói miễn phí giới hạn 8 giờ video YouTube/ngày; chỉ nhận video công khai, không nhận private/unlisted | Dùng được để **kiểm chứng nhanh** giả định "AI tìm được đoạn chỉ có trên bảng" mà không phải xây gì |
| Nghiên cứu EduVidQA (EMNLP 2025) | https://aclanthology.org/2025.emnlp-main.1760 | Bước 3–5: trả lời câu hỏi của sinh viên dựa trên video bài giảng | Bộ dữ liệu 5.252 cặp hỏi đáp từ 296 video khoa học máy tính; có khảo sát sinh viên muốn câu trả lời thế nào | Tác giả đánh giá đây là bài toán **còn khó** với các mô hình đa phương thức hiện tại | Không nên để AI **tự trả lời/giải thích** nội dung; chỉ nên để AI **chỉ ra đúng đoạn video**, sinh viên tự xem lời giảng gốc |

**Kết luận research:**

```text
Bước "tìm theo chữ trên màn hình" đã có giải pháp Rule (Panopto: OCR + keyword).
Công cụ chỉ dựa transcript (NotebookLM) không giải được ca công thức chỉ có trên bảng.
Mô hình đa phương thức (Gemini) xem được hình ảnh nhưng hỏi đáp tự do vẫn là bài toán khó (EduVidQA).
→ Không tự xây agent. Hướng hợp lý: Workflow cố định — index transcript + khung hình/OCR,
  AI chỉ trả về mốc thời gian + khung hình, sinh viên tự xem đoạn gốc.
→ Cần kiểm chứng trước: sinh viên có tìm được bằng keyword OCR (mức Rule) hay không.
```

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

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

Bài của nhóm nằm ở ô: **Độ mơ hồ cao × Độ phức tạp trung bình** → Workflow có AI ở 1–2 bước.

Vì sao:

- **Mơ hồ cao:** sinh viên hỏi bằng ngôn ngữ tự nhiên và chỉ nhớ mơ hồ ("đoạn thầy chứng minh công thức đạo hàm"), không có từ khóa chính xác. Nội dung cần tìm nằm trong **hình ảnh** (công thức viết trên bảng, slide), không có trong transcript. Không viết được luật cố định để khớp kiểu câu hỏi này.
- **Phức tạp trung bình:** dữ liệu đa phương thức (âm thanh + hình ảnh) nhưng các bước **cố định, không rẽ nhánh**: lập chỉ mục video một lần → nhận câu hỏi → trả về mốc thời gian. AI không cần tự quyết bước tiếp theo.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Giảng viên/trợ giảng chia chương (chapters) có tiêu đề cho video; đăng kèm slide/ảnh bảng viết; sinh viên ghi chú mốc thời gian khi xem | Video ngắn, ít, giảng viên có thời gian chia chương | Tốn công giảng viên cho mỗi video; chương quá thô, không tìm được tới từng công thức | Dùng làm **phương án quay về** |
| **Rule** | Index transcript (ASR) + chữ trên màn hình (OCR) + slide, tìm theo từ khóa và nhảy tới mốc thời gian (như Panopto Smart Search) | Sinh viên nhớ đúng từ khóa và công thức là chữ in rõ (slide) | Không hiểu câu hỏi tự nhiên; OCR công thức viết tay kém; tìm sai nếu sinh viên dùng từ khác giảng viên | **Dùng cho bước lập chỉ mục** (OCR/slide). Cần kiểm chứng có đủ dùng không **[chờ CP4]** |
| **Workflow** | Bước cố định: (1) Rule: index transcript + OCR + slide theo thời gian → (2) AI: tạo mô tả ngắn cho từng đoạn/khung hình (kể cả công thức viết tay) → (3) AI: so khớp câu hỏi của sinh viên, trả **top 3 mốc thời gian + ảnh khung hình** → (4) Sinh viên bấm xem đoạn gốc | Câu hỏi diễn đạt tự nhiên, nội dung chỉ có trên hình ảnh | Trả sai mốc thời gian; mô tả công thức sai; chi phí xử lý video | **Chọn** |
| **Agent** | AI tự xem video, tự quyết tìm thêm tài liệu, tự giải thích và tự trả lời bài tập cho sinh viên | Khi bước tiếp theo không đoán trước được | Giải thích sai kiến thức (EduVidQA cho thấy bài toán còn khó); sinh viên dựa vào AI thay vì xem lời giảng; khó kiểm soát | Không chọn |

**Mức chọn:** Workflow (Rule ở bước lập chỉ mục, AI ở bước mô tả khung hình và so khớp câu hỏi).

**Vì sao không chọn mức đơn giản hơn:**

- **No AI** đòi giảng viên chia chương cho từng video và vẫn không đi tới mức từng công thức.
- **Rule** (OCR + keyword) giải được ca công thức in trên slide, nhưng không giải được hai ca chính của P4: (1) sinh viên **không nhớ từ khóa**, chỉ nhớ ý; (2) công thức **viết tay trên bảng**. Đây là lập luận dựa trên research. **[chờ CP4]** Cần kết quả phỏng vấn: bao nhiêu sinh viên đã thử tìm bằng từ khóa mà không ra. Nếu đa số tìm được bằng từ khóa, nhóm nên hạ xuống mức Rule.

**Ghi chú chi phí (đầu vào cho mục 8, dòng Viability):**

- Ước tính theo bậc độ lớn với Gemini Flash (giá trên các trang tổng hợp: khoảng 0,25–1,5 USD/1 triệu token đầu vào, **cần đối chiếu trang giá chính thức của Google**): video 90 phút ≈ 1,6 triệu token → **≈ 0,4–2,4 USD để lập chỉ mục 1 video, chạy 1 lần**. Một môn 15 buổi ≈ 6–36 USD, chia 150 sinh viên ≈ 1.000–6.000đ/sinh viên/môn. Trả lời câu hỏi trên chỉ mục: khoảng vài USD/tháng.
- Chi phí chỉ thấp khi **index một lần, hỏi nhiều lần**. Nếu mỗi câu hỏi lại gửi nguyên video cho AI (kiểu Agent tự xem video), mỗi câu tốn 0,4–2,4 USD. Đây thêm một lý do chọn Workflow.
- Sinh viên khó tự trả tiền (có cách miễn phí: tua tay, NotebookLM, gói miễn phí AI Studio; nhu cầu không liên tục). Mô hình hợp lý: **nhà trường/khoa chi trả** hoặc tích hợp vào nền tảng video trường đã dùng. Rào cản chính không phải tiền mà là **quyền sử dụng video bài giảng** và **ai vận hành**.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Top 3 mốc thời gian trong video có khả năng chứa nội dung sinh viên hỏi, kèm ảnh khung hình và 1 dòng mô tả đoạn đó (ví dụ "35:10 — chứng minh đạo hàm của hàm hợp trên bảng") |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên xem đoạn gốc và tự xác định đúng đoạn cần tìm hay không; trợ giảng duyệt bộ mục lục tự sinh trước khi mở cho lớp |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh viên bấm vào mốc thời gian, xem lại lời giảng gốc của giảng viên rồi làm bài tập |
| **Outcome** — đo kết quả bằng gì? | Thời gian tìm lại một đoạn kiến thức; tỉ lệ tìm thấy đúng đoạn trong top 3; số lần sinh viên phải tua tay sau khi đã hỏi |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Video bài giảng (đã có), transcript (đã có), slide (thường có), câu hỏi của sinh viên. Chưa chắc: quyền đưa video bài giảng vào dịch vụ AI bên ngoài **[cần hỏi nhà trường/giảng viên]** |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Nút "Đúng đoạn / Không đúng" sau mỗi kết quả; câu hỏi không tìm thấy được gửi cho trợ giảng bổ sung mục lục |

### 6.4. Hai câu hỏi của Google PAIR

- **Augment hay automate?** **Augment.** AI chỉ rút ngắn bước "tìm đoạn video", việc học vẫn là sinh viên xem lời giảng gốc. Lý do: research EduVidQA cho thấy để AI tự trả lời nội dung bài giảng còn khó và dễ sai, trong khi sinh viên cần hiểu đúng cách giảng viên giải thích. **[chờ CP4]** Bổ sung bằng chứng từ phỏng vấn: sinh viên muốn "được chỉ chỗ" hay "được giải thích luôn".
- **Báo nhầm hay bỏ sót, cái nào tệ hơn?**
  - Báo nhầm **mốc thời gian** ít tệ: sinh viên mất vài giây xem là biết sai.
  - Bỏ sót (báo "không có" trong khi có) làm sinh viên quay về tua tay, tức là quay về baseline, không tệ hơn hiện tại.
  - **Tệ nhất là AI tự giải thích sai nội dung** (báo nhầm kiến thức), vì sinh viên học sai mà không biết.
  - Thiết kế xử lý: AI **không tự giải thích kiến thức**, chỉ trả mốc thời gian + khung hình gốc; luôn trả 3 ứng viên thay vì 1; nói rõ "không tìm thấy" thay vì đoán.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên học môn lập trình/toán, xem lại video bài giảng dài (khoảng 90 phút) khi làm bài tập |
| **Quy trình** | Mở lại video → nhớ mơ hồ nội dung → tìm từ khóa trong transcript → không ra thì tua và quan sát từng đoạn → xem lại đoạn tìm được → làm bài tập |
| **Bottleneck** | Định vị đoạn video khi nội dung (công thức, chứng minh) **chỉ xuất hiện trên bảng/slide**, không được giảng viên đọc thành lời nên không có trong transcript |
| **Impact** | Ước tính ban đầu (P4): 150 sinh viên × 6 lần tìm/tháng × 7 phút/lần ≈ 105 giờ học/tháng. **[chờ CP4]** Thay bằng số liệu kiểm chứng của thành viên 2 |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian tìm lại một đoạn: baseline **[chờ CP4]** (P4 ước tính 7 phút) → dưới 2 phút, đo bằng bấm giờ trên bộ 30 câu hỏi thử; (2) Tỉ lệ đúng đoạn trong top 3 ≥ 80%; (3) Với câu hỏi về nội dung **chỉ có trên bảng/slide**, tỉ lệ đúng trong top 3 ≥ 70%. **Guardrail:** 0 mốc thời gian bịa; 100% câu hỏi về nội dung không có trong video được trả lời "không tìm thấy". Khi pilot: dưới 20% lượt tìm sinh viên vẫn phải tua tay sau khi dùng công cụ |
| **Boundary** | AI **không** tự giải thích hay viết lời giải thay giảng viên; chỉ trả mốc thời gian + khung hình gốc. AI không bịa mốc thời gian không tồn tại; không tìm thấy thì nói "không tìm thấy". Chỉ dùng video thuộc khóa học được nhà trường/giảng viên cho phép. **HITL:** trợ giảng duyệt mục lục tự sinh của mỗi video trước khi mở cho lớp; sinh viên luôn tự xem đoạn gốc để xác nhận |
| **AI intervention point** | (a) Khi lập chỉ mục video: AI mô tả khung hình/đoạn có công thức (sau bước OCR bằng rule). (b) Khi sinh viên hỏi: AI so khớp câu hỏi với chỉ mục, thay cho bước "tua và quan sát từng đoạn" |
| **Mức chọn** | **Workflow** |
| **Rủi ro & người kiểm tra** | Trả sai mốc / mô tả sai công thức → sinh viên kiểm bằng cách xem đoạn gốc, bấm "Không đúng"; mục lục sai → trợ giảng duyệt trước khi mở. Transcript tự động sai (video không phụ đề, giảng viên phát âm không chuẩn, thuật ngữ chuyên ngành, tiếng Việt chen tiếng Anh, thu âm kém) → không phụ thuộc riêng transcript: index thêm kênh hình (OCR + mô tả khung hình), cung cấp danh sách thuật ngữ môn học cho bước speech-to-text, kiểm thử trên ít nhất 1 video giọng khó nghe. Quyền sử dụng video bài giảng với dịch vụ AI bên ngoài → giảng viên/nhà trường phê duyệt trước pilot |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| AI làm gì | AI phân tích transcript + hình ảnh, lập chỉ mục và trả lời câu hỏi kèm mốc thời gian | AI **chỉ trả mốc thời gian + khung hình**, không tự giải thích nội dung | EduVidQA: AI tự trả lời câu hỏi bài giảng còn khó, dễ sai kiến thức; báo nhầm kiến thức là lỗi tệ nhất (PAIR) |
| Bottleneck | Tìm đúng đoạn trong video dài | Tìm đoạn mà nội dung **chỉ có trên bảng/slide**, không có trong transcript | Research: tìm theo lời nói đã có công cụ giải (NotebookLM, transcript); khoảng trống thật nằm ở phần hình ảnh |
| Success Metric | Giảm 70% thời gian tìm kiếm | Thêm tỉ lệ đúng trong top 3, tách riêng nhóm câu hỏi "chỉ có trên bảng" | Chỉ đo thời gian thì không biết AI có tìm **đúng** không |
| Mức can thiệp | Chưa chọn | Workflow, Rule ở bước OCR | Panopto cho thấy mức Rule đã giải được phần chữ in trên slide |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

Cách kiểm: chọn 3 video bài giảng thật; trợ giảng/giảng viên viết **30 câu hỏi thử kèm mốc thời gian đúng**, gồm 10 câu nội dung có trong lời giảng, 10 câu nội dung **chỉ có trên bảng/slide**, 5 câu diễn đạt mơ hồ, 5 câu về nội dung **không có** trong video. Chạy thử (ví dụ bằng Gemini trên AI Studio) và so với cách tìm bằng từ khóa.

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đúng đoạn | Mốc đúng nằm trong top 3, lệch không quá ±30 giây | Cả 3 mốc đều sai hoặc lệch quá 30 giây |
| 2 | Tìm được nội dung chỉ có trên hình | ≥ 7/10 câu "chỉ có trên bảng/slide" đúng trong top 3 | Chỉ tìm được câu có trong transcript (không hơn tìm từ khóa) |
| 3 | Không bịa | Mọi mốc thời gian trả về đều tồn tại và khung hình khớp mô tả; 5/5 câu "không có trong video" (100%) được trả lời "không tìm thấy" | Có mốc thời gian không tồn tại, hoặc đoán bừa cho câu không có trong video |
| 4 | Không giải thích thay giảng viên | Đầu ra chỉ gồm mốc thời gian, khung hình, mô tả 1 dòng | Đầu ra tự giải thích/chứng minh công thức |
| 5 | Nhanh hơn baseline | Sinh viên thử nghiệm tìm được đoạn đúng trong dưới 2 phút | Lâu hơn hoặc ngang tua tay |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

- Panopto — Video Search and Discovery (Smart Search: ASR, OCR, slide): https://www.panopto.com/features/video-search/
- Google — NotebookLM adds audio and YouTube support (26/09/2024): https://blog.google/innovation-and-ai/products/notebooklm-audio-video-sources/
- Google AI Studio — Video understanding (YouTube URL, mốc MM:SS, 1 FPS, giới hạn gói miễn phí): https://aistudio.google.com/docs/video-understanding
- Giá Gemini API (trang tổng hợp, cần đối chiếu trang giá chính thức của Google): https://costbench.com/software/llm-api-providers/google-gemini-api/
- Ray, Sharma, Aditya, Goyal (2025). *EduVidQA: Generating and Evaluating Long-form Answers to Student Questions based on Lecture Videos*. EMNLP 2025: https://aclanthology.org/2025.emnlp-main.1760

# Báo cáo cá nhân — 2A202603780_TruongThiThuHa

## 1. Thông tin học viên

- Họ tên: Trương Thị Thu Hà
- MSSV: 2A202603780
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomE1
- Link repo nhóm: https://github.com/miao1114/K5-L3B-DAY02-NhomE1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi notebook báo lỗi, tôi muốn xác định dòng lỗi và nguyên nhân để sửa nhanh thay vì thử nhiều lần. | Học viên AI20K | Ước tính 1–2 giờ/lần, 3–4 lần/tuần. Ngày 06/11 có làm bài lab KNN và LLM phân loại JSON, phải kiểm tra và sửa code nhiều lần. Chưa đo thời gian chính xác. |
| 2 | Tốn thời gian | Khi bắt đầu project, tôi muốn thiết lập môi trường và API key nhanh để tập trung làm bài. | Học viên AI20K | Ước tính 1–3 giờ/lần, 1–2 lần/tuần. |
| 3 | Lặp lại | Khi kết thúc buổi học, tôi muốn tổng hợp kiến thức từ slide và notebook để ôn tập hiệu quả. | Học viên AI20K | Ước tính 45–60 phút/buổi, 5 buổi/tuần. |
| 4 | Tốn thời gian | Khi nhận đề lab, tôi muốn xác định các yêu cầu và thứ tự thực hiện để không bỏ sót tiêu chí. | Học viên AI20K | Ước tính 30–60 phút/đề, khoảng 5 đề/tuần. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi gặp khái niệm mới như RAG, MCP, API, tôi muốn tìm nguồn giải thích dễ hiểu để áp dụng vào bài tập. | Học viên AI20K | Ước tính 30–90 phút/khái niệm, 3–5 lần/tuần. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi phải lựa chọn prompt, mô hình hoặc cách gọi API, tôi muốn so sánh chất lượng và chi phí token để chọn phương án phù hợp. | Học viên AI20K | Ước tính 45–90 phút/lần, 1–2 lần/tuần. Ví dụ bài LLM ngày 06/11 yêu cầu so sánh chi phí token giữa JSON output và output một từ. |
| 7 | Tốn thời gian | Khi hoàn thành bài lab, tôi muốn kiểm tra từng tiêu chí rubric để tránh thiếu yêu cầu và bị trừ điểm. | Học viên AI20K | Ước tính 30–60 phút/bài, 3 lần/tuần. |
| 8 | Pain từ người khác | Khi nộp bài lab, học viên muốn biết chính xác quy định đặt tên repo và file để tránh bị trừ điểm không đáng có. | Học viên, coach | Coach Day 02 có slide "Tránh mất điểm oan" liên quan đến lỗi đặt tên (5 điểm). Bản thân đã phải hỏi lại cách đặt tên ngày 09/11. Chưa thống kê số học viên khác. |
| 9 | Pain từ người khác | Khi không theo kịp một bước trong buổi lab, học viên muốn biết phần kiến thức đang thiếu để tiếp tục làm bài mà không phải hỏi lại toàn bộ. | Học viên, coach | Vấn đề cần khảo sát thêm: dự kiến hỏi 3–5 học viên về số lần bị mắc ở một bước lab trong tuần. |
| 10 | Pain từ người khác | Khi làm việc nhóm trên GitHub, học viên muốn biết phiên bản code nào mới nhất và thay đổi ở đâu để tránh xung đột khi kết hợp bài làm. | Học viên làm nhóm | Vấn đề cần xác minh: khảo sát 3–5 học viên đã làm việc nhóm, ghi nhận số lần gặp xung đột code và thời gian xử lý. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý tưởng tự xác định:** Debug code, cấu hình môi trường, tổng hợp kiến thức, đọc đề lab và tìm hiểu khái niệm mới.
- **Ý tưởng AI hỗ trợ mở rộng:** So sánh chi phí token, kiểm tra rubric, quản lý quy định nộp bài và các khó khăn khi học hoặc làm việc nhóm.
- **Ý tưởng giữ lại:** Các vấn đề có hoạt động cụ thể, tần suất lặp lại và có thể đo lường thời gian xử lý.
- **Ý tưởng loại bỏ:** "Xây dựng AI Learning Assistant" vì đây là một giải pháp, không phải mô tả vấn đề cần giải quyết.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Debug lỗi notebook (#1) | Tần suất cao, khoảng 3–4 lần/tuần, mất nhiều thời gian | Chưa đo thời gian thực tế |
| 2 | Đọc hiểu đề lab (#4) | Gặp thường xuyên, đề Day 02 phân tán trong nhiều file | Checklist có sẵn có thể đã đủ |
| 3 | Sai quy định đặt tên (#8) | Có cảnh báo từ coach, rủi ro mất 5 điểm | Chưa biết bao nhiêu người bị trừ điểm |

### Problem Card #1 — Debug lỗi notebook

| Trường | Nội dung |
|---|---|
| Job Story | Khi notebook báo lỗi, tôi muốn xác định dòng lỗi và nguyên nhân để sửa nhanh thay vì thử nhiều lần. |
| Actor | Học viên AI20K làm bài lab Python/notebook. |
| Thời điểm / bối cảnh | Trong và sau buổi lab, khi chạy code gặp lỗi và cần hoàn thành bài đúng hạn. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc traceback → 2. Đoán nguyên nhân → 3. Tra cứu tài liệu → 4. Sửa code → 5. Chạy lại. Nếu vẫn lỗi, quay lại bước 2. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: khoảng **55 phút/lần**, do mất thời gian xác định nguyên nhân và tìm hướng xử lý. |
| Impact (nếu không giải thì sao) | Ước tính 90 phút/lần × 3–4 lần/tuần = 4,5–6 giờ/tuần. |
| Success metric (baseline → target) | Thời gian sửa lỗi: **90 phút → dưới 20 phút**. Đo bằng thời gian từ lúc xuất hiện lỗi đến khi code chạy đúng yêu cầu. |
| Phương án không dùng AI | Đọc traceback, dùng debugger, checklist lỗi phổ biến, tra cứu tài liệu, hỏi coach. |
| Giả thuyết về AI (nếu có) | Chỉ dùng cho lỗi khó, sau khi đã thử checklist: AI phân tích traceback và đoạn code liên quan, gợi ý nguyên nhân và cách sửa từng bước, không viết lại toàn bộ bài. Học viên tự kiểm tra và chạy lại. |
| Cảm nhận nhanh | Workflow có tiềm năng ứng dụng AI, nhưng cần kiểm chứng hiệu quả. |

Quy trình nháp hiện tại:

```text
[1. Đọc lỗi: 5 phút]
          ↓
[2. Đoán nguyên nhân: 25 phút] ← BOTTLENECK
          ↓
[3. Tra tài liệu: 30 phút]     ← BOTTLENECK
          ↓
[4. Sửa code: 20 phút]
          ↓
[5. Chạy lại: 10 phút]
          ↓
   Code chạy đúng?
       │       │
      Có      Không → Quay lại bước 2
       ↓
   Hoàn thành

Tổng ước tính: 90 phút/lần
```

Ví dụ: Ngày 06/11, khi thực hành KNN và bài LLM trả kết quả JSON, tôi phải kiểm tra code, đối chiếu yêu cầu và điều chỉnh nhiều lần. Thời gian 90 phút là ước lượng cho một lần debug khó, không phải thời gian đã đo riêng cho bài này.

### Problem Card #2 — Đọc hiểu đề lab

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận đề lab, tôi muốn xác định đầy đủ yêu cầu và thứ tự thực hiện để không bỏ sót tiêu chí. |
| Actor | Học viên AI20K. |
| Thời điểm / bối cảnh | Đầu buổi lab, khi cần đọc nhiều tài liệu trên GitHub. |
| Quy trình hiện tại (3–7 bước) | 1. Mở README → 2. Đọc các file liên quan → 3. Tạo checklist → 4. Đối chiếu rubric → 5. Bắt đầu làm. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: khoảng **35 phút/đề**, do thông tin nằm ở nhiều file. |
| Impact (nếu không giải thì sao) | Ước tính 50 phút/đề × 5 đề/tuần = 250 phút/tuần. Có rủi ro bỏ sót yêu cầu. |
| Success metric (baseline → target) | Thời gian tạo checklist: **50 phút → dưới 15 phút**. Số tiêu chí bị bỏ sót: chưa có baseline → mục tiêu 0. |
| Phương án không dùng AI | Dùng CHECKPOINTS.md, SUBMISSION.md hoặc mẫu checklist chuẩn. |
| Giả thuyết về AI (nếu có) | AI tổng hợp nội dung các file thành checklist, kèm đường dẫn tới yêu cầu gốc để học viên đối chiếu. |
| Cảm nhận nhanh | No AI hoặc Rule có thể đủ nếu tài liệu đã rõ ràng. |

Quy trình nháp hiện tại:

```text
[1. Mở README: 5 phút]
          ↓
[2. Đọc file liên quan: 20 phút] ← BOTTLENECK
          ↓
[3. Tạo checklist: 15 phút]      ← BOTTLENECK
          ↓
[4. Đối chiếu rubric: 10 phút]
          ↓
[5. Bắt đầu làm bài]

Tổng: 50 phút/đề
```

### Problem Card #3 — Sai quy định đặt tên khi nộp

| Trường | Nội dung |
|---|---|
| Job Story | Khi nộp bài lab, tôi muốn xác định đúng tên repo và file để tránh bị trừ điểm. |
| Actor | Học viên AI20K và coach. |
| Thời điểm / bối cảnh | Khi tạo repository và chuẩn bị nộp bài. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc README/SUBMISSION → 2. Xem slide coach → 3. Hỏi lại quy định → 4. Đặt tên → 5. Nộp LMS. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: khoảng **15 phút**, do cần xác minh cách đặt tên giữa các nguồn. |
| Impact (nếu không giải thì sao) | Nguy cơ bị trừ 5 điểm nếu nộp sai quy định. |
| Success metric (baseline → target) | Thời gian xác nhận tên đúng: **15 phút → dưới 2 phút**. Số lần bị trừ điểm: chưa có baseline → mục tiêu 0. |
| Phương án không dùng AI | Chuẩn hóa hướng dẫn, tạo checklist hoặc script kiểm tra tên tự động. |
| Giả thuyết về AI (nếu có) | Không cần AI nếu quy định là mẫu cố định. |
| Cảm nhận nhanh | Rule. |

Quy trình nháp hiện tại:

```text
[1. Đọc README/SUBMISSION: 5 phút]
          ↓
[2. Xem slide coach: 5 phút]
          ↓
[3. Hỏi lại quy định: 15 phút] ← BOTTLENECK
          ↓
[4. Đặt tên repo/file: 3 phút]
          ↓
[5. Nộp LMS: 2 phút]

Tổng: 30 phút/lần
```

Đã kiểm tra ngày 09/11: hai nguồn cùng quy định **tên repo** nhưng ghi khác nhau. `SUBMISSION.md` ghi `K5-<L3A/L3B>-DAY02-TenNhom-DiscoveryProblemFraming` và nói rõ không dùng họ tên hay MSSV; slide của coach ghi `K5-<L3A/L3B>-DAY02-HoVaTen-MSSV-DiscoveryProblemFraming`. Đây là bằng chứng thật cho bottleneck ở bước 3.

### Card muốn pitch nhất

- Card số: #1 – Debug lỗi notebook.
- Vì sao: Đây là vấn đề xuất hiện thường xuyên trong quá trình học AI20K, có quy trình rõ ràng và gây tốn nhiều thời gian. Công việc đòi hỏi đọc traceback, hiểu logic và đối chiếu code với tài liệu nên có khả năng tận dụng LLM. Hiệu quả có thể đo bằng thời gian sửa lỗi và tỷ lệ sửa đúng.
- Câu hỏi muốn nhóm phản biện: "Liệu việc sử dụng AI để phân tích và gợi ý sửa lỗi notebook có thực sự giảm thời gian debug từ khoảng 90 phút xuống dưới 20 phút so với việc sử dụng checklist và debugger thông thường, mà vẫn đảm bảo học viên hiểu nguyên nhân lỗi?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 90 phút chưa được đo thực tế, chỉ là ước lượng. | Có | Ghi rõ là ước lượng và đề xuất bấm giờ trong 1 tuần để thu thập baseline. |
| Không phải lỗi nào cũng cần AI. Các lỗi đơn giản có thể sửa bằng debugger. | Có | Bổ sung phương án không dùng AI; chỉ ưu tiên AI cho lỗi khó xác định nguyên nhân. |
| AI có thể đưa ra cách sửa sai hoặc làm thay đổi logic bài tập. | Có | Học viên phải tự kiểm tra, chạy lại và đối chiếu yêu cầu trước khi chấp nhận kết quả. |
| Mục tiêu giảm xuống dưới 20 phút có thể quá tham vọng. | Có | Giữ dưới 20 phút làm mục tiêu thử nghiệm, không khẳng định chắc chắn đạt được. |
| Chưa chứng minh AI tốt hơn cách debug thông thường. | Có | Đề xuất so sánh các lần debug bằng checklist/debugger với các lần có AI hỗ trợ, ghi nhận thời gian và tỷ lệ sửa đúng. |
| Nếu sử dụng AI để sửa toàn bộ code, học viên có thể không hiểu bài. | Có | Giới hạn vai trò AI ở phân tích nguyên nhân, hướng dẫn kiểm tra và gợi ý sửa từng bước; không mặc định viết lại toàn bộ bài. |

**Kết luận sau phản biện:** Giữ Card #1 để pitch, nhưng chưa khẳng định AI là giải pháp tối ưu. Cần kiểm chứng bằng dữ liệu thực tế và so sánh với phương án không dùng AI.

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| **Pitch Problem Card** | Pitch Card #1 “Debug lỗi notebook”, với giả định mất khoảng 90 phút/lần, 3–4 lần/tuần. Đặt câu hỏi phản biện: “Liệu AI phân tích và gợi ý sửa lỗi notebook có thực sự giảm thời gian debug từ 90 phút xuống dưới 20 phút so với checklist/debugger?” | Card #1 không được chọn. Nhóm thống nhất lựa chọn P4 về tìm lại nội dung trong video bài giảng dài. |
| **Phản biện bài của bạn khác** | Đặt 4 câu hỏi trong quá trình thảo luận P4: (1) Độ chính xác của speech-to-text khi video không có phụ đề, giảng viên phát âm không rõ và OCR đa ngôn ngữ; (2) Có nên gợi ý kiến thức liên quan hay không; (3) User research đã chứng minh người dùng có nhu cầu đủ lớn để trả phí chưa; (4) Đã xác định ngưỡng sai số và độ chính xác của AI chưa? | Câu 1 góp phần hình thành giả định #5 về Feasibility. Câu 3 góp phần hình thành giả định #6 về Viability và câu 11 trong survey. Câu 2 được đối chiếu với kết quả survey (1/7 người gặp khó khăn ở bước xem lại để hiểu), hỗ trợ quyết định giữ phạm vi “tìm lại” thay vì “giải thích”. Câu 4 đã được đề xuất để bổ sung tiêu chí đánh giá AI nhưng chưa đưa vào bài nhóm. |
| **Nhận phản biện** | Có pitch Card #1 để nhóm xem xét, nhưng không ghi lại được câu hỏi phản biện cụ thể từ các thành viên. | Không ghi nhận nội dung chỉnh sửa trực tiếp từ phản biện vì thiếu thông tin xác minh. |
| **Gom cluster / cây OST** | Không trực tiếp phụ trách. Leader và Thành viên 4 thực hiện. | — |
| **Chọn Candidate Problem** | Trực tiếp tham gia thảo luận, phản biện và lựa chọn P4 cùng nhóm. Đóng góp góc nhìn về tính khả thi kỹ thuật, nhu cầu người dùng và phạm vi giải pháp. | Nhóm thống nhất lựa chọn P4 để tiếp tục kiểm chứng bằng user research. |
| **Kiểm chứng / Research** | Phụ trách CP4: xây dựng Assumption Map với 6 giả định; thiết kế Google Form gồm 12 câu theo nguyên tắc The Mom Test; thu thập 7 phản hồi từ học viên nhóm khác; tổng hợp kết quả và phân loại tín hiệu xác nhận/phản bác. Tạo PR #1 trên GitHub. Ngoài ra, nghiên cứu 5 công cụ tương tự gồm Panopto, NotebookLM, Ask YouTube, ClassTranscribe và TwelveLabs; hoàn thành bộ 5 slide và gửi Thành viên 3 tham khảo. | Kết quả survey phản bác giả định #2: 0/7 người báo cáo mất trên 5 phút và không có người tham gia nào nêu nhu cầu tìm công thức. Nhóm điều chỉnh problem theo hướng “định vị đoạn code/giải thích trong nhiều video”, đồng thời hạ ước tính impact xuống khoảng 5–15 phút/tuần/người (ước tính cần kiểm chứng thêm). Kết quả 7/7 từng trả phí cho AI học tập chỉ là tín hiệu tham khảo, chưa chứng minh sẵn sàng trả phí cho giải pháp P4. |
| **Quy trình nhóm** | Không trực tiếp phụ trách. Thành viên 4 thực hiện. | — |
| **Problem Statement** | Phụ trách xây dựng Problem Statement v0, sử dụng kết quả survey làm baseline và điều chỉnh phạm vi vấn đề theo bằng chứng thu thập được. | Đang thực hiện; chưa ghi nhận là bản hoàn thành. |
| **Mức can thiệp AI** | Không trực tiếp phụ trách (Thành viên 3 thực hiện). Đóng góp phản biện về độ chính xác của speech-to-text, OCR và tiêu chí đánh giá AI. | Đã đề xuất xem xét giới hạn kỹ thuật và tiêu chí chất lượng AI; phần tiêu chí đánh giá chưa được tích hợp vào bài nhóm. |
| **Quyết định** | Không phụ trách tổng hợp quyết định cuối cùng (Leader thực hiện). Có tham gia thảo luận lựa chọn P4. | Đóng góp ý kiến và bằng chứng research phục vụ việc xác định phạm vi vấn đề. |

**Minh chứng:** [Pull Request #1 – CP4 Research](https://github.com/miao1114/K5-L3B-DAY02-NhomE1-DiscoveryProblemFraming/pull/1)

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tự liệt kê các vấn đề trước; dùng ChatGPT gợi ý thêm ý và dùng Claude chuyển ý thô sang mẫu Job Story "Khi… tôi muốn… để…" | Chuẩn hóa cách viết, chỉ ra dòng còn chứa chữ "AI" hoặc thiếu dấu hiệu thật | AI gợi ý "xây dựng AI Learning Assistant", là giải pháp chứ chưa phải vấn đề; các con số AI đưa ra chỉ là ước lượng chung | Bỏ ý giải pháp; tự thêm ví dụ thật (lab KNN và LLM ngày 06/11); ghi rõ số nào là ước tính |
| CP2 Problem Card | Dùng Claude dựng khung 3 Problem Card và quy trình nháp; dùng ChatGPT đóng vai "PM hoài nghi" phản biện card #1 | Phản biện của ChatGPT chỉ ra baseline 90 phút chưa đo, thiếu phương án không dùng AI, rủi ro AI sửa sai làm học viên không hiểu bài | Khung do AI dựng để trống số phút, AI không biết trải nghiệm thật của tôi; một số phản biện chung chung, áp dụng cho card nào cũng được | Tự điền số phút từng bước theo trải nghiệm; giới hạn vai trò AI chỉ cho lỗi khó, gợi ý từng bước, không viết lại cả bài |
| CP4 Research | Dùng Claude soạn câu hỏi survey theo The Mom Test và tạo Google Form, đếm và tổng hợp 7 phản hồi, tìm 5 công cụ tương tự kèm nguồn và làm 5 slide; dùng ChatGPT soạn kịch bản phỏng vấn | Tạo form nhanh, đếm số liệu chính xác, tìm được công cụ thật kèm link nguồn | ChatGPT tạo 2 bài "phỏng vấn mẫu" mang tính giả định, không phải dữ liệu thật; nhiều ô trong bảng so sánh công cụ chỉ ghi "chưa rõ" vì nguồn không nói | Không đưa phỏng vấn giả định vào bài, chọn survey thay phỏng vấn; giữ nguyên ô "chưa rõ" thay vì đoán; tự đọc kết quả survey và đề xuất thu hẹp problem |
| CP5 Quy trình | Không phụ trách (Thành viên 4), không dùng AI cho phần này | — | — | — |
| CP5–6 Problem Statement | Chưa thực hiện (đang làm v0) | — | — | — |
| CP6 Mức can thiệp / quyết định | Dùng Claude để kiểm tra các câu phản biện của tôi về speech-to-text, OCR, khả năng trả tiền và ngưỡng sai số | Gợi ý boundary "AI chỉ trả mốc thời gian kèm ảnh khung hình gốc", và cách đo độ chính xác (tìm đúng trong top 3, lệch ≤ 30 giây) | Các ngưỡng (8/10, 30 giây) chỉ là đề xuất, chưa có dữ liệu thử thật | Ghi là đề xuất, chưa đưa vào bài nhóm; để Thành viên 3 quyết định sau khi thử trên video thật |
| CP7 Tổng hợp đóng góp (mục 4) | Dùng ChatGPT chỉnh câu chữ bảng đóng góp | Câu văn rõ ràng, đủ ý | ChatGPT thêm đoạn "Tổng kết" và "Bài học rút ra" chung chung, không phải lời của tôi | Bỏ hai đoạn đó, chỉ giữ việc tôi đã làm thật |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi nhận ra một vấn đề nghiêm trọng với cá nhân chưa chắc đã phổ biến. Việc lựa chọn problem cần dựa trên tần suất, mức độ ảnh hưởng và bằng chứng thực tế thay vì cảm nhận chủ quan.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Nhóm từng tập trung vào OCR và speech-to-text trước khi xác thực nhu cầu. Sau đó, nhóm xây dựng Assumption Map và khảo sát người dùng để thu hẹp phạm vi vấn đề.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Ban đầu, tôi cho rằng AI giúp giảm thời gian debug notebook từ 90 xuống 20 phút là một ý tưởng tốt. Sau khi thảo luận, tôi nhận ra đây chỉ là giả định chưa được kiểm chứng và đồng ý chuyển sang nghiên cứu P4.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có. Khảo sát cho thấy 0/7 người mất trên 5 phút để tìm nội dung và không ai cần tìm công thức. Kết quả này trái với dự đoán ban đầu, khiến tôi nhận ra cần ưu tiên dữ liệu thay vì giả định.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là thu hẹp phạm vi vấn đề theo bằng chứng thực tế, phân biệt dữ liệu đã kiểm chứng với giả định và tránh phóng đại mức độ ảnh hưởng.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Tôi sẽ phỏng vấn trực tiếp người dùng sớm hơn, tập trung vào trải nghiệm thực tế. Khi phản biện, tôi sẽ hỏi kỹ hơn về bằng chứng chứng minh vấn đề đủ nghiêm trọng và thường xuyên để cần giải pháp AI.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Nhóm E1 lựa chọn vấn đề sinh viên gặp khó khăn khi tìm lại nội dung trong video bài giảng dài. Quy trình hiện tại là tua video thủ công và quan sát để xác nhận đúng đoạn cần tìm. Nhóm đặt mục tiêu giảm thời gian tìm kiếm từ 2–5 phút xuống không quá 2 phút. Qua khảo sát 7 học viên, nhóm nhận thấy mức độ nghiêm trọng của vấn đề chưa được chứng minh rõ ràng. AI được cân nhắc để hỗ trợ định vị nội dung, với giới hạn chỉ trả về mốc thời gian và khung hình gốc, không tự giải thích kiến thức. Nhóm cần xác định mức can thiệp phù hợp và so sánh hiệu quả với phương án No AI và Rule. Vì vậy, nhóm quyết định Not Yet, ưu tiên đo baseline thực tế và kiểm chứng hiệu quả trước khi triển khai AI.

---

## 7. Tài liệu tham khảo

-

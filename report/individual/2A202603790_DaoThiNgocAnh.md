# Báo cáo cá nhân — 2A202603790_DaoThiNgocAnh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đào Thị Ngọc Anh
- MSSV: 2A202603790
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm E1
- Link repo nhóm: https://github.com/miao1114/K5-L3B-DAY02-NhomE1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi khám xong và ra quầy thanh toán viện phí, tôi (bệnh nhân) muốn hóa đơn được tính đúng ngay, để không phải chờ nhân viên ngồi kiểm tra lại từng điều kiện bảo hiểm và từng dịch vụ y tế đã sử dụng | Bệnh nhân, nhân viên thanh toán hóa đơn, bệnh viện | 1 hóa đơn có thể mất 2–3 giờ chờ gọi thanh toán; phải chờ tuần tự đến lượt nên mất rất nhiều thời gian |
| 2 | Lặp lại | Khi lập hóa đơn cho bệnh nhân, tôi (nhân viên bệnh viện) muốn các dịch vụ từ mọi phòng ban tự gom về theo mã bệnh nhân, để không phải check mã của từng bệnh nhân ở từng phòng ban rồi nhập tay vào hóa đơn | Nhân viên, bệnh nhân, bệnh viện | Vẫn phải thanh toán thủ công qua nhân viên nên mọi người chờ lâu; nhân viên lặp lại việc tạo hóa đơn cả ngày, dễ nhầm lẫn vì xử lý quá nhiều mã bệnh nhân trong 1 ngày |
| 3 | Tốn thời gian | Khi cuối tháng nhận hàng trăm hóa đơn VAT (giấy hoặc PDF) từ nhiều nhà cung cấp, tôi (kế toán) muốn mã số thuế, tên hàng hóa, tiền thuế… tự vào phần mềm kế toán, để không phải nhìn từng tờ và gõ tay từng dòng | Nhân viên kế toán, doanh nghiệp | Hàng trăm hóa đơn/tháng nhập tay; dễ nhầm lẫn khi thống kê, tính toán |
| 4 | Lặp lại | Khi chấm xong bài thi tự luận, tôi (giáo viên) muốn điểm trên giấy thi được đưa vào phần mềm quản lý điểm mà không phải lật từng tờ và gõ tay, để không nhập sai điểm của học sinh | Giáo viên, học sinh | Tốn nhiều thời gian; chỉ cần hoa mắt gõ nhầm một dòng là sai điểm của học sinh |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tra cứu tình trạng tốt nghiệp của một sinh viên, tôi (chuyên viên trường đại học) muốn tìm được hồ sơ đầy đủ ở một chỗ, để trả lời nhanh mà không phải lục nhiều nguồn | Chuyên viên tại trường, sinh viên/cựu sinh viên | Có trường hợp không tìm được vì hồ sơ đã quá lâu; form lưu thông tin không thống nhất giữa các năm |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- _(Tự điền: nếu CP1 có dùng AI gợi ý thêm vấn đề thì ghi ý giữ lại / bỏ đi và lý do; nếu không dùng thì ghi "Không dùng AI ở CP1".)_

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> Các con số thời gian/số lượng trong 3 card dưới đây là **ước lượng ban đầu**, cần bấm giờ hoặc phỏng vấn người làm thật để kiểm chứng ở CP4.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Thanh toán viện phí | Ảnh hưởng nhiều người cùng lúc (bệnh nhân chờ 2–3 giờ, nhân viên lặp lại cả ngày); gộp được 2 vấn đề #1 và #2 ở CP1 | Thời gian chờ có thể do khâu khác (chờ kết quả xét nghiệm), không chỉ khâu thanh toán; có thể chỉ cần tích hợp HIS, không cần AI |
| 2 | Nhập hóa đơn VAT / thống kê cuối tháng của doanh nghiệp | Lặp lại hằng tháng, khối lượng lớn, bottleneck rõ (gõ tay), sai sót ảnh hưởng tới kê khai thuế | Hóa đơn điện tử đã bắt buộc và có file XML, nên tỷ lệ hóa đơn giấy/scan thực tế còn lại là bao nhiêu? |
| 3 | Tra cứu thông tin / tình trạng tốt nghiệp sinh viên | Dữ liệu phân tán, không thống nhất; có lúc không tìm được hồ sơ | Tần suất yêu cầu có đủ lớn không; gốc rễ có phải là dữ liệu chưa được số hóa (AI không giải quyết được) |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi bệnh nhân khám/điều trị xong và đến quầy thanh toán, tôi muốn có ngay danh sách đầy đủ dịch vụ bệnh nhân đã dùng ở mọi khoa kèm phần BHYT chi trả, để xuất hóa đơn nhanh và đúng, bệnh nhân không phải chờ lâu |
| Actor | Nhân viên thu ngân / thanh toán viện phí (người chịu ảnh hưởng gián tiếp: bệnh nhân) |
| Thời điểm / bối cảnh | Giờ cao điểm 8h–11h sáng và lúc bệnh nhân làm thủ tục ra viện, hàng chờ dài ở quầy |
| Quy trình hiện tại (3–7 bước) | 1. Nhận phiếu / mã bệnh nhân · 2. Tra dịch vụ đã dùng ở từng khoa (xét nghiệm, chẩn đoán hình ảnh, thuốc, giường) · 3. Đối chiếu chỉ định với dịch vụ đã thực hiện · 4. Kiểm tra thẻ BHYT (tuyến, mức hưởng, danh mục được chi trả) · 5. Tính phần BHYT trả và phần bệnh nhân trả · 6. Xuất hóa đơn · 7. Thu tiền, trả biên lai |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4, gom dịch vụ từ nhiều khoa và kiểm tra điều kiện BHYT: khoảng 8 phút/hồ sơ, dễ sót dịch vụ hoặc áp sai mức hưởng |
| Impact (nếu không giải thì sao) | Khoảng 12 phút/hồ sơ; 1 quầy xử lý khoảng 35 hồ sơ/ngày nên giờ cao điểm bệnh nhân chờ 2–3 giờ. Áp sai BHYT thì bệnh viện bị xuất toán và phải làm lại |
| Success metric (baseline → target) | Thời gian xử lý 12 → dưới 5 phút/hồ sơ; thời gian chờ giờ cao điểm 2–3 giờ → dưới 45 phút; tỷ lệ hồ sơ bị BHYT từ chối không tăng |
| Phương án không dùng AI | Hệ thống HIS tự gom dịch vụ theo mã bệnh nhân + rule engine tính BHYT + thanh toán QR/kiosk: giải quyết phần lớn việc gom số liệu và tính tiền, nhưng chưa bắt được các ca chỉ định bất thường hoặc sai danh mục |
| Giả thuyết về AI (nếu có) | AI đối chiếu dịch vụ đã dùng với quy định BHYT và cảnh báo dịch vụ có nguy cơ bị từ chối hoặc bị sót; nhân viên duyệt trước khi xuất hóa đơn |
| Cảm nhận nhanh | Workflow (chủ yếu Rule, AI chỉ ở bước kiểm tra) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~12 phút/hồ sơ

[1 Nhận mã BN: 1'] → [2 Tra dịch vụ các khoa: 4'] → [3 Đối chiếu chỉ định: 2']
→ [4 Check BHYT: 2'] ← BOTTLENECK (bước 2–4)
→ [5 Tính tiền: 1'] → [6 Xuất hóa đơn: 1'] → [7 Thu tiền: 1']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi cuối tháng nhận hàng trăm hóa đơn VAT (giấy hoặc PDF) từ nhiều nhà cung cấp, tôi muốn thông tin trên hóa đơn (MST, tên hàng, số tiền, tiền thuế) tự vào phần mềm kế toán, để chốt sổ và kê khai thuế đúng hạn mà không phải gõ tay từng dòng |
| Actor | Kế toán viên (mảng mua hàng / thuế) ở doanh nghiệp vừa và nhỏ |
| Thời điểm / bối cảnh | Từ ngày 25 đến ngày 5 tháng sau, trước hạn nộp tờ khai thuế GTGT |
| Quy trình hiện tại (3–7 bước) | 1. Gom hóa đơn (email, giấy, Zalo) · 2. Phân loại theo nhà cung cấp / loại chi phí · 3. Đọc và gõ từng trường vào phần mềm · 4. Tra cứu tính hợp lệ của hóa đơn và MST trên cổng thuế · 5. Đối chiếu với PO / phiếu nhập kho · 6. Hạch toán · 7. Lập bảng kê, kiểm tra tổng |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, gõ tay: khoảng 3 phút/hóa đơn, dễ gõ nhầm số tiền hoặc MST, phát hiện muộn khi đối chiếu tổng |
| Impact (nếu không giải thì sao) | 300 hóa đơn × 3 phút ≈ 15 giờ/tháng chỉ để gõ; sai sót thì phải điều chỉnh tờ khai, có nguy cơ bị phạt |
| Success metric (baseline → target) | Thời gian nhập 3 phút → dưới 45 giây/hóa đơn; tỷ lệ sai trường dưới 1%; chốt sổ trước ngày 5 hằng tháng |
| Phương án không dùng AI | Tải file XML hóa đơn điện tử từ cổng của Tổng cục Thuế rồi import thẳng vào phần mềm kế toán: giải quyết gần hết hóa đơn điện tử, nhưng không xử lý được hóa đơn giấy, bản scan hoặc PDF không kèm XML |
| Giả thuyết về AI (nếu có) | OCR + LLM trích xuất các trường từ hóa đơn scan/PDF thành dữ liệu có cấu trúc, đánh dấu các trường có độ tin cậy thấp; kế toán duyệt rồi mới import |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~3–4 phút/hóa đơn (≈ 15–20 giờ/tháng)

[1 Gom: 10'/ngày] → [2 Phân loại: 20s] → [3 Gõ tay: 3'] ← BOTTLENECK
→ [4 Tra hợp lệ: 30s] → [5 Đối chiếu PO: 30s] → [6 Hạch toán: 20s] → [7 Bảng kê: 2h/tháng]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận yêu cầu tra cứu tình trạng tốt nghiệp của một sinh viên (doanh nghiệp xác minh bằng, cựu sinh viên xin giấy xác nhận), tôi muốn tìm ra hồ sơ đầy đủ của sinh viên đó trong vài phút, để trả lời đúng hạn mà không phải lục nhiều nguồn |
| Actor | Chuyên viên Phòng Đào tạo / Công tác sinh viên |
| Thời điểm / bối cảnh | Hằng ngày, tăng mạnh vào mùa tuyển dụng và mùa xét tốt nghiệp; khó nhất với các khóa cũ (trước khi có phần mềm quản lý) |
| Quy trình hiện tại (3–7 bước) | 1. Nhận yêu cầu (email, giấy, điện thoại) · 2. Tìm trong phần mềm quản lý đào tạo · 3. Không thấy thì mở các file Excel theo khóa/năm · 4. Lục quyết định tốt nghiệp / sổ gốc cấp bằng (giấy hoặc scan) · 5. Đối chiếu họ tên, ngày sinh, MSSV giữa các nguồn khác định dạng · 6. Soạn phản hồi / giấy xác nhận · 7. Trình ký, gửi |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5, dữ liệu phân tán và không thống nhất (tên có/không dấu, MSSV đổi định dạng qua các năm): 20–60 phút/yêu cầu với khóa cũ, có lúc không tìm thấy |
| Impact (nếu không giải thì sao) | Giả định 10 yêu cầu/tuần × khoảng 40 phút ≈ 6–7 giờ/tuần/chuyên viên; trả lời chậm thì sinh viên lỡ hồ sơ xin việc, nhà trường mất uy tín |
| Success metric (baseline → target) | Thời gian ~40 → dưới 10 phút/yêu cầu; tỷ lệ "không tìm thấy" giảm một nửa; không có thông tin sai lệch nào trong giấy xác nhận |
| Phương án không dùng AI | Số hóa sổ gốc, gom các file Excel về một cơ sở dữ liệu, chuẩn hóa định dạng, tìm kiếm mờ theo tên: hiệu quả lâu dài nhưng tốn công làm sạch dữ liệu một lần (lớn) |
| Giả thuyết về AI (nếu có) | AI tìm và ghép bản ghi trên nhiều nguồn (phần mềm, Excel, bản scan), trả về các ứng viên khớp kèm nguồn trích dẫn; chuyên viên xác nhận; AI không tự gửi thông tin ra ngoài |
| Cảm nhận nhanh | Agent hoặc Workflow (tìm kiếm + RAG) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~40 phút/yêu cầu (khóa cũ)

[1 Nhận yêu cầu: 2'] → [2 Tìm phần mềm: 3'] → [3 Lục Excel: 10']
→ [4 Lục sổ gốc / scan: 15'] → [5 Đối chiếu: 5'] ← BOTTLENECK (bước 3–5)
→ [6 Soạn phản hồi: 3'] → [7 Trình ký, gửi: 2']
```

### Card muốn pitch nhất

- Card số: 1 (Thanh toán viện phí)
- Vì sao: Ảnh hưởng trực tiếp tới nhiều người mỗi ngày (bệnh nhân chờ 2–3 giờ), dấu hiệu thật rõ ràng, và gom được cả 2 vấn đề lặp lại + tốn thời gian ở CP1.
- Câu hỏi muốn nhóm phản biện: Thời gian chờ 2–3 giờ thực sự nằm ở khâu thanh toán hay ở khâu khác? Và vấn đề này có cần AI không, hay chỉ cần tích hợp hệ thống HIS + rule tính BHYT là đủ?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: phần lớn vấn đề có thể là thiếu tích hợp hệ thống HIS, không cần AI | Đồng ý một phần | Ghi rõ HIS + rule engine trong "Phương án không dùng AI"; thu hẹp vai trò AI chỉ còn bước cảnh báo sai/sót BHYT; đổi cảm nhận nhanh thành Workflow (chủ yếu Rule) |
| Card #2: hóa đơn điện tử đã bắt buộc và có XML, nên impact có thể nhỏ hơn ước tính | Đồng ý | Thêm phương án import XML; giới hạn phạm vi AI ở hóa đơn giấy/scan/PDF; đưa "tỷ lệ hóa đơn giấy còn lại" vào danh sách cần kiểm chứng |
| Card #3: gốc rễ là dữ liệu chưa số hóa / không thống nhất; dữ liệu cá nhân sinh viên nhạy cảm | Đồng ý | Thêm boundary: chuyên viên xác nhận, AI không tự gửi thông tin ra ngoài; xếp card này ở rank 3 |
| Cả 3 card: baseline thời gian chỉ là ước lượng | Đồng ý | Ghi chú các số liệu là ước lượng, sẽ bấm giờ / phỏng vấn người làm thật ở CP4 |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Chọn candidate problem | Tham gia chấm điểm shortlist. Nhóm chọn bài toán sinh viên khó tìm lại đoạn kiến thức trong video bài giảng dài, khi công thức chỉ có trên bảng/slide| Nhóm chọn candidate P4 |
| Kiểm chứng / research | **Phụ trách CP4 Research.** Tự mở và kiểm tra 4 nguồn: Panopto Smart Search, Google NotebookLM, Gemini API video understanding, nghiên cứu EduVidQA (EMNLP 2025). Với mỗi nguồn ghi rõ giải bước nào trong quy trình, điểm mạnh, khoảng trống/rủi ro | Mục 3.3 của `group_report.md`. Kết luận: mức Rule (OCR + từ khóa) đã giải được một phần; công cụ chỉ dựa transcript không giải được ca công thức chỉ có trên bảng → nhóm thu hẹp bottleneck và không tự xây agent |
| Quy trình nhóm | Cung cấp quy trình hiện tại 5 bước của sinh viên (mở video → nhớ mơ hồ → tìm từ khóa → tua tay → xem lại) để đối chiếu cột "Giải bước nào" trong bảng research.| Giúp chỉ ra đúng bước 3–4 là chỗ các công cụ hiện có còn bỏ trống |
| Problem Statement | **Viết Problem Statement v1** và bảng thay đổi v0 → v1 (AI chỉ trả mốc thời gian + khung hình; bottleneck đổi thành "nội dung chỉ có trên bảng/slide"; thêm metric tỉ lệ đúng trong top 3). Viết 5 tiêu chí đánh giá đầu ra của AI | Mục 7 của `group_report.md`. Bài nhóm có metric đo được độ **đúng**, không chỉ đo thời gian |
| Mức can thiệp AI | **Phụ trách CP6.** Đặt bài vào ma trận độ mơ hồ cao × phức tạp trung bình; so sánh 4 mức No AI / Rule / Workflow / Agent; viết AI Canvas và 2 câu hỏi Google PAIR | Mục 6.1–6.4. Nhóm chọn **Workflow** (Rule ở bước OCR, AI ở bước mô tả khung hình và so khớp câu hỏi), có lý do vì sao không chọn mức đơn giản hơn |
| Quyết định | Ước tính chi phí lập chỉ mục video (≈ 0,4–2,4 USD/video, chỉ rẻ khi "index một lần, hỏi nhiều lần") và chỉ ra rào cản chính là quyền dùng video bài giảng, không phải tiền | Đầu vào cho dòng Viability ở mục 8.1; góp phần vào quyết định **Not Yet** của nhóm |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-

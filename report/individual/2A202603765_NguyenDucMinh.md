# Báo cáo cá nhân — 2A202603765_NguyenDucMinh

## 1. Thông tin học viên

- Họ tên: Nguyễn Đức Minh
- MSSV: 2A202603765
- Tên nhóm: Nhóm E1
- Link repo nhóm: https://github.com/miao1114/K5-L3B-DAY02-NhomE1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Các số liệu dưới đây là ước lượng ban đầu, chưa đo thực tế.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi chấm bài toán viết tay, tôi muốn biết học sinh sai từ bước nào, để hướng dẫn sửa bài. | Giáo viên, học sinh | Khoảng 5 phút/bài, 30 bài/đợt. |
| 2 | Tốn thời gian | Khi làm bài tập, tôi muốn tìm lại đúng đoạn kiến thức trong video bài giảng, để tiếp tục làm bài. | Sinh viên | Khoảng 7 phút/lần tìm, 6 lần/tháng. |
| 3 | Lặp lại | Khi nhận đơn bán sỉ qua tin nhắn, ảnh hoặc ghi âm, tôi muốn xác định đúng mặt hàng và số lượng, để tránh nhập sai đơn. | Nhân viên nhập đơn, đại lý | Khoảng 4 phút/đơn, 60 đơn/ngày. |
| 4 | Pain từ người khác | Khi đọc nhóm Zalo lớp, tôi muốn biết thông báo nào cần làm và hạn khi nào, để không bỏ lỡ việc của con. | Phụ huynh, học sinh | Khoảng 10 phút/ngày đọc và ghi lại thông báo. |
| 5 | Lặp lại | Khi tính tiền điện nước cuối tháng, tôi muốn đọc đúng chỉ số từ ảnh đồng hồ, để tính đúng tiền từng phòng. | Chủ trọ, người thuê | Khoảng 4,7 giờ/tháng cho 40 phòng. |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi khách gửi nhiều phản hồi sửa video, tôi muốn biết yêu cầu mới nhất, để sửa đủ và đúng ý khách. | Người dựng video, khách hàng | Khoảng 20 phản hồi/video, 2 phút xử lý/phản hồi. |

**Dùng AI:** Hỗ trợ diễn đạt và phân loại 6 ý; bỏ các ý quá rộng như “trợ lý quản lý mọi thông báo”.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

Thời lượng là giả định cần kiểm chứng; target là mục tiêu đề xuất, chưa phải kết quả thực tế.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm bước giải sai trong bài toán viết tay (#1) | Actor rõ, có thể đối chiếu kết quả với giáo viên. | Đọc chữ viết tay và nhận diện cách giải khác mẫu có chính xác không? |
| 2 | Tìm lại kiến thức trong video bài giảng (#2) | Tình huống cụ thể, đo được thời gian tìm và độ đúng của đoạn. | Mục lục và transcript đã đủ chưa? |
| 3 | Chuẩn hóa đơn hàng bán sỉ (#3) | Lặp lại thường xuyên, dữ liệu đầu ra rõ. | Có danh mục mã hàng và lịch sử để đối chiếu không? |

### Problem Card #1 — Tìm bước giải sai trong bài toán viết tay

| Trường | Nội dung |
|---|---|
| Job Story | Khi chấm bài toán viết tay, tôi muốn tìm bước sai đầu tiên và nguyên nhân, để hướng dẫn học sinh sửa bài. |
| Actor | Giáo viên Toán THCS. |
| Thời điểm / bối cảnh | Sau bài tập hoặc kiểm tra; giới hạn ở phương trình bậc hai, có đề, ảnh bài giải rõ và tiêu chí chấm. |
| Quy trình hiện tại | Xem đề → đọc bài giải → kiểm tra từng bước → viết hướng dẫn sửa → kiểm tra nhận xét. |
| Bottleneck | Bước 3: tìm bước sai và phân loại lỗi, khoảng **2/5 phút/bài**. |
| Impact | Phản hồi chậm hoặc chưa rõ nguyên nhân; khoảng **150 phút cho 30 bài**. |
| Success metric | **5 → ≤ 3 phút/bài**, gồm giáo viên duyệt. Thử trên 30 bài: xác định đúng bước sai đầu tiên và loại lỗi ở ít nhất 90% bài có lỗi; không đánh dấu sai bài đúng trong mẫu. Nhãn đối chiếu do giáo viên xác nhận. |
| Phương án không dùng AI | Tiêu chí chấm theo bước, danh mục lỗi thường gặp và mẫu nhận xét. |
| Giả thuyết về AI | Đề xuất bước sai, loại lỗi và giải thích từ ảnh bài giải. Giáo viên duyệt; ảnh khó đọc chuyển về kiểm tra thủ công, không tự chấm điểm cuối cùng. |
| Cảm nhận nhanh | **Workflow:** AI đề xuất → giáo viên kiểm tra → ghi nhận xét. |

```text
HIỆN TẠI — giả định 5 phút/bài

[1 Xem đề + tiêu chí chấm: 0,5'] → [2 Đọc lời giải: 1']
→ [3 Tìm bước sai + loại lỗi: 2'] ← BOTTLENECK
→ [4 Viết hướng dẫn sửa: 1'] → [5 Kiểm tra nhận xét: 0,5']
```

### Problem Card #2 — Tìm lại kiến thức trong video bài giảng

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài tập, tôi muốn tìm đúng đoạn giảng viên giải thích công thức, để tiếp tục làm bài mà không phải tua nhiều đoạn. |
| Actor | Sinh viên học qua video bài giảng Toán. |
| Thời điểm / bối cảnh | Video 90 phút có transcript nhưng công thức trên bảng/slide không được đọc đầy đủ; người học không nhớ mốc thời gian. |
| Quy trình hiện tại | Xác định nội dung → tìm transcript → tua video → xem để xác nhận → lưu mốc thời gian. |
| Bottleneck | Bước 3: tua và quan sát bảng/slide, khoảng **4/7 phút/lần tìm**. |
| Impact | Gián đoạn làm bài; khoảng **7 phút/lần × 6 lần = 42 phút/tháng/sinh viên**. |
| Success metric | **7 → ≤ 2 phút/lần**, tính đến khi xác nhận đúng đoạn. Với 20 yêu cầu có đoạn tham chiếu, ít nhất **18/20** có phần giải thích đúng trong 3 kết quả đầu. Ghi riêng thời gian và chi phí lập chỉ mục. |
| Phương án không dùng AI | Mục lục theo thời gian, tiêu đề slide, danh mục công thức và bookmark. |
| Giả thuyết về AI | Dùng transcript và khung hình để tìm đoạn, trả mốc thời gian cùng hình liên quan. Người học mở để xác nhận; thiếu căn cứ thì báo chưa tìm thấy. |
| Cảm nhận nhanh | **Workflow:** lập chỉ mục → tìm đoạn → người học xác nhận. Chọn **No AI/Rule** nếu mục lục đã đủ. |

```text
HIỆN TẠI — giả định 7 phút/lần tìm

[1 Xác định nội dung: 0,5'] → [2 Tìm transcript: 1']
→ [3 Tua video + xem bảng/slide: 4'] ← BOTTLENECK
→ [4 Xác nhận đúng đoạn: 1'] → [5 Lưu mốc thời gian: 0,5']
```

### Problem Card #3 — Chuẩn hóa đơn hàng bán sỉ

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận đơn qua tin nhắn, ảnh hoặc ghi âm, tôi muốn xác định đúng mã hàng, số lượng và đơn vị, để tránh nhập sai và giao nhầm. |
| Actor | Nhân viên nhập đơn của nhà phân phối thực phẩm. |
| Thời điểm / bối cảnh | Đại lý đặt hàng không theo biểu mẫu, dùng tên tắt hoặc nhắc đơn cũ; thử trong một nhóm sản phẩm. |
| Quy trình hiện tại | Gom yêu cầu → đọc/nghe → tra mã hàng → hỏi lại → nhập đơn → đối chiếu. |
| Bottleneck | Bước 3: tra mã hàng, đơn vị và lịch sử, khoảng **1,5/4 phút thao tác/đơn**; chưa tính chờ đại lý. |
| Impact | Chậm nhập đơn, dễ nhầm hàng; **60 đơn × 26 ngày × 4 phút = 104 giờ/tháng**. |
| Success metric | **4 → ≤ 2 phút thao tác/đơn**, gồm duyệt và sửa. Thử trên 30 đơn có nhãn đối chiếu: ít nhất **95% dòng hàng** đúng đồng thời mã, số lượng và đơn vị; dòng thiếu/mâu thuẫn phải hỏi lại. |
| Phương án không dùng AI | Biểu mẫu đặt hàng, bảng tên gọi–mã hàng và Excel kiểm tra đơn vị. |
| Giả thuyết về AI | Trích xuất dòng hàng, đề xuất mã theo danh mục và lịch sử. Thiếu căn cứ thì hỏi lại; nhân viên duyệt trước khi xuất đơn. |
| Cảm nhận nhanh | **Workflow:** AI trích xuất → Rule kiểm tra → nhân viên duyệt. **Rule** có thể đủ khi dùng biểu mẫu chuẩn. |

```text
HIỆN TẠI — giả định 4 phút thao tác/đơn, chưa tính chờ trả lời

[1 Gom yêu cầu: 0,25'] → [2 Đọc/nghe: 0,75']
→ [3 Tra mã hàng + đơn vị + lịch sử: 1,5'] ← BOTTLENECK
→ [4 Soạn câu hỏi nếu cần: 0,25'] → [5 Nhập đơn: 0,75']
→ [6 Đối chiếu: 0,5']
```

### Card muốn pitch nhất

- **Card số:** #2 — Tìm lại kiến thức trong video bài giảng.
- **Vì sao:** Phạm vi rõ, gần bối cảnh học tập; đo được thời gian tìm và độ đúng của đoạn.
- **Câu hỏi muốn nhóm phản biện:** Mục lục đã đủ chưa? Thời gian tiết kiệm có bù công sức lập chỉ mục không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Thời gian và tần suất tìm chưa được đo. | Đồng ý | Ghi rõ là giả định; bỏ ước tính suy rộng cho 150 học viên. |
| Chưa chứng minh cần AI. | Đồng ý | Thêm phương án mục lục/bookmark và lựa chọn No AI/Rule. |
| Có công thức chưa chắc có đúng phần giải thích. | Đồng ý | Yêu cầu đoạn chứa phần giải thích; đo đến lúc người học xác nhận. |
| Mẫu thử nhỏ và chưa tính chi phí lập chỉ mục. | Đồng ý một phần | Giới hạn kết luận ở thử nghiệm ban đầu; thêm yêu cầu đo thời gian và chi phí lập chỉ mục. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

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

## Tài liệu tham khảo

- [EduVidQA — EMNLP 2025](https://aclanthology.org/2025.emnlp-main.1760/): nghiên cứu hỏi–đáp dựa trên video bài giảng.
- [HublerX — From WhatsApp to SAP with zero re-entry](https://www.hublerx.ai/resources/case-study/gcc-food-wholesale-distributor-sap-quote-order-workflow): case study do nhà cung cấp công bố về tiếp nhận và nhập đơn hàng.

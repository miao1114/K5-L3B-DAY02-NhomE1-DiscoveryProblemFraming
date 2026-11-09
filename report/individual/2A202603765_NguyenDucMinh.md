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
| Pitch Problem Card | Đưa ra 3 card: tìm bước giải sai, tìm kiến thức trong video và chuẩn hóa đơn bán sỉ. Card tôi muốn pitch nhất là tìm kiến thức trong video. | Card #2 được nhóm chọn để phân tích tiếp; nội dung tổng hợp ở mục 2.1 báo cáo nhóm. |
| Phản biện bài của bạn khác | Chưa ghi lại câu hỏi cụ thể tôi đã trực tiếp đặt; cần tự bổ sung theo buổi thảo luận. | Các câu hỏi tham khảo trong báo cáo nhóm chưa được tính là câu hỏi do tôi đã đặt. |
| Nhận phản biện | Báo cáo nhóm ghi nhận lo ngại về chi phí xây dựng và vận hành AI cho card chấm toán. Bảng phản biện AI ở mục 3 cũng chỉ ra baseline chưa đo và chưa chứng minh cần AI. | Giữ số liệu ở dạng giả định, thêm phương án không dùng AI và yêu cầu kiểm tra kết quả. Câu hỏi nguyên văn nhận từ bạn khác chưa được ghi lại. |
| Gom cluster / cây OST | Tổng hợp 12 candidate thành 4 cluster ở mục 2.2; trình bày OST cho bài toán tìm kiến thức trong video ở mục 2.3. | Tách nhu cầu tìm đúng đoạn khỏi các ý giải pháp như chatbot hay tự tạo mục lục. |
| Chọn candidate problem | Tổng hợp bảng shortlist, lý do chọn và lý do chưa chọn các hướng khác ở mục 2.4. | Nhóm chọn bài toán video vì gần bối cảnh học tập và có thể giới hạn phạm vi thử nghiệm. |
| Kiểm chứng / research | Dùng tài liệu tham khảo trong báo cáo để nêu rủi ro kỹ thuật ở mục 8. Chưa có dữ liệu phỏng vấn hoặc khảo sát được cập nhật ở mục 3. | Giữ kết luận ở mức cần kiểm chứng, chưa khẳng định người dùng thật sự cần giải pháp AI. |
| Quy trình nhóm | Tổng hợp phần quy trình CP5 do Hùng chuẩn bị vào báo cáo chính và cập nhật phân công trong TEAM.md. | Báo cáo có As-Is/To-Be, bảng Before/After và hai ảnh quy trình; phần trực tiếp xây dựng CP5 được ghi nhận cho Hùng. |
| Problem Statement | Theo phân công, tôi tổng hợp báo cáo; chưa có đóng góp riêng được ghi nhận ở phần viết Problem Statement. | Mục 5 và 7 vẫn cần hoàn thiện, đối chiếu với quy trình và metric. |
| Mức can thiệp AI | Trong phần quyết định, giữ yêu cầu so sánh phương án AI với mục lục và bookmark trước khi xây dựng. | Workflow ở CP5 là đề xuất; phần so sánh đầy đủ tại CP6 do Hà phụ trách và chưa hoàn thiện. |
| Quyết định | Tổng hợp 4 rủi ro, kết luận Not Yet, bước tiếp theo và ngưỡng dừng ở mục 8. | Chưa xây sản phẩm ngay; đề xuất kiểm chứng nhu cầu và thử khả năng tìm đúng đoạn trước. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Dùng AI hỗ trợ diễn đạt và phân loại 6 ý. | Giúp viết rõ người gặp vấn đề và việc họ muốn làm. | Ý quá rộng và số liệu ước lượng chưa chứng minh pain thật. | Bỏ ý “trợ lý quản lý mọi thông báo”, ghi rõ số liệu chưa đo thực tế. |
| CP2 Problem Card | Dùng AI phản biện 3 card và rà soát cách đo. | Chỉ ra thiếu sót về baseline, độ đúng và phương án không dùng AI. | Dễ coi tìm được hình công thức là đã tìm đúng phần giải thích; chưa tính công lập chỉ mục. | Bổ sung người học xác nhận, ghi riêng công lập chỉ mục và giữ lựa chọn No AI/Rule. |
| CP4 Research | Chưa có nhật ký riêng về việc dùng AI cho research CP4. | Chưa ghi nhận. | Chưa có dữ liệu kiểm chứng người dùng để kết luận. | Không điền kết quả phỏng vấn hoặc khảo sát khi chưa có bằng chứng. |
| CP5 Quy trình | Nhờ AI tích hợp phần CP5 của Hùng vào báo cáo chung và đối chiếu nội dung. | Giúp ghép đúng mục 4.1–4.3 và kiểm tra liên kết ảnh. | Sau khi ghép, bảng phân công cũ vẫn chưa khớp phần Hùng làm. | Yêu cầu sửa TEAM.md: Hùng phụ trách quy trình CP5, hỗ trợ CP3; hai phần chưa có người nhận được ghi cần phân công lại. |
| CP5–6 Problem Statement | Chưa có đóng góp hoặc nhật ký dùng AI riêng cho phần này. | Chưa ghi nhận. | Bảng v0 và v1 trong báo cáo chung còn trống. | Chưa ghi phần này là đã hoàn thành; cần nhóm tự viết và chốt. |
| CP6 Mức can thiệp / quyết định | Dùng AI hỗ trợ rà soát lập luận và cách trình bày phần quyết định. | Giúp sắp xếp 4 rủi ro, bước tiếp theo và ngưỡng dừng. | Có nghiên cứu liên quan chưa đủ chứng minh giải pháp của nhóm làm được; số liệu thử nghiệm vẫn chưa có. | Giữ kết luận Not Yet, yêu cầu so sánh với mục lục/bookmark và ghi các ngưỡng là mục tiêu thử nghiệm. |
| Bổ sung báo cáo cá nhân | Nhờ AI soạn bản nháp mục 4, 5 và 6 bằng cách viết đơn giản, dựa trên nội dung trong repo. | Giúp tổng hợp phần việc và diễn đạt ngắn gọn. | AI không biết đầy đủ trải nghiệm của tôi hoặc câu hỏi thực tế trong buổi thảo luận. | Tôi cần tự đọc lại bản nháp, sửa theo trải nghiệm thật và bổ sung những chỗ chưa ghi nhận. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Qua các các problems của các bạn tôi nhận ra được khá nhiều ấn đề. Có những vấn đề có ở hiện tại nhưng con người vẫn đang giải quyết nhưng nhiều nơi lại thấy Ai là không cần thiết cho vấn đề đó. Có những vấn đề tồn đọng nhưng ChatBot AI vẫn có thể làm được việc đó.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có một số problems khi nói ra bọn em đã nhìn ra ngay giải pháp non AI mà không cần thực sự phải sử dụng AI. Sau đó bọn em trao đổi và cho rằng vấn đề này không thực sự phải áp dụng AI vào để cải thiện quá nhiều.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Mới đầu bọn em chọn dự án Tối ưu hóa đơn từ nhiều nguồn cho công ty nó là vấn đề thực tế mà gia đình của một bạn trong nhóm gặp phải. Nhưng sau khi tìm hiểu bọn em đã thấy có một số giải pháp có sẵn ở trên mạng nhưng nhiều công ty chưa thực sự áp dụng vào và vận hành nó.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Khi khảo sát em thấy hiện tượng thực sự không quá cao như em nghĩ vì đa số mọi người khi quên công thức đó thì ngay lúc đó họ vẫn có thể hình dung rằng thanh thời gian ở đoạn nào từ đó sẽ xem lại nhanh hơn. Chứ chưa phải họ cần dùng đến nó họ quên và cần tìm vid để học lại.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Theo em, khó nhất là xác định vấn đề có thực sự gây mất thời gian không và đo bằng cách nào. Mốc 7 phút chưa được đo thực tế, còn 2 phút chỉ là mục tiêu. Vì vậy, cần đo cả thời gian tìm và việc người học có tìm đúng đoạn cần xem không.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, em sẽ khảo sát và quan sát cách mọi người tìm video sớm hơn để biết nhu cầu có đủ lớn không. Em cũng sẽ hỏi nhóm kỹ hơn xem mục lục, bookmark đã đủ chưa và dùng AI có thực sự tiết kiệm thời gian hơn không.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán nhóm em chọn là tìm lại công thức và phần giải thích trong video bài giảng dài. Người học thường tìm transcript, tua video, kiểm tra đoạn rồi lưu mốc; bước nghẽn dự kiến là tua khi transcript thiếu công thức. Mốc 7 phút chưa được đo, còn mục tiêu là tìm đúng trong 2 phút, gồm kiểm tra, và đạt 18/20 yêu cầu trong 3 kết quả đầu. Hệ thống chỉ dùng video được phép sử dụng, không tự tạo công thức hay mốc thời gian và phải để người học kiểm tra. Nhóm đề xuất Workflow kết hợp AI và Rule nhưng vẫn cần so sánh với mục lục, bookmark. Hiện nhóm chọn Not Yet vì chưa đủ bằng chứng về nhu cầu và khả năng làm được, nên cần kiểm chứng thêm trước khi xây sản phẩm.

---

## Tài liệu tham khảo

- [EduVidQA — EMNLP 2025](https://aclanthology.org/2025.emnlp-main.1760/): nghiên cứu hỏi–đáp dựa trên video bài giảng.
- [HublerX — From WhatsApp to SAP with zero re-entry](https://www.hublerx.ai/resources/case-study/gcc-food-wholesale-distributor-sap-quote-order-workflow): case study do nhà cung cấp công bố về tiếp nhận và nhập đơn hàng.

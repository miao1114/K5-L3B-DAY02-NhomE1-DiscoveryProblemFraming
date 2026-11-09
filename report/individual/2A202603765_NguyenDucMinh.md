# Báo cáo cá nhân — 2A202603765_NguyenDucMinh

## 1. Thông tin học viên

- Họ tên: Nguyễn Đức Minh
- MSSV: 2A202603765
- Tên nhóm: Nhóm E1
- Link repo nhóm: https://github.com/miao1114/K5-L3B-DAY02-NhomE1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

**Cơ sở:** 6 tình huống tham khảo và nguồn nghiên cứu liên quan. Số liệu thời gian, quy mô và bottleneck là **giả định chưa đo thực tế**; target là mục tiêu đề xuất.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian; Pain từ người khác | **Tìm bước giải sai trong bài toán viết tay.** Khi chấm bài giải phương trình bậc hai viết tay của học sinh, tôi muốn xác định bước đầu tiên em làm sai và phân biệt lỗi tính toán với lỗi tư duy, để phản hồi đúng nguyên nhân và hướng dẫn em sửa bài. | Giáo viên Toán THCS; học sinh nhận phản hồi. | Phải đọc từng bước và đối chiếu rubric, kể cả cách giải khác mẫu. Ước tính **30 bài × 5 phút = 150 phút/đợt**; phạm vi ban đầu: **1 dạng bài**, phương trình bậc hai. |
| 2 | Tốn thời gian | **Tìm lại đoạn kiến thức trong video bài giảng dài.** Khi làm bài tập và cần xem lại cách giảng viên giải thích một công thức trong video 90 phút, tôi muốn tìm đúng đoạn có công thức cùng phần giải thích liên quan, để tiếp tục làm bài mà không phải tua và xem lại từng đoạn. | Sinh viên học qua video; học viên khóa học trực tuyến. | Công thức chỉ hiện trên bảng/slide và không được đọc đầy đủ nên tìm từ khóa trong transcript không ra. **Giả định minh họa:** 150 học viên × 6 lần tìm/tháng × 7 phút/lần = **105 giờ/tháng** cho cả nhóm. [EduVidQA](https://aclanthology.org/2025.emnlp-main.1760/) có **5.252 cặp hỏi–đáp từ 296 video khoa học máy tính**, cung cấp bối cảnh nghiên cứu liên quan, chưa xác nhận thời gian tìm kiếm nêu trên. |
| 3 | Lặp lại; Cần đọc, tổng hợp nhiều thông tin | **Chuẩn hóa đơn hàng bán sỉ từ tin nhắn, ảnh và ghi âm.** Khi nhận yêu cầu đặt hàng của đại lý qua nhiều dạng tin nhắn với tên gọi tắt hoặc nhắc lại đơn cũ, tôi muốn xác định đúng mã sản phẩm, số lượng và đơn vị tính, để nhập đơn đầy đủ và tránh giao nhầm hàng. | Nhân viên nhập đơn/bán hàng của nhà phân phối thực phẩm; đại lý; bộ phận kho. | Nhân viên phải đọc tin nhắn, xem ảnh, nghe ghi âm rồi tra mã và nhập lại vào phần mềm. [Case study HublerX](https://www.hublerx.ai/resources/case-study/gcc-food-wholesale-distributor-sap-quote-order-workflow) mô tả đơn hàng qua WhatsApp/email và thao tác nhập lại vào SAP; đây là thông tin do nhà cung cấp công bố. **Giả định minh họa:** 60 đơn/ngày × 26 ngày/tháng × 4 phút/đơn = **104 giờ/tháng**. |
| 4 | Lặp lại; Pain từ người khác | **Bỏ lỡ thông báo quan trọng trong nhóm Zalo lớp.** Khi theo dõi nhiều nhóm Zalo của hai con đang học tiểu học, tôi muốn biết thông báo nào cần hành động, áp dụng cho con nào và hạn khi nào, để chuẩn bị đúng đồ dùng, nộp bài hoặc đóng khoản phí đúng hạn. | Phụ huynh có con học tiểu học; học sinh; giáo viên phải nhắc lại thông báo. | Tình huống trong ảnh gồm hạn nộp bài Mỹ thuật, mặc đồng phục thể dục, đóng tiền tham quan và đổi lịch học; phụ huynh phải tự đọc, lọc rồi ghi chú. **Giả định minh họa:** 10 phút/ngày × 22 ngày học/tháng = **220 phút, tức 3 giờ 40 phút/tháng/phụ huynh**. Chưa có nhật ký sử dụng hay số lần bỏ lỡ thông báo thực tế. |
| 5 | Lặp lại | **Nhập lại chỉ số điện nước từ ảnh đồng hồ.** Khi chốt tiền điện nước cuối tháng cho khu trọ 40 phòng, tôi muốn đối chiếu chính xác chỉ số trong ảnh với phòng và kỳ trước, để tính đúng mức tiêu thụ, lập bảng thanh toán và có căn cứ giải thích khi người thuê thắc mắc. | Chủ trọ/người quản lý; người thuê của 40 phòng. | Quy trình hiện tại: mở ảnh → đọc số → nhập Excel → trừ chỉ số kỳ trước → tính tiền từng phòng; nhập sai một chữ số có thể gây tranh chấp. **Giả định minh họa:** 40 phòng × 2 đồng hồ/phòng × 2 phút đọc và nhập/đồng hồ + 40 phòng × 3 phút tính và lập bảng/phòng = **280 phút, khoảng 4,7 giờ/tháng**; chưa tính thời gian đi chụp ảnh. |
| 6 | Tốn thời gian; Cần đọc, tổng hợp nhiều thông tin | **Tổng hợp yêu cầu chỉnh sửa video từ khách hàng.** Khi khách hàng gửi phản hồi cho bản dựng qua tin nhắn, ghi âm và ảnh chụp, rồi tiếp tục thay đổi yêu cầu, tôi muốn có danh sách chỉnh sửa mới nhất gắn với đúng mốc thời gian, để sửa đủ việc và tránh làm theo yêu cầu đã bị hủy. | Freelancer dựng video TikTok/quảng cáo; khách hàng duyệt bản dựng. | Trong tình huống tham khảo, phản hồi gồm rút ngắn phần mở đầu, sửa chữ tại 00:35, đổi font theo ảnh và sau đó hủy yêu cầu đổi nhạc; người dựng phải đối chiếu thứ tự phản hồi. **Giả định minh họa:** 15 video/tháng × 20 phản hồi/video × 2 phút đọc, xác định mốc thời gian và chuẩn hóa/phản hồi = **600 phút, tức 10 giờ/tháng**. Chưa đo trên dự án thực tế. |

**Dùng AI:** Chuẩn hóa Job Story, phân loại lăng kính, kiểm tra phép tính và tìm nguồn tham khảo. Giữ 6 vấn đề cụ thể; bỏ cách diễn đạt quá rộng như “AI chấm bài” và “trợ lý quản lý mọi thông báo”.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tìm bước giải sai trong bài toán viết tay (#1) | Actor rõ; có thể giới hạn ở phương trình bậc hai; kết quả đối chiếu được với giáo viên qua bước sai đầu tiên và loại lỗi. | Đọc chữ viết tay có đủ chính xác không? Giáo viên có thống nhất bước sai và loại lỗi không? Có thu thập được bài mẫu và rubric không? |
| 2 | Tìm lại đoạn kiến thức trong video bài giảng dài (#2) | Pain cụ thể khi công thức chỉ xuất hiện trên hình; đo được thời gian tìm và mức độ đúng của đoạn trả về. | Mục lục và transcript có sẵn đã đủ chưa? Có truy cập được video và xác định được đoạn đúng để đánh giá không? |
| 3 | Chuẩn hóa đơn hàng bán sỉ từ tin nhắn, ảnh và ghi âm (#3) | Công việc lặp lại; có trường dữ liệu rõ là SKU, số lượng, đơn vị; có thể so sánh với biểu mẫu đặt hàng chuẩn. | Đại lý có chấp nhận dùng biểu mẫu không? Có danh mục SKU, quy đổi đơn vị và lịch sử đơn hàng không? |

### Problem Card #1 — Tìm bước giải sai trong bài toán viết tay

| Trường | Nội dung |
|---|---|
| Job Story | Khi chấm bài giải phương trình bậc hai viết tay của học sinh, tôi muốn xác định bước đầu tiên em làm sai và phân biệt lỗi tính toán với lỗi tư duy, để phản hồi đúng nguyên nhân và hướng dẫn em sửa bài. |
| Actor | Giáo viên Toán THCS đang chấm bài tự luận về phương trình bậc hai. |
| Thời điểm / bối cảnh | Sau bài tập hoặc bài kiểm tra; giáo viên có đề, bài giải viết tay và rubric, nhưng học sinh có thể dùng cách giải khác đáp án mẫu. Phạm vi ban đầu chỉ gồm bài giải phương trình bậc hai một ẩn trên ảnh rõ, đủ trang. |
| Quy trình hiện tại (3–7 bước) | 1. Xem đề và rubric · 2. Đọc các dòng lời giải · 3. Kiểm tra từng phép biến đổi để tìm bước sai đầu tiên và phân loại lỗi · 4. Viết giải thích, gợi ý sửa · 5. Kiểm tra lại và ghi nhận xét. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 3 mất **2 phút/bài** trong tổng **5 phút/bài**, vì phải kiểm tra tính hợp lệ của từng bước, kể cả cách giải khác mẫu. Cần bấm giờ để xác nhận thay vì mặc định đây là bước tốn nhất. |
| Impact (nếu không giải thì sao) | Phản hồi chậm, thiếu giải thích nguyên nhân hoặc đánh dấu sai cách giải hợp lệ. Ước tính **30 bài × 5 phút = 150 phút/đợt** chấm và nhận xét. |
| Success metric (baseline → target) | Baseline chưa đo; giả định **5 → không quá 3 phút/bài**, gồm thời gian giáo viên duyệt. Thử trên 30 bài chưa dùng để chỉnh prompt: ít nhất **90%** bài có lỗi được xác định đúng bước sai đầu tiên theo nhãn giáo viên; ít nhất **90%** đúng loại lỗi theo rubric; không đánh dấu sai bài đúng trong mẫu thử. Ghi riêng số bài ảnh khó đọc phải chuyển về xử lý thủ công. |
| Phương án không dùng AI | Rubric theo từng phép biến đổi, danh mục lỗi thường gặp và mẫu nhận xét; yêu cầu học sinh trình bày mỗi bước trên một dòng. So sánh thời gian với phương án này trước khi kết luận cần AI. |
| Giả thuyết về AI (nếu có) | Từ ảnh, đề và rubric, AI đề xuất vị trí bước sai đầu tiên, loại lỗi và giải thích có trích lại dòng liên quan. Không ép lời giải theo đúng thứ tự đáp án mẫu. Giáo viên duyệt và sửa; ảnh không rõ hoặc thiếu ngữ cảnh thì yêu cầu kiểm tra thủ công, không tự chấm điểm cuối cùng. |
| Cảm nhận nhanh | **Workflow (giả thuyết):** nhận dữ liệu → AI đề xuất → giáo viên kiểm tra → ghi nhận xét. Cần so sánh với rubric và mẫu nhận xét trước khi chốt. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — giả định 5 phút/bài; 30 bài = 150 phút/đợt

[1 Xem đề + rubric: 0,5'] → [2 Đọc lời giải: 1']
→ [3 Tìm bước sai đầu tiên + phân loại lỗi: 2'] ← BOTTLENECK GIẢ ĐỊNH
→ [4 Viết giải thích + gợi ý sửa: 1'] → [5 Kiểm tra + ghi nhận xét: 0,5']
```

### Problem Card #2 — Tìm lại đoạn kiến thức trong video bài giảng dài

| Trường | Nội dung |
|---|---|
| Job Story | Khi làm bài tập và cần xem lại cách giảng viên giải thích một công thức trong video 90 phút, tôi muốn tìm đúng đoạn có công thức cùng phần giải thích liên quan, để tiếp tục làm bài mà không phải tua và xem lại từng đoạn. |
| Actor | Sinh viên đang làm bài tập từ một video bài giảng Toán có transcript nhưng chưa có mục lục chi tiết. |
| Thời điểm / bối cảnh | Sinh viên nhớ công thức xuất hiện trên bảng/slide nhưng không nhớ mốc thời gian; transcript không chứa đầy đủ công thức. Phạm vi ban đầu: một video 90 phút mà người học có quyền sử dụng. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định công thức/nội dung cần tìm · 2. Tìm từ khóa trong transcript · 3. Tua video và quan sát bảng/slide khi tìm từ khóa không ra · 4. Xem đoạn nghi ngờ để xác nhận có đúng phần giải thích cần tìm · 5. Ghi mốc thời gian và quay lại bài tập. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 3 mất **4 phút/lần** trong tổng **7 phút/lần**, do phải xem hình ở nhiều mốc thời gian khi transcript không chứa công thức. |
| Impact (nếu không giải thì sao) | Gián đoạn làm bài, mất thời gian tìm hoặc bỏ qua phần giải thích cần thiết. Theo giả định ở CP1: **6 lần/tháng × 7 phút = 42 phút/tháng/sinh viên**; 150 sinh viên tương đương **105 giờ/tháng**. Chưa xác nhận quy mô này bằng khảo sát. |
| Success metric (baseline → target) | Baseline chưa đo; giả định **7 → không quá 2 phút/lần tìm**, tính đến khi người học xác nhận đúng đoạn. Với 20 câu hỏi có đoạn tham chiếu do người xem gán trước, ít nhất **18/20** câu có đoạn đúng trong 3 kết quả đầu; đoạn đúng phải chứa phần giải thích cần tìm, không chỉ có hình công thức. Ghi riêng thời gian và chi phí lập chỉ mục ban đầu. |
| Phương án không dùng AI | Bổ sung mục lục theo mốc thời gian, tiêu đề slide, danh mục công thức và bookmark cá nhân; dùng tìm kiếm transcript hiện có. Kiểm tra xem mục lục chi tiết có giải quyết phần lớn nhu cầu hay không. |
| Giả thuyết về AI (nếu có) | Phân tích transcript cùng khung hình bảng/slide để lập chỉ mục theo thời gian; khi nhận câu hỏi, trả về tối đa 3 đoạn kèm mốc bắt đầu–kết thúc và khung hình liên quan. Người học mở đoạn để xác nhận; khi không có căn cứ thì báo chưa tìm thấy. |
| Cảm nhận nhanh | **Workflow (giả thuyết):** lập chỉ mục → tìm đoạn → hiển thị căn cứ → người học xác nhận. Có thể chọn **No AI/Rule** nếu mục lục và tìm kiếm từ khóa đã đủ. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — giả định 7 phút/lần tìm khi transcript không đủ

[1 Xác định nội dung cần tìm: 0,5'] → [2 Tìm transcript: 1']
→ [3 Tua video + quan sát bảng/slide: 4'] ← BOTTLENECK GIẢ ĐỊNH
→ [4 Xem và xác nhận đúng phần giải thích: 1'] → [5 Ghi mốc + quay lại bài: 0,5']
```

### Problem Card #3 — Chuẩn hóa đơn hàng bán sỉ từ tin nhắn, ảnh và ghi âm

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận yêu cầu đặt hàng của đại lý qua tin nhắn, ảnh hoặc ghi âm với tên gọi tắt hay nhắc lại đơn cũ, tôi muốn xác định đúng mã sản phẩm, số lượng và đơn vị tính, để nhập đơn đầy đủ và tránh giao nhầm hàng. |
| Actor | Nhân viên tiếp nhận và nhập đơn bán sỉ của một nhà phân phối thực phẩm. |
| Thời điểm / bối cảnh | Trong ngày làm việc, đại lý gửi yêu cầu không theo biểu mẫu, ví dụ “3 thùng sữa loại hôm trước”. Nhân viên có danh mục SKU, quy đổi đơn vị và lịch sử đơn hàng. Phạm vi thử ban đầu: một nhà phân phối, một nhóm sản phẩm; chưa tích hợp ghi đơn trực tiếp vào hệ thống bán hàng. |
| Quy trình hiện tại (3–7 bước) | 1. Gom tin nhắn, ảnh và ghi âm thuộc cùng yêu cầu · 2. Đọc/nghe để tách các dòng hàng · 3. Tra tên gọi, ảnh hoặc lịch sử để xác định SKU và đơn vị · 4. Hỏi lại đại lý khi thiếu hoặc mâu thuẫn thông tin · 5. Nhập đơn vào phần mềm · 6. Đối chiếu lại trước khi chuyển xử lý. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 3 mất **1,5 phút/đơn** trong tổng **4 phút thao tác/đơn**, do tên gọi không trùng mã hàng và đơn vị thùng/lốc/hộp có thể khác nhau. Thời gian chờ đại lý trả lời được đo riêng, không nằm trong 4 phút này. |
| Impact (nếu không giải thì sao) | Nhập chậm, nhầm SKU hoặc số lượng/đơn vị dẫn tới sửa đơn và giao sai. Theo giả định CP1: **60 đơn/ngày × 26 ngày × 4 phút = 104 giờ thao tác/tháng** cho tổng lượng đơn; chưa có số đo tỷ lệ nhập sai và chi phí xử lý lỗi. |
| Success metric (baseline → target) | Baseline chưa đo; giả định **4 → không quá 2 phút thao tác/đơn**, gồm kiểm tra và sửa bản nháp. Trên 30 đơn thử đã có nhãn đối chiếu, ít nhất **95% dòng hàng** khớp đồng thời SKU, số lượng và đơn vị; tất cả trường hợp được gán nhãn thiếu/mâu thuẫn thông tin phải được yêu cầu xác nhận. Đo riêng thời gian chờ; chỉ xuất đơn đã được nhân viên duyệt. |
| Phương án không dùng AI | Biểu mẫu đặt hàng có danh mục SKU và đơn vị cố định; bảng ánh xạ tên thường gọi; file Excel kiểm tra trường bắt buộc và quy đổi đơn vị theo quy tắc. Nếu đại lý chấp nhận biểu mẫu, ưu tiên thử cách này trước. |
| Giả thuyết về AI (nếu có) | Trích xuất dòng hàng từ tin nhắn, ảnh và ghi âm, đề xuất SKU dựa trên danh mục và lịch sử được cung cấp, gắn căn cứ từ nội dung gốc. Không tự đoán khi “loại hôm trước” chưa có lịch sử để đối chiếu. Nhân viên xác nhận dòng chưa rõ, duyệt rồi xuất bảng đơn có cấu trúc; quy đổi đơn vị và kiểm tra tồn kho dùng dữ liệu/quy tắc của hệ thống. |
| Cảm nhận nhanh | **Workflow (giả thuyết):** gom yêu cầu → AI trích xuất/đề xuất SKU → Rule kiểm tra → nhân viên duyệt → xuất đơn. **Rule** có thể đủ nếu đầu vào được chuẩn hóa bằng biểu mẫu. |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — giả định 4 phút thao tác/đơn; chưa tính chờ đại lý

[1 Gom nội dung cùng đơn: 0,25'] → [2 Đọc/nghe, tách dòng hàng: 0,75']
→ [3 Tra SKU + đơn vị + lịch sử: 1,5'] ← BOTTLENECK GIẢ ĐỊNH
→ [4 Soạn câu hỏi xác nhận nếu cần: 0,25']
→ [5 Nhập phần mềm: 0,75'] → [6 Đối chiếu lại: 0,5']

Thời gian chờ trả lời: ghi riêng khi có phát sinh.
Các thời lượng là giả định trung bình phân bổ trên mỗi đơn.
```
### Card muốn pitch nhất

- **Card số:** #2 — Tìm lại đoạn kiến thức trong video bài giảng dài.
- **Vì sao:** Tình huống cụ thể: sinh viên cần tìm lại phần giải thích công thức nhưng transcript không chứa đầy đủ nội dung trên bảng/slide. Có thể giới hạn thử nghiệm ở một video 90 phút và đo thời gian tìm, độ đúng của đoạn trả về.
- **Câu hỏi muốn nhóm phản biện:** Thế nào là tìm đúng phần giải thích, và thời gian tiết kiệm có bù được công sức lập chỉ mục video không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Thời gian 7 phút/lần và tần suất 6 lần/tháng chưa được đo thực tế. | Đồng ý | Ghi rõ số liệu là giả định, baseline chưa đo; bổ sung hướng kiểm chứng bằng quan sát thao tác và tách thời gian tìm đoạn khỏi thời gian học lại kiến thức. |
| Ước tính 105 giờ/tháng giả định cả 150 học viên đều gặp vấn đề với cùng tần suất. | Đồng ý | Ghi impact là ước tính chưa được khảo sát xác nhận; cần đo tỷ lệ người thực sự gặp vấn đề trước khi suy rộng cho cả lớp. |
| Chưa chứng minh cần AI vì mục lục và bookmark có thể đã đủ. | Đồng ý | Bổ sung phương án không dùng AI gồm mục lục, tiêu đề slide và bookmark; giữ lựa chọn No AI/Rule nếu các cách này đáp ứng nhu cầu. |
| Tìm thấy hình công thức chưa chắc tìm đúng phần giải thích cần xem. | Đồng ý | Làm rõ tiêu chí: đoạn trả về phải chứa phần giải thích liên quan; đo thời gian đến khi người học xác nhận đúng đoạn, không chỉ đến khi có kết quả. |
| Một video và 20 câu hỏi chưa đủ để khái quát cho nhiều bài giảng. | Đồng ý một phần | Giữ mẫu này cho thử nghiệm ban đầu; bổ sung yêu cầu tách câu hỏi đánh giá khỏi câu hỏi dùng để điều chỉnh và mở rộng video nếu tiếp tục kiểm chứng. |
| Chưa tính công sức và chi phí lập chỉ mục video. | Đồng ý | Bổ sung yêu cầu ghi riêng thời gian, chi phí lập chỉ mục và đối chiếu với số lượt tìm thực tế để đánh giá lợi ích. |

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

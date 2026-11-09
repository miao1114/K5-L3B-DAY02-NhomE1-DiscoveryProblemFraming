# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm:
- Candidate problem nhóm chọn (1 câu):
- Quyết định cuối (Go / Not Yet / No-Go):

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | Phạm Thế Hùng | 2A202603778 | Phân tích quy trình CP5; hỗ trợ Leader ở CP3 | |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | Phạm Thế Hùng (theo phân công) | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | | | Assumption map, snapshot hoặc survey |
| CP4 — Research | | | Bảng research có link |
| CP5 — Quy trình trước/sau | Phạm Thế Hùng | | Mục 4.1–4.3; ảnh As-Is/To-Be; bảng Before/After |
| CP5 — Problem Statement v0 | | | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HoVaTen-MSSV

**Phần việc phụ trách:**

-

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

-

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

-

**Điều mình học được từ phần nhóm:**

-

### PhamTheHung-2A202603778

**Phần việc phụ trách:**

- Phụ trách CP5 — quy trình trước/sau, trực tiếp điền mục 4.1–4.3 của báo cáo nhóm.
- Hỗ trợ Leader gom problem và làm OST tại CP3 theo phân công;

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Dùng AI hỗ trợ triển khai bản nháp quy trình tìm lại công thức và phần giải thích trong video 90 phút: As-Is 5 bước, To-Be 4 bước; bổ sung actor, input/output, thời gian, bottleneck, bước người học kiểm tra, boundary và phương án quay về thủ công.
- Chuẩn bị hai ảnh quy trình và bảng Before/After.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo nhóm — mục 4.1–4.3](report/team/group_report.md#4-quy-trình-trướcsau-cp5).
- [Ảnh As-Is](report/assets/cp5-workflow-current.png) và [ảnh To-Be](report/assets/cp5-workflow-future.png).
- Nhật ký tham gia và sử dụng AI: mục 4–5 trong [báo cáo cá nhân](report/individual/2A202603778_PhamTheHung.md).

**Điều mình học được từ phần nhóm:**

- Quy trình cần được tách thành từng bước có actor, input, output và thời gian để chỉ rõ bước nghẽn; với bài toán này, cần kiểm chứng riêng thời gian tua video khi transcript không chứa đủ công thức trên bảng/slide.
- Tìm đúng hình công thức chưa đủ: kết quả cần có cả phần giải thích liên quan, mốc thời gian và nguồn video để người học mở lại kiểm tra.
- Quy trình cải thiện vẫn cần bước con người xác nhận và phương án quay về tìm thủ công khi kết quả sai hoặc hệ thống lỗi. Thời gian kiểm tra phải được tính vào tổng thời gian tìm.

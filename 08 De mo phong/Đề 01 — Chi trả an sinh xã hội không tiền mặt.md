# Đề mô phỏng 01 — Bài toán liên ngành: chi trả an sinh xã hội không dùng tiền mặt

**Thời gian: 90 phút. Sản phẩm nộp: (1) Tờ trình/báo cáo tham mưu (.docx), (2) file bảng tính/dashboard (.xlsx), (3) slide 5 trang (.pptx). Thuyết trình 3 phút, hỏi đáp 5 phút.**

## Tình huống

Bạn là chuyên viên Phòng Khách hàng cá nhân, Chi nhánh X của một ngân hàng thương mại nhà nước tại một tỉnh có 9 huyện, thị. Chi nhánh được UBND tỉnh giao phối hợp với Sở Nội vụ (lĩnh vực lao động, người có công, xã hội) và Bảo hiểm xã hội tỉnh để chi trả trợ cấp an sinh xã hội hằng tháng qua tài khoản cho khoảng 38.000 đối tượng (người có công, bảo trợ xã hội, hưu trí). Hiện nay:

- Mới 61% đối tượng đã có tài khoản và nhận qua tài khoản; 39% còn nhận tiền mặt tại điểm chi trả của bưu điện, mỗi kỳ mất 3–5 ngày, phát sinh sai sót đối chiếu.
- Danh sách chi trả do cấp xã lập bằng Excel, gửi qua email lên Sở, Sở gửi ngân hàng; mỗi tháng ngân hàng nhận 9 file khác định dạng, cán bộ phải nhập lại và đối chiếu tay với Cơ sở dữ liệu dân cư, mất trung bình 6 ngày công/tháng, tỷ lệ hồ sơ sai (tên, số CCCD, tài khoản không khớp) khoảng 4–7%.
- Người cao tuổi ở vùng sâu không biết dùng ứng dụng, sợ mất tiền, thường xuyên gọi lên chi nhánh hỏi "tiền đã về chưa".
- Giám đốc chi nhánh muốn đề xuất UBND tỉnh một phương án nâng tỷ lệ chi trả qua tài khoản lên 90% trong 12 tháng, giảm sai sót, và sử dụng AI hỗ trợ khâu đối chiếu, giải đáp, theo dõi.

## Dữ liệu đề cho (12 tháng, toàn tỉnh) [số liệu mô phỏng]

| Tháng | Đối tượng phải chi trả | Nhận qua tài khoản | Hồ sơ sai phải trả lại | Ngày công đối chiếu | Cuộc gọi hỏi tiến độ | Khiếu nại |
|---|---|---|---|---|---|---|
| 09/2025 | 37.200 | 20.100 | 1.900 | 5,5 | 1.240 | 41 |
| 10/2025 | 37.300 | 20.600 | 2.100 | 5,8 | 1.310 | 44 |
| 11/2025 | 37.400 | 21.000 | 2.300 | 6,0 | 1.380 | 47 |
| 12/2025 | 37.600 | 21.300 | 2.600 | 6,5 | 1.520 | 55 |
| 01/2026 | 37.700 | 21.700 | 2.400 | 6,2 | 1.610 | 58 |
| 02/2026 | 37.800 | 22.000 | 1.800 | 5,4 | 1.150 | 36 |
| 03/2026 | 37.900 | 22.300 | 2.000 | 5,6 | 1.220 | 40 |
| 04/2026 | 38.000 | 22.600 | 2.200 | 5,9 | 1.290 | 43 |
| 05/2026 | 38.000 | 22.800 | 2.300 | 6,0 | 1.330 | 45 |
| 06/2026 | 38.100 | 23.000 | 2.500 | 6,3 | 1.400 | 49 |
| 07/2026 | 38.100 | 23.100 | 2.600 | 6,4 | 1.450 | 52 |
| 08/2026 | 38.200 | 23.300 | 2.700 | 6,6 | 1.480 | 54 |

## Yêu cầu

1. Phân rã bài toán: mục tiêu, đối tượng tác động (ít nhất 3 nhóm), ràng buộc pháp lý (chú ý dữ liệu cá nhân, bí mật thông tin khách hàng, chia sẻ dữ liệu liên ngành), dữ liệu cần dùng và mức nhạy cảm, tiêu chí đánh giá phương án có trọng số.
2. Đề xuất và so sánh ít nhất 3 phương án; sử dụng AI để hỗ trợ tổng hợp, so sánh; **trình bày rõ phần kiểm chứng và phản biện độc lập** đối với đầu ra của AI.
3. Phân tích số liệu trên bằng bảng tính/dashboard: ít nhất 5 chỉ số then chốt, ý nghĩa quản trị của từng chỉ số, ước tính hiệu quả phương án theo 3 kịch bản.
4. Xây dựng báo cáo tham mưu/tờ trình gửi Giám đốc chi nhánh để trình UBND tỉnh: phương án, nguồn lực, rủi ro, lộ trình 12 tháng, cơ chế phối hợp ba bên.
5. Đề xuất nguyên tắc triển khai AI an toàn tại chi nhánh cho bài toán này: phân quyền dữ liệu, kiểm soát đầu ra, lưu vết sử dụng, đào tạo người dùng.

## Gợi ý điểm khó của đề (tự đọc sau khi làm xong)

- Dữ liệu đối tượng an sinh là **dữ liệu cá nhân nhạy cảm** (tình trạng sức khoẻ, hoàn cảnh) + thông tin tài khoản → tuyệt đối không đưa danh sách lên AI công cộng; phương án phải có bước ẩn danh hoá hoặc AI nội bộ.
- "AI hỗ trợ đối chiếu" dễ bị viết thành "AI tự động duyệt danh sách chi trả" → sai nguyên tắc; đối chiếu là đề xuất, cán bộ xác nhận, Sở ký.
- Đối tượng tác động nhóm 1 (người cao tuổi vùng sâu) là lý do phương án phải có kênh không cần smartphone (SMS, điểm hỗ trợ, uỷ quyền).
- Phối hợp ba bên cần **quy chế chia sẻ dữ liệu**: ai là bên kiểm soát dữ liệu, chuẩn file, kênh truyền, trách nhiệm khi sai.
- Chỉ số "cuộc gọi hỏi tiến độ" chính là KPI cho phương án thông báo chủ động; đừng bỏ.

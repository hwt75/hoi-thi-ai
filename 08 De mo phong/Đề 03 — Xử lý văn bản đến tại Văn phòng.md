# Đề mô phỏng 03 — Công vụ chung: tổng hợp, phân loại và dự thảo xử lý văn bản đến tại Văn phòng

**Thời gian: 90 phút. Sản phẩm nộp: báo cáo đề xuất (.docx), bảng tính/dashboard (.xlsx), slide (.pptx). Thuyết trình 3 phút.**

Đề này cố tình **không** thuộc ngành ngân hàng, để luyện trường hợp đề liên ngành chung cho cả bảng Bộ, ban, ngành Trung ương.

## Tình huống

Văn phòng của một cơ quan cấp Tổng cục/Cục thuộc Bộ nhận trung bình 2.800 văn bản đến mỗi tháng qua Hệ thống quản lý văn bản và điều hành (liên thông trục văn bản quốc gia), email công vụ và bản giấy. Văn thư đăng ký, Chánh Văn phòng đọc và đề xuất phân công, lãnh đạo cơ quan bút phê, văn bản được chuyển về đơn vị chuyên môn. Vấn đề:

- Chánh Văn phòng mất 2–3 giờ/ngày đọc và tóm tắt văn bản để đề xuất phân công; 12% văn bản bị phân công sai đơn vị, phải chuyển lại.
- Văn bản có thời hạn xử lý (công văn xin ý kiến, kiến nghị cử tri, yêu cầu báo cáo) bị trễ hạn khoảng 15%, gây bị nhắc nhở.
- Nhiều văn bản trùng nội dung hoặc liên quan đến hồ sơ đã xử lý trước đó, cán bộ không tra được lịch sử.
- Khoảng 8% văn bản đến có độ mật hoặc nội bộ, không được đưa ra ngoài hệ thống.
- Lãnh đạo muốn ứng dụng AI để tóm tắt, gợi ý phân công, cảnh báo hạn, và tra cứu văn bản liên quan; đồng thời phải bảo đảm an toàn thông tin.

## Dữ liệu đề cho (12 tháng) [số liệu mô phỏng]

| Tháng | Văn bản đến | Có thời hạn | Trễ hạn | Phân công sai | Giờ Chánh VP dành cho phân loại | Văn bản mật/nội bộ | Văn bản trùng/liên quan hồ sơ cũ |
|---|---|---|---|---|---|---|---|
| 09/2025 | 2.650 | 1.120 | 150 | 300 | 52 | 210 | 380 |
| 10/2025 | 2.780 | 1.190 | 170 | 330 | 55 | 220 | 400 |
| 11/2025 | 2.900 | 1.260 | 190 | 350 | 58 | 235 | 420 |
| 12/2025 | 3.400 | 1.520 | 260 | 430 | 66 | 270 | 510 |
| 01/2026 | 2.300 | 980 | 120 | 260 | 45 | 190 | 320 |
| 02/2026 | 2.100 | 900 | 100 | 230 | 41 | 170 | 290 |
| 03/2026 | 2.950 | 1.280 | 200 | 360 | 59 | 240 | 430 |
| 04/2026 | 3.000 | 1.310 | 210 | 370 | 60 | 245 | 440 |
| 05/2026 | 3.050 | 1.340 | 220 | 380 | 61 | 250 | 450 |
| 06/2026 | 3.200 | 1.420 | 240 | 400 | 63 | 260 | 470 |
| 07/2026 | 3.100 | 1.360 | 230 | 390 | 62 | 255 | 460 |
| 08/2026 | 3.150 | 1.390 | 235 | 395 | 62 | 258 | 465 |

## Yêu cầu

1. Phân rã bài toán.
2. 3 phương án, so sánh có trọng số, kiểm chứng và phản biện độc lập.
3. Dashboard ≥ 5 KPI, ý nghĩa quản trị, 3 kịch bản.
4. Báo cáo đề xuất gửi lãnh đạo cơ quan: quy trình mới, nguồn lực, rủi ro, lộ trình.
5. Nguyên tắc AI an toàn của Văn phòng, đặc biệt: xử lý văn bản mật/nội bộ (tuyệt đối không đưa lên AI công cộng), phân quyền theo vai trò văn thư/chánh văn phòng/lãnh đạo, lưu vết bút phê.

## Gợi ý điểm khó

- 8% văn bản mật/nội bộ là **rào cản kiến trúc**: phương án dùng AI công cộng cho phần còn lại phải có bộ lọc tự động dựa trên dấu mật ở hệ thống; phương án hoàn chỉnh cần AI trên hạ tầng nội bộ (Luật BVBMNN 117/2025 cấm dùng AI xâm phạm bí mật nhà nước).
- "AI gợi ý phân công" phải giữ bút phê của lãnh đạo là quyết định; nêu rõ trong quy trình.
- Thể thức: đây là **báo cáo đề xuất** gửi lãnh đạo cùng cơ quan, ký hiệu BC, không phải tờ trình gửi cấp trên; Nơi nhận vẫn theo NĐ 30/2020.
- Căn cứ thêm: Luật Lưu trữ 33/2024 + NĐ 113/2025 (lưu trữ điện tử), Luật Giao dịch điện tử 20/2023 (giao dịch điện tử của CQNN), NĐ 30/2020 (văn thư).
- KPI "giờ Chánh Văn phòng dành cho phân loại" là chỉ số về chi phí cơ hội của lãnh đạo, ý nghĩa quản trị rất mạnh.

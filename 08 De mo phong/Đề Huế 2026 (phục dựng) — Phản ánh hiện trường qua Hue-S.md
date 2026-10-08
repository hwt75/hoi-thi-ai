# Đề Huế 2026 (phục dựng) — Nâng cao hiệu quả xử lý phản ánh hiện trường của người dân qua Hue-S

> **Đây là đề phục dựng**, không phải đề thật của Hội thi TP Huế ngày 10/7/2026 (đề thật không được công bố, xem `Huế 2026 — kết quả tìm đề thật.md`). Đề được dựng đúng theo **định hướng Bảng B** trong Phụ lục Công văn 8158-CV/TWĐTN-KHCN: tình huống cấp sở/ngành có **dữ liệu đa nguồn** (văn bản chỉ đạo, số liệu thống kê, phản ánh của người dân, tiến độ công việc); yêu cầu **prompt có cấu trúc**, **PivotTable/dashboard**, **kiểm chứng đề xuất của AI bằng dữ liệu đề**, sản phẩm công vụ hoàn chỉnh, và **ẩn danh dữ liệu**. Bối cảnh Hue-S là dịch vụ có thật của Huế; mọi số liệu và văn bản trong đề là **mô phỏng**.

**Thời gian: 90 phút. Sản phẩm nộp: (1) báo cáo tham mưu (.docx), (2) bảng tính có PivotTable/biểu đồ và bảng theo dõi tiến độ (.xlsx), (3) bản trình bày ngắn cho lãnh đạo (.pptx), (4) phần trình bày cách đã dùng AI: prompt đã dùng, dữ liệu nào được/không được đưa vào AI, các bước kiểm chứng.**

## Tình huống

Bạn là chuyên viên Trung tâm Giám sát, điều hành đô thị thông minh TP Huế (IOC), bộ phận theo dõi phản ánh hiện trường tiếp nhận qua ứng dụng Hue-S. Phản ánh của người dân được IOC tiếp nhận, phân loại, chuyển UBND phường, xã hoặc đơn vị chuyên môn xử lý, sau đó công khai kết quả trên Hue-S. Quy định nội bộ: xử lý và phản hồi trong **48 giờ** với phản ánh thông thường.

Từ tháng 4/2026 lượng phản ánh tăng mạnh sau khi thành phố sắp xếp đơn vị hành chính, tỷ lệ đúng hạn giảm, người dân bắt đầu phàn nàn trên mạng xã hội. Lãnh đạo Trung tâm yêu cầu bạn trong buổi sáng nay lập báo cáo tham mưu: hiện trạng, nguyên nhân, phương án cải tiến quy trình có ứng dụng AI, bảng theo dõi tiến độ, và nguyên tắc dùng AI an toàn với dữ liệu phản ánh (có thông tin cá nhân của người phản ánh).

## Nguồn dữ liệu 1 — Trích văn bản chỉ đạo (mô phỏng)

> Công văn số …/UBND-… ngày 15/8/2026 của UBND thành phố: "… Giao Trung tâm IOC chủ trì, phối hợp UBND các phường, xã và các sở, ngành: (1) nâng tỷ lệ phản ánh được xử lý, phản hồi đúng hạn 48 giờ đạt **tối thiểu 90%** trước 31/12/2026; (2) giảm phản ánh trùng lặp, phản ánh chuyển sai đơn vị; (3) nghiên cứu ứng dụng trí tuệ nhân tạo hỗ trợ phân loại, điều phối, bảo đảm **không để lộ thông tin cá nhân của người phản ánh** theo quy định của Luật Bảo vệ dữ liệu cá nhân; (4) báo cáo UBND thành phố trước ngày 30/9/2026."

## Nguồn dữ liệu 2 — Thống kê phản ánh theo tháng (toàn thành phố)

| Tháng | Phản ánh tiếp nhận | Xử lý đúng hạn (≤48h) | Quá hạn | Thời gian xử lý TB (giờ) | Phản ánh trùng | Hài lòng (%) |
|---|---|---|---|---|---|---|
| 09/2025 | 2.140 | 1.690 | 450 | 41 | 180 | 78 |
| 10/2025 | 2.260 | 1.760 | 500 | 43 | 195 | 77 |
| 11/2025 | 2.380 | 1.810 | 570 | 46 | 210 | 75 |
| 12/2025 | 2.050 | 1.620 | 430 | 40 | 170 | 79 |
| 01/2026 | 1.780 | 1.450 | 330 | 37 | 140 | 81 |
| 02/2026 | 1.690 | 1.400 | 290 | 36 | 130 | 82 |
| 03/2026 | 2.320 | 1.780 | 540 | 45 | 205 | 76 |
| 04/2026 | 2.610 | 1.930 | 680 | 49 | 240 | 73 |
| 05/2026 | 2.890 | 2.050 | 840 | 53 | 270 | 70 |
| 06/2026 | 3.120 | 2.140 | 980 | 57 | 300 | 68 |
| 07/2026 | 3.260 | 2.190 | 1.070 | 60 | 320 | 66 |
| 08/2026 | 3.180 | 2.170 | 1.010 | 58 | 310 | 67 |

## Nguồn dữ liệu 3 — Phân bổ 12 tháng theo lĩnh vực và theo đơn vị xử lý

| Lĩnh vực | Tiếp nhận | Đúng hạn |
|---|---|---|
| Vệ sinh môi trường, rác thải | 8.420 | 6.890 |
| Trật tự đô thị, vỉa hè | 6.130 | 4.760 |
| Hạ tầng giao thông, chiếu sáng | 5.210 | 3.880 |
| Cấp thoát nước, ngập úng | 3.640 | 2.510 |
| An ninh trật tự, tiếng ồn | 3.960 | 3.310 |
| Hành chính, dịch vụ công | 2.320 | 1.640 |

| Đơn vị xử lý | Tiếp nhận | Đúng hạn |
|---|---|---|
| Phường A | 4.120 | 3.560 |
| Phường B | 3.890 | 3.010 |
| Phường C | 3.410 | 2.340 |
| Phường D | 3.260 | 2.790 |
| Phường E | 2.980 | 2.260 |
| Phường G | 2.740 | 2.310 |
| Phường H | 2.610 | 1.720 |
| Phường K | 2.350 | 2.020 |
| Xã M | 2.190 | 1.520 |
| Xã N | 2.130 | 1.460 |

## Nguồn dữ liệu 4 — Ba phản ánh nguyên văn (mô phỏng, dùng để thử phân loại)

1. "Tôi là Nguyễn Văn T., SĐT 09xx xxx 123, nhà số 15 kiệt … đường Bà Triệu. Rác ở đầu kiệt 3 ngày chưa thu, mùi hôi, có ảnh kèm. Đề nghị phường xử lý gấp." (đã gửi 2 lần trong 2 ngày)
2. "Đèn đường đoạn từ cầu … đến ngã ba … tắt cả tuần, tối rất nguy hiểm cho học sinh. Tôi đã báo phường nhưng phường nói thuộc công ty chiếu sáng."
3. "Quán cà phê số … đường … mở nhạc lớn đến 1 giờ sáng nhiều đêm, con tôi mất ngủ. Tôi tên Lê Thị H., CCCD 046xxxxxxxxx, mong giữ kín tên tôi."

## Yêu cầu

1. **Thiết kế prompt có cấu trúc** (vai trò, bối cảnh, dữ liệu, yêu cầu đầu ra, ràng buộc) để AI hỗ trợ phân tích vấn đề, đề xuất phương án và dàn ý báo cáo. Nộp nguyên văn prompt.
2. **Phân tích dữ liệu bằng Excel**: tổng hợp, PivotTable theo lĩnh vực và đơn vị, biểu đồ xu hướng, dashboard ngắn; chỉ ra ít nhất 5 chỉ số then chốt và ý nghĩa quản trị.
3. **Kiểm chứng đề xuất của AI bằng dữ liệu đề bài**: chỉ rõ điểm hợp lý, điểm cần chỉnh, rủi ro, điều kiện áp dụng.
4. **Sản phẩm công vụ hoàn chỉnh**: báo cáo tham mưu gửi Giám đốc Trung tâm để trình UBND thành phố (hiện trạng, nguyên nhân, phương án, quy trình mới có AI, nguồn lực, rủi ro, lộ trình đến 31/12/2026), kèm **bảng theo dõi tiến độ** các đầu việc.
5. **Bảo mật**: nêu cách ẩn danh 3 phản ánh ở nguồn 4 trước khi đưa vào AI, dữ liệu nào tuyệt đối không đưa lên AI công cộng, và nguyên tắc dùng AI an toàn tại Trung tâm.

## Gợi ý điểm khó (đọc sau khi làm)

- Nguồn 4 là **bẫy điểm liệt**: phản ánh 1 và 3 chứa tên, số điện thoại, CCCD. Đưa nguyên văn lên ChatGPT là vi phạm; phải ẩn danh trước và ghi vào nhật ký.
- Tỷ lệ đúng hạn không giảm đều mà giảm theo **lượng tiếp nhận**: điểm nghẽn là năng lực xử lý ở vài phường (C, H, M, N) và lĩnh vực ngập úng, hạ tầng, chứ không phải toàn hệ thống. Đề xuất AI phải nhắm đúng chỗ đó.
- Phản ánh 2 cho thấy lỗi **điều phối sai đơn vị**; đây là chỗ AI phân loại có giá trị, nhưng người điều phối vẫn quyết định.
- Mục tiêu 90% đến 31/12 chỉ còn 3 tháng: bài phải tách "làm ngay" (điều phối, tăng cường phường yếu) và "nền tảng" (AI phân loại, gộp trùng), và nói thẳng khả năng đạt.
- Bảng theo dõi tiến độ là sản phẩm riêng của Bảng B, đừng bỏ.

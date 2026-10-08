# Đề mô phỏng 02 — Cải tiến quy trình nghiệp vụ: tiếp nhận và xử lý phản ánh, kiến nghị của khách hàng qua kênh số

**Thời gian: 90 phút. Sản phẩm nộp: tờ trình (.docx), bảng tính/dashboard (.xlsx), slide (.pptx). Thuyết trình 3 phút.**

## Tình huống

Trung tâm Chăm sóc khách hàng của Hội sở một ngân hàng thương mại nhà nước tiếp nhận phản ánh, kiến nghị (PAKN) của khách hàng qua 4 kênh: tổng đài, ứng dụng ngân hàng số, email, và cổng dịch vụ công/mạng xã hội. Quy trình hiện tại: nhân viên đọc từng PAKN, phân loại thủ công vào 18 nhóm nghiệp vụ, chuyển phòng chuyên môn, theo dõi, tổng hợp trả lời, gửi khách hàng. Vấn đề:

- Khoảng 30% PAKN bị phân loại sai nhóm ở lần đầu, phải chuyển lại, mỗi lần chuyển mất trung bình 1,5 ngày.
- Quy định nội bộ yêu cầu trả lời trong 5 ngày làm việc; tỷ lệ đúng hạn dao động 70–78%.
- Câu trả lời do nhiều phòng soạn, không thống nhất giọng văn, đôi khi trích quy định đã cũ.
- Trung tâm muốn dùng AI để phân loại sơ bộ, gợi ý phòng xử lý, dự thảo trả lời theo mẫu, và tổng hợp báo cáo tuần cho Ban Tổng Giám đốc.
- Nội dung PAKN chứa họ tên, số tài khoản, số giao dịch, đôi khi cả ảnh CCCD.

## Dữ liệu đề cho (12 tháng) [số liệu mô phỏng]

| Tháng | PAKN tiếp nhận | Phân loại sai lần đầu | Trả lời đúng hạn | Thời gian xử lý TB (ngày) | Giờ công | PAKN về lỗi giao dịch số | Khách hàng đánh giá hài lòng (%) |
|---|---|---|---|---|---|---|---|
| 09/2025 | 4.120 | 1.180 | 3.140 | 4,6 | 3.300 | 1.510 | 71 |
| 10/2025 | 4.380 | 1.290 | 3.290 | 4,8 | 3.480 | 1.640 | 70 |
| 11/2025 | 4.650 | 1.400 | 3.420 | 5,1 | 3.720 | 1.790 | 68 |
| 12/2025 | 5.900 | 1.860 | 4.130 | 5,9 | 4.700 | 2.480 | 63 |
| 01/2026 | 6.300 | 2.010 | 4.350 | 6,2 | 5.020 | 2.700 | 61 |
| 02/2026 | 3.900 | 1.090 | 3.050 | 4,4 | 3.120 | 1.320 | 73 |
| 03/2026 | 4.700 | 1.390 | 3.520 | 4,9 | 3.760 | 1.750 | 69 |
| 04/2026 | 4.850 | 1.450 | 3.620 | 5,0 | 3.880 | 1.820 | 69 |
| 05/2026 | 5.000 | 1.510 | 3.700 | 5,2 | 4.000 | 1.900 | 68 |
| 06/2026 | 5.250 | 1.600 | 3.830 | 5,4 | 4.200 | 2.050 | 67 |
| 07/2026 | 5.400 | 1.660 | 3.890 | 5,6 | 4.320 | 2.140 | 66 |
| 08/2026 | 5.600 | 1.740 | 3.980 | 5,8 | 4.480 | 2.260 | 65 |

## Yêu cầu

1. Phân rã bài toán (mục tiêu, đối tượng tác động, ràng buộc pháp lý, dữ liệu, tiêu chí).
2. Ít nhất 3 phương án cải tiến quy trình, so sánh có trọng số; phần kiểm chứng và phản biện độc lập đối với đầu ra AI.
3. Dashboard: ít nhất 5 KPI, ý nghĩa quản trị, 3 kịch bản hiệu quả.
4. Tờ trình Ban Tổng Giám đốc: **quy trình mới dạng bảng bước** (ai làm gì, AI hỗ trợ gì, điểm kiểm soát, thời gian), nguồn lực, rủi ro, lộ trình.
5. Nguyên tắc AI an toàn cho Trung tâm: đặc biệt cách xử lý dữ liệu cá nhân trong PAKN trước khi đưa vào AI, và kiểm soát dự thảo trả lời trước khi gửi khách hàng.

## Gợi ý điểm khó

- PAKN chứa dữ liệu cá nhân và thông tin tài khoản → phương án phải có bước **che/ẩn danh tự động** trước khi AI phân loại; hoặc AI chạy trên hạ tầng nội bộ.
- Dự thảo trả lời gửi khách hàng là "đầu ra hướng ngoại" → bắt buộc người duyệt; nêu rõ khách hàng biết có AI hỗ trợ hay không (dự thảo Thông tư NHNN về AI: chatbot phải thông báo).
- KPI "phân loại sai lần đầu" là chỉ số đo trực tiếp giá trị của AI; đặt mục tiêu cho nó.
- Tháng 12–01 tăng vọt do mùa cao điểm: phương án phải nói được cách xử lý đỉnh tải.
- "Trích quy định đã cũ" → trợ lý công vụ chỉ trả lời từ kho quy định đã cập nhật (điểm cộng cho Custom GPT demo).

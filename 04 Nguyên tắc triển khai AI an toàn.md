# Bộ nguyên tắc triển khai AI an toàn trong đơn vị

Dùng làm **Phụ lục** của tờ trình. Trong phòng thi: chạy prompt P10 để thêm 2 quy tắc riêng cho bài toán vào mỗi trục, điền tên đơn vị, xong. Căn cứ pháp lý ở mỗi trục lấy từ `03` (đã kiểm ngày 09/9/2026; tự kiểm lại trước ngày thi).

## Mở đầu (3 câu, dán vào đầu phụ lục)

Việc ứng dụng trí tuệ nhân tạo tại {ĐƠN VỊ} tuân thủ nguyên tắc **AI hỗ trợ, con người quyết định và chịu trách nhiệm** theo Luật Trí tuệ nhân tạo số 134/2025/QH15 và Khung đạo đức trí tuệ nhân tạo quốc gia (Thông tư 05/2026/TT-BKHCN). Bộ nguyên tắc gồm bốn trục: phân quyền dữ liệu, kiểm soát đầu ra, lưu vết sử dụng, đào tạo người dùng; mỗi trục có biện pháp cụ thể, người chịu trách nhiệm và bằng chứng kiểm tra. Bộ nguyên tắc áp dụng cho mọi công cụ AI, kể cả công cụ công cộng do cá nhân tự đăng ký.

## Phân loại dữ liệu (nền của trục 1)

| Mức | Ví dụ tại ngân hàng | Được dùng với AI nào |
|---|---|---|
| **M1 Công khai** | Văn bản pháp luật, biểu mẫu công bố, thông cáo, lãi suất niêm yết | Mọi công cụ, kể cả AI công cộng |
| **M2 Nội bộ** | Quy trình nghiệp vụ, số liệu tổng hợp không định danh, dự thảo chưa ban hành | AI công cộng **chỉ khi đã ẩn danh hoá và bỏ số liệu nhạy cảm**; ưu tiên AI có hợp đồng doanh nghiệp (không dùng dữ liệu để huấn luyện) |
| **M3 Dữ liệu cá nhân, thông tin khách hàng** | Họ tên + CCCD, số tài khoản, số dư, lịch sử giao dịch, sinh trắc học, điểm tín dụng | **Cấm** đưa lên AI công cộng. Chỉ AI triển khai trên hạ tầng nội bộ / đã đánh giá tác động theo NĐ 356/2025 |
| **M4 Mật, bí mật kinh doanh, bí mật nhà nước** | Tài liệu đóng dấu mật, chiến lược chưa công bố, dữ liệu thanh tra | **Cấm tuyệt đối** với mọi AI ngoài hệ thống được cấp phép riêng |

Căn cứ: Luật BVBMNN 117/2025/QH15 (cấm dùng AI xâm phạm bí mật nhà nước); Luật Các TCTD 32/2024/QH15 Điều 13 và NĐ 117/2018/NĐ-CP (bí mật thông tin khách hàng, không cung cấp cho bên thứ ba); Luật BVDLCN 91/2025/QH15 và NĐ 356/2025/NĐ-CP (danh mục DLCN cơ bản/nhạy cảm); CV 557/BKHCN-CĐSQG (cấm nhập bí mật nhà nước, thông tin nội bộ chưa công bố, DLCN vào chatbot AI công cộng).

## Bốn trục

| Trục | Nguyên tắc | Biện pháp cụ thể | Người chịu trách nhiệm | Bằng chứng kiểm tra |
|---|---|---|---|---|
| **1. Phân quyền dữ liệu** | Dữ liệu chỉ đến được AI ở mức được phép; quyền theo vai trò, không theo cá nhân | 1.1 Áp dụng bảng phân loại M1–M4; mọi tài liệu đưa vào AI phải được gán mức trước.<br>1.2 Tài khoản AI cấp theo vai trò (soạn thảo / phân tích / quản trị), đăng nhập SSO, tắt tính năng dùng dữ liệu để huấn luyện.<br>1.3 Dữ liệu M3 chỉ xử lý bằng AI trên hạ tầng nội bộ hoặc nhà cung cấp có thoả thuận xử lý dữ liệu; có hồ sơ đánh giá tác động xử lý DLCN.<br>1.4 Ẩn danh hoá bắt buộc (thay tên, che số) trước khi dùng dữ liệu M2 với AI công cộng.<br>*(P10 thêm 2 quy tắc riêng cho bài toán)* | Trưởng đơn vị chủ quản dữ liệu; Phòng CNTT (kỹ thuật); Bộ phận Pháp chế (đánh giá tác động) | Bảng phân loại đã ký; danh sách tài khoản và vai trò; hồ sơ đánh giá tác động; biên bản kiểm tra định kỳ quý |
| **2. Kiểm soát đầu ra** | AI đề xuất, người có thẩm quyền quyết định; đầu ra phải kiểm chứng trước khi dùng | 2.1 Không có quy trình nào để AI tự động phê duyệt, từ chối, xếp hạng hồ sơ hay đánh giá cá nhân.<br>2.2 Đầu ra AI được đánh dấu "Dự thảo do AI hỗ trợ" cho đến khi người có thẩm quyền ký.<br>2.3 Bắt buộc kiểm chứng: số liệu đối chiếu nguồn gốc; căn cứ pháp lý tra trên cơ sở dữ liệu văn bản; nội dung nghiệp vụ do cán bộ chuyên môn xác nhận.<br>2.4 Đầu ra dùng cho khách hàng (chatbot, thông báo) phải nêu rõ là do AI tạo và có đường thoát sang người thật.<br>2.5 Phân loại rủi ro hệ thống AI theo Luật TTNT trước khi triển khai; hệ thống rủi ro cao phải đánh giá an toàn và được người đại diện theo pháp luật phê duyệt. | Người ký văn bản; Trưởng phòng nghiệp vụ; Bộ phận kiểm soát nội bộ | Dấu "Dự thảo AI hỗ trợ" trên bản thảo; checklist kiểm chứng đính kèm hồ sơ; phiếu phân loại rủi ro; báo cáo sai lệch AI hằng tháng |
| **3. Lưu vết sử dụng** | Mọi lần dùng AI trong công vụ đều truy được: ai, khi nào, đưa gì vào, lấy gì ra, dùng vào đâu | 3.1 Nhật ký sử dụng AI theo mẫu (thời điểm, công cụ, mục đích, mức dữ liệu đầu vào, đầu ra dùng thế nào, người kiểm chứng) đính kèm hồ sơ công việc.<br>3.2 Công cụ AI nội bộ ghi log tập trung theo Thông tư 09/2020/TT-NHNN; lưu tối thiểu theo quy định lưu trữ.<br>3.3 Sự cố (rò rỉ dữ liệu, đầu ra sai gây hậu quả) báo cáo trong 24 giờ cho Phòng CNTT và Kiểm soát nội bộ.<br>3.4 Rà soát nhật ký ngẫu nhiên hằng tháng; phát hiện đưa dữ liệu M3/M4 lên AI công cộng thì xử lý như vi phạm bảo mật. | Từng cán bộ (ghi nhật ký); Phòng CNTT (log hệ thống); Kiểm soát nội bộ (rà soát) | Nhật ký trong hồ sơ; log hệ thống; biên bản rà soát tháng; sổ sự cố |
| **4. Đào tạo người dùng** | Chỉ người đã được đào tạo mới được dùng AI trong công vụ; đào tạo lại khi công cụ hoặc quy định đổi | 4.1 Khoá bắt buộc 4 giờ trước khi cấp tài khoản: phân loại dữ liệu, viết yêu cầu, nhận biết AI bịa, kiểm chứng, ghi nhật ký; kiểm tra đạt ≥ 80%.<br>4.2 Cập nhật hằng năm theo Chỉ thị 14/CT-TTg (kỹ năng số CBCCVC) và khi có văn bản mới.<br>4.3 Mỗi phòng có 1 "đầu mối AI" hỗ trợ đồng nghiệp và tổng hợp lỗi thường gặp.<br>4.4 Thư viện prompt và mẫu đầu ra chuẩn dùng chung, cập nhật quý. | Phòng Tổ chức nhân sự (kế hoạch); Phòng CNTT (nội dung kỹ thuật); Trưởng phòng (cử đầu mối) | Danh sách hoàn thành khoá học; kết quả kiểm tra; danh sách đầu mối; thư viện prompt có ngày cập nhật |

## Lộ trình áp dụng bộ nguyên tắc (gắn với lộ trình 3 giai đoạn của tờ trình)

| Giai đoạn | Việc về AI an toàn |
|---|---|
| Thí điểm (3 tháng) | Ban hành bảng phân loại dữ liệu; cấp tài khoản cho nhóm thí điểm sau đào tạo; nhật ký thủ công; chỉ dữ liệu M1–M2 |
| Mở rộng (6 tháng) | Đánh giá tác động DLCN; triển khai AI trên hạ tầng nội bộ cho dữ liệu M3; log tập trung; rà soát tháng |
| Vận hành chính thức | Quy chế sử dụng AI ban hành chính thức; kiểm toán nội bộ hằng năm; cập nhật theo Thông tư của NHNN về AI khi ban hành |

## Căn cứ pháp lý của bộ nguyên tắc (dán vào cuối phụ lục)

- Luật Trí tuệ nhân tạo số 134/2025/QH15 (Điều 9 phân loại rủi ro; nguyên tắc AI không thay thế thẩm quyền, trách nhiệm con người) và Nghị định 142/2026/NĐ-CP.
- Thông tư 05/2026/TT-BKHCN ban hành Khung đạo đức trí tuệ nhân tạo quốc gia (Điều 3: an toàn tin cậy, quyền con người và công bằng, trách nhiệm giải trình).
- Công văn 557/BKHCN-CĐSQG ngày 31/3/2025 hướng dẫn CCVC sử dụng chatbot AI.
- Luật Bảo vệ dữ liệu cá nhân số 91/2025/QH15; Nghị định 356/2025/NĐ-CP.
- Luật Bảo vệ bí mật nhà nước số 117/2025/QH15; Luật An ninh mạng số 116/2025/QH15.
- Luật Các tổ chức tín dụng số 32/2024/QH15 (Điều 13); Nghị định 117/2018/NĐ-CP.
- Thông tư 09/2020/TT-NHNN về an toàn hệ thống thông tin trong hoạt động ngân hàng.
- Chỉ thị 14/CT-TTg ngày 22/4/2026 về bồi dưỡng kiến thức, kỹ năng số cho CBCCVC.
- (Tham khảo định hướng, chưa có hiệu lực) Dự thảo Thông tư của NHNN về an toàn, quản lý rủi ro và điều kiện triển khai AI trong ngành Ngân hàng.

## Câu chốt khi thuyết trình (15 giây)

"Bốn trục này không phải lý thuyết: chính bài thi này đã áp dụng cả bốn. Dữ liệu đề bài được phân loại trước khi đưa vào AI, mọi đầu ra được kiểm chứng chéo bằng mô hình thứ hai và tra tay, nhật ký sử dụng AI đính kèm ở phụ lục, và tôi là người đã được đào tạo để làm việc đó."

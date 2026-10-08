# Đáp án mẫu — Đề Huế 2026 (phục dựng): Phản ánh hiện trường qua Hue-S

Bài mẫu theo 5 yêu cầu của đề (định hướng Bảng B). Số liệu tính từ 4 nguồn trong đề; số khác gắn [GIẢ ĐỊNH]. Căn cứ pháp lý theo tệp 03 (tra 09/9/2026). Khác với đề Bảng C, đề này chấm nặng ở **prompt có cấu trúc** và **kiểm chứng đề xuất AI bằng dữ liệu**, nên hai phần đó viết kỹ hơn.

---

## Yêu cầu 1 — Prompt có cấu trúc (nộp nguyên văn)

### Bước 0: ẩn danh trước khi dùng AI (làm tay, 2 phút)

Ba phản ánh ở nguồn 4 được viết lại trước khi dán vào AI:

| Gốc | Sau ẩn danh |
|---|---|
| "Tôi là Nguyễn Văn T., SĐT 09xx xxx 123, nhà số 15 kiệt … đường Bà Triệu. Rác ở đầu kiệt 3 ngày chưa thu…" (gửi 2 lần) | "PA-01: Người dân khu vực đường Bà Triệu phản ánh rác đầu kiệt 3 ngày chưa thu, có ảnh, gửi 2 lần trong 2 ngày." |
| "Đèn đường đoạn từ cầu … đến ngã ba … tắt cả tuần… phường nói thuộc công ty chiếu sáng." | "PA-02: Đèn đường một đoạn tuyến tắt cả tuần, nguy hiểm cho học sinh; phường trả lời thuộc công ty chiếu sáng." |
| "Quán cà phê số … đường … mở nhạc lớn đến 1 giờ sáng… Tôi tên Lê Thị H., CCCD 046xxxxxxxxx, mong giữ kín tên." | "PA-03: Quán cà phê trên một tuyến phố mở nhạc lớn đến 1 giờ sáng nhiều đêm; người phản ánh đề nghị giữ kín danh tính." |

Nguyên tắc: bỏ họ tên, số điện thoại, CCCD, số nhà; giữ lĩnh vực, địa bàn ở mức tuyến đường, nội dung và tình trạng lặp lại. Số liệu thống kê (nguồn 2, 3) là dữ liệu tổng hợp không định danh, được phép đưa vào AI. Văn bản chỉ đạo (nguồn 1) chỉ đưa phần trích trong đề, không đưa số công văn và toàn văn.

### Prompt 1 — Phân tích vấn đề (ChatGPT)

```
[VAI TRÒ] Bạn là chuyên viên phân tích của Trung tâm Giám sát, điều hành đô thị thông minh một thành phố trực thuộc Trung ương, có kinh nghiệm cải tiến quy trình xử lý phản ánh của người dân.

[BỐI CẢNH] Phản ánh hiện trường của người dân qua ứng dụng đô thị thông minh được Trung tâm tiếp nhận, phân loại, chuyển đơn vị xử lý, công khai kết quả. Hạn xử lý 48 giờ. UBND thành phố giao mục tiêu: đúng hạn ≥ 90% trước 31/12/2026, giảm trùng lặp và chuyển sai đơn vị, ứng dụng AI hỗ trợ phân loại, điều phối nhưng không để lộ thông tin cá nhân người phản ánh.

[DỮ LIỆU] (a) Bảng 12 tháng: {dán nguồn 2}. (b) Phân bổ theo lĩnh vực và đơn vị: {dán nguồn 3}. (c) Ba phản ánh đã ẩn danh: {dán PA-01..03}.

[YÊU CẦU ĐẦU RA] Trả lời đúng 4 phần, dạng bảng hoặc danh sách đánh số:
1. Hiện trạng: 6 chỉ số then chốt tính từ dữ liệu, ghi rõ công thức và con số (12 tháng và tháng gần nhất).
2. Nguyên nhân: xếp hạng 4 nguyên nhân có bằng chứng số liệu; mỗi nguyên nhân chỉ ra dòng dữ liệu nào chứng minh.
3. Ba phương án cải tiến theo mức thay đổi tăng dần; mỗi phương án: các bước, AI làm gì / người làm gì, nguồn lực [GIẢ ĐỊNH], rủi ro, khả năng đạt 90% trước 31/12 (Cao/Trung/Thấp kèm lý do).
4. Dàn ý báo cáo tham mưu 7 mục.

[RÀNG BUỘC] Không bịa số ngoài dữ liệu đã cho; số tự đặt phải gắn [GIẢ ĐỊNH]. Không nêu số hiệu văn bản pháp luật; nếu cần nói "cần tra". AI trong phương án chỉ được đề xuất, phân loại, dự thảo; quyết định và phản hồi chính thức là con người. Văn phong hành chính, câu ngắn.
```

### Prompt 2 — Phản biện chéo (Claude, dán đầu ra Prompt 1)

```
[VAI TRÒ] Bạn là Phó Giám đốc phụ trách nghiệp vụ, nổi tiếng khó tính khi duyệt báo cáo tham mưu.
[DỮ LIỆU] Bản phân tích do một chuyên viên làm với sự hỗ trợ của AI: {dán đầu ra Prompt 1} và dữ liệu gốc: {dán nguồn 2, 3}.
[YÊU CẦU] Đối chiếu từng con số và từng nhận định với dữ liệu gốc. Trả về bảng: STT | Nhận định/con số | Khớp dữ liệu? (Đúng/Sai/Không kiểm được) | Chỉ ra dòng dữ liệu | Cần sửa thế nào. Sau bảng: 3 rủi ro bị bỏ sót và 2 điều kiện để phương án đề xuất khả thi. Không khen.
```

### Prompt 3 — Bảng theo dõi tiến độ (ChatGPT, sau khi chốt phương án)

```
Từ phương án đã chọn: {dán}. Lập bảng theo dõi tiến độ đến 31/12/2026, xuất CSV: Mã việc | Đầu việc | Đơn vị chủ trì | Phối hợp | Bắt đầu | Hạn | Sản phẩm | Chỉ số đo | Trạng thái (để trống) | Ghi chú. Tối đa 12 đầu việc, chia 3 nhóm: làm ngay (tháng 10), nền tảng (tháng 10–11), đánh giá (tháng 12).
```

---

## Yêu cầu 2 — Phân tích dữ liệu (Excel)

### Chỉ số then chốt

| Chỉ số | 12 tháng | 08/2026 | Mục tiêu 31/12 | Ý nghĩa quản trị |
|---|---|---|---|---|
| Tỷ lệ xử lý đúng hạn 48h | 74,1% | 68,2% | ≥ 90% | Giảm từ 79,0% (9/2025) xuống 68,2%: hệ thống mất 11 điểm trong khi lượng phản ánh tăng 49%. Lãnh đạo cần quyết: tăng năng lực xử lý ở đâu, chứ không phải tuyên truyền người dân bớt phản ánh. IOC theo dõi tuần. |
| Tỷ lệ quá hạn | 25,9% | 31,8% | ≤ 10% | Cứ 3 phản ánh tháng 8 có 1 quá hạn. Vượt 20% liên tiếp 2 tuần → họp giao ban với các phường quá hạn nhiều. |
| Thời gian xử lý trung bình (giờ, trọng số) | 48,7 | 58 | ≤ 36 | Đã vượt hạn 48h ngay ở mức trung bình, nghĩa là quá nửa phản ánh trễ nhẹ; giảm được nhanh bằng điều phối đúng đơn vị ngay từ đầu. |
| Tỷ lệ phản ánh trùng | 9,0% | 9,7% | ≤ 3% | Gần 1/10 công sức xử lý là việc trùng, và trùng tăng khi trễ (dân gửi lại). AI gộp trùng giải quyết trực tiếp; đây là lợi ích dễ đo nhất. |
| Hài lòng (trọng số) | 73,2% | 67% | ≥ 85% | Đi ngược chiều thời gian xử lý gần như hoàn hảo: dân chấm điểm tốc độ. Không cần khảo sát thêm, cần giảm giờ. |
| Chênh lệch đúng hạn giữa đơn vị | 65,9% – 86,4% | — | mọi đơn vị ≥ 85% | 4 đơn vị dưới 70% (Phường C 68,6%, Phường H 65,9%, Xã M 69,4%, Xã N 68,5%) chiếm 10.340 phản ánh, bằng 35% tổng. Nâng 4 đơn vị này lên 85% là +1.600 phản ánh đúng hạn, tương đương +5,4 điểm toàn thành phố. |

### PivotTable 1 — theo lĩnh vực (từ nguồn 3)

| Lĩnh vực | Tiếp nhận | Đúng hạn | Tỷ lệ | Quá hạn |
|---|---|---|---|---|
| Vệ sinh môi trường, rác thải | 8.420 | 6.890 | 81,8% | 1.530 |
| Trật tự đô thị, vỉa hè | 6.130 | 4.760 | 77,7% | 1.370 |
| Hạ tầng giao thông, chiếu sáng | 5.210 | 3.880 | 74,5% | 1.330 |
| Cấp thoát nước, ngập úng | 3.640 | 2.510 | 69,0% | 1.130 |
| An ninh trật tự, tiếng ồn | 3.960 | 3.310 | 83,6% | 650 |
| Hành chính, dịch vụ công | 2.320 | 1.640 | 70,7% | 680 |
| **Tổng** | **29.680** | **21.990** | **74,1%** | **7.690** |

Đọc: ba lĩnh vực đầu chiếm 55% số quá hạn; hai lĩnh vực có tỷ lệ thấp nhất (ngập úng, hành chính) đều thuộc loại **phải chuyển sang đơn vị chuyên môn** chứ phường không tự xử lý được → lỗi nằm ở điều phối liên đơn vị, khớp với PA-02.

### PivotTable 2 — theo đơn vị (từ nguồn 3), xếp theo tỷ lệ

Phường A 86,4% · Phường K 86,0% · Phường D 85,6% · Phường G 84,3% · Phường B 77,4% · Phường E 75,8% · Xã M 69,4% · Phường C 68,6% · Xã N 68,5% · Phường H 65,9%.

Đọc: 4 đơn vị tốt nhất đã đạt gần 90% với cách làm hiện tại → mục tiêu 90% không phi thực tế, vấn đề là lan cách làm của nhóm này sang nhóm dưới.

### Biểu đồ (sheet Dashboard)

1. Đường kép "Tiếp nhận" và "Tỷ lệ đúng hạn" 12 tháng, tiêu đề: *"Tiếp nhận tăng 49% từ tháng 2, đúng hạn rơi 14 điểm"*.
2. Cột "Quá hạn theo lĩnh vực", tiêu đề: *"Ba lĩnh vực chiếm 55% quá hạn"*.
3. Thanh ngang "Tỷ lệ đúng hạn theo đơn vị" có đường mốc 85%, tiêu đề: *"4 đơn vị dưới 70% giữ 35% khối lượng"*.
4. Phân tán "Thời gian xử lý" và "Hài lòng", tiêu đề: *"Dân chấm điểm tốc độ"*.

---

## Yêu cầu 3 — Kiểm chứng đề xuất của AI bằng dữ liệu đề (Phụ lục 2)

Đầu ra Prompt 1 (ChatGPT) sau khi qua Prompt 2 (Claude) và tự đối chiếu:

| STT | AI nói | Kiểm bằng dữ liệu | Kết luận | Xử lý |
|---|---|---|---|---|
| 1 | "Tỷ lệ đúng hạn giảm do phản ánh tăng đột biến sau sắp xếp đơn vị hành chính" | Tiếp nhận tăng từ 2.320 (3/2026) lên 3.260 (7/2026), đúng hạn giảm 76,7% → 67,2% cùng kỳ | **Hợp lý**, nhưng tháng 10–11/2025 lượng 2.260–2.380 cũng đã cho đúng hạn 76–77%, tức năng lực xử lý đã căng từ trước | Giữ, thêm câu "năng lực xử lý đã tới hạn từ cuối 2025" |
| 2 | "Nguyên nhân chính là phường thiếu nhân lực" | Không có dữ liệu nhân lực trong đề; 4 phường tốt nhất đạt 84–86% với cùng cơ chế | **Không kiểm được**, có dấu hiệu sai: chênh lệch giữa đơn vị lớn hơn chênh lệch giữa tháng | Hạ xuống "giả thuyết cần khảo sát"; thay bằng nguyên nhân có bằng chứng: điều phối sai đơn vị (lĩnh vực chuyển tiếp có tỷ lệ thấp nhất) và trùng lặp 9% |
| 3 | "AI phân loại sẽ nâng đúng hạn lên 90% trong 3 tháng" | Trùng lặp 9,0% và lĩnh vực chuyển tiếp chiếm 1.810 quá hạn; loại bỏ hết cũng chỉ thêm ≈ 6–8 điểm | **Lạc quan quá**: AI một mình không đủ, phải kèm tăng cường 4 đơn vị yếu | Đưa 3 kịch bản: thận trọng 82%, cơ sở 87%, lạc quan 91% [GIẢ ĐỊNH]; báo cáo nói thẳng 90% là "có thể đạt nếu…" |
| 4 | AI đề xuất "hệ thống tự động đóng phản ánh trùng" | PA-01 gửi 2 lần vì chưa được xử lý; đóng tự động sẽ mất phản ánh chính đáng | **Rủi ro** giao quyền cho AI | Sửa: AI gợi ý "có thể trùng với PA-…", điều phối viên xác nhận gộp; phản ánh gốc giữ nguyên trạng thái |
| 5 | AI trích "Nghị định 13/2023 về dữ liệu cá nhân" | Tệp 03: NĐ 13/2023 hết hiệu lực 01/01/2026, thay bằng Luật BVDLCN 91/2025 + NĐ 356/2025 | **Sai hiệu lực** | Thay căn cứ; ghi vào nhật ký là điểm AI bịa/lỗi thời |
| 6 | AI xếp "hài lòng thấp" là nguyên nhân | Hài lòng giảm cùng chiều thời gian xử lý (r âm rõ theo bảng) | **Nhầm nhân quả**: hài lòng là hệ quả | Chuyển sang chỉ số kết quả |
| 7 | Claude bổ sung rủi ro "phường coi AI là lý do để chờ" | Không có trong dữ liệu, nhưng khớp kinh nghiệm vận hành | Chấp nhận là rủi ro vận hành | Thêm biện pháp: hạn 48h tính từ lúc tiếp nhận, không tính từ lúc AI phân loại xong |

Điều kiện áp dụng phương án (từ Prompt 2, đã đối chiếu): (1) UBND thành phố ban hành quy chế phối hợp có chế tài với đơn vị quá hạn; (2) dữ liệu phản ánh được ẩn danh **tự động** ở hệ thống trước khi tới mô-đun AI, không giao cán bộ làm tay.

---

## Yêu cầu 4 — Báo cáo tham mưu (rút gọn; thể thức theo mẫu 05, ký hiệu BC)

**BÁO CÁO — Hiện trạng và phương án nâng cao hiệu quả xử lý phản ánh hiện trường qua Hue-S** · Kính gửi: Giám đốc Trung tâm.

**I. Hiện trạng**: 12 tháng tiếp nhận 29.680 phản ánh, đúng hạn 74,1%; tháng 8/2026 còn 68,2% với 3.180 phản ánh, thời gian xử lý trung bình 58 giờ, vượt hạn 48 giờ; trùng lặp 9,7%; hài lòng 67%. Bốn đơn vị dưới 70% giữ 35% khối lượng; hai lĩnh vực phải chuyển đơn vị chuyên môn (ngập úng, hành chính) có tỷ lệ thấp nhất.

**II. Nguyên nhân** (có bằng chứng số liệu): (1) năng lực xử lý tới hạn từ cuối 2025, lượng tăng 49% sau tháng 2/2026; (2) điều phối sai hoặc chậm với phản ánh liên đơn vị; (3) trùng lặp 9% do dân gửi lại khi chưa thấy phản hồi; (4) chênh lệch cách làm giữa đơn vị. Nguyên nhân "thiếu nhân lực" chưa có dữ liệu, đề nghị khảo sát.

**III. Căn cứ**: NQ 57-NQ/TW; Luật TTNT 134/2025/QH15, NĐ 142/2026/NĐ-CP; Luật BVDLCN 91/2025/QH15, NĐ 356/2025/NĐ-CP; Luật ANM 116/2025/QH15; Luật Dữ liệu 60/2024/QH15; TT 05/2026/TT-BKHCN; CV 557/BKHCN-CĐSQG; QĐ 1671/QĐ-TTg; Công văn số …/UBND-… ngày 15/8/2026 của UBND thành phố; Quy chế vận hành Hue-S [điền].

**IV. Phương án**: so sánh 3 phương án (Excel): PA1 điều phối lại + tăng cường 4 đơn vị yếu, không AI (3,55); **PA2 PA1 + AI hỗ trợ phân loại, gợi ý đơn vị, gợi ý trùng, dự thảo phản hồi (3,95)**; PA3 nền tảng mới tích hợp toàn bộ (2,60). Chọn PA2. Quy trình mới:

| Bước | Việc | Người | AI hỗ trợ | Kiểm soát | Hạn |
|---|---|---|---|---|---|
| 1 | Tiếp nhận, ẩn danh tự động | Hệ thống Hue-S | Không | Log ẩn danh | 0h |
| 2 | Phân loại lĩnh vực, gợi ý đơn vị, gợi ý trùng | Điều phối viên IOC | Gợi ý kèm độ tin cậy và lý do | Điều phối viên xác nhận; dưới 80% tin cậy bắt buộc xem tay | 2h |
| 3 | Xử lý hiện trường | Đơn vị được giao | Không | Cập nhật trạng thái có ảnh | 40h |
| 4 | Dự thảo phản hồi cho dân | Cán bộ đơn vị | Dự thảo theo mẫu từ trạng thái xử lý | Người ký duyệt; mở đầu "phản hồi có hỗ trợ của AI" | 46h |
| 5 | Công khai, đo hài lòng, cảnh báo quá hạn | IOC | Tổng hợp tuần, cảnh báo đơn vị sắp quá hạn | Giao ban tuần | 48h |

**V. Nguồn lực** [GIẢ ĐỊNH]: 2 điều phối viên tăng cường tháng 10–12; dịch vụ AI 120 triệu/năm hoặc mô hình chạy trên hạ tầng IOC; điều chỉnh Hue-S 250 triệu; đào tạo 40 người, 60 triệu.

**VI. Rủi ro**: lộ thông tin cá nhân (ẩn danh tự động, đánh giá tác động theo NĐ 356/2025); AI phân loại sai (ngưỡng tin cậy, người xác nhận, đo tỷ lệ sửa lại hằng tuần); đóng nhầm phản ánh trùng (chỉ gợi ý, không tự đóng); đơn vị ỷ lại AI (hạn tính từ tiếp nhận); phụ thuộc nhà cung cấp (hợp đồng dữ liệu, phương án nội bộ); không đạt 90% (tiêu chí dừng/đi tiếp tháng 11).

**VII. Lộ trình đến 31/12/2026**: Tháng 10 làm ngay: điều phối lại lĩnh vực chuyển tiếp, giao ban với 4 đơn vị yếu, cảnh báo quá hạn thủ công. Tháng 10–11 nền tảng: ẩn danh tự động, thí điểm AI phân loại ở 3 lĩnh vực nhiều quá hạn nhất, đo tỷ lệ gợi ý đúng. Tháng 12: mở rộng nếu gợi ý đúng ≥ 85%, đánh giá, báo cáo UBND. Kịch bản cơ sở đạt 87%, mốc 90% đạt nếu quy chế phối hợp ban hành trong tháng 10.

**VIII. Kiến nghị**: phê duyệt PA2; trình UBND ban hành quy chế phối hợp có chế tài; cho phép áp dụng nguyên tắc AI an toàn tại Phụ lục 3.

### Bảng theo dõi tiến độ (sheet riêng trong Excel)

| Mã | Đầu việc | Chủ trì | Phối hợp | Bắt đầu | Hạn | Sản phẩm | Chỉ số đo | Trạng thái |
|---|---|---|---|---|---|---|---|---|
| V01 | Rà soát, ban hành bảng điều phối lĩnh vực → đơn vị | IOC | Sở chuyên môn | 01/10 | 10/10 | Bảng điều phối | Tỷ lệ chuyển sai | |
| V02 | Giao ban với Phường C, H, Xã M, N; cam kết đúng hạn | Giám đốc IOC | 4 đơn vị | 05/10 | 15/10 | Biên bản | Đúng hạn 4 đơn vị ≥ 80% tháng 11 | |
| V03 | Cảnh báo quá hạn thủ công hằng ngày | IOC | — | 01/10 | liên tục | Báo cáo ngày | Quá hạn ≤ 20% | |
| V04 | Ẩn danh tự động trên Hue-S | Phòng kỹ thuật | Nhà cung cấp | 01/10 | 31/10 | Mô-đun, log | 0 phản ánh có DLCN tới AI | |
| V05 | Đánh giá tác động xử lý DLCN | Pháp chế | IOC | 01/10 | 31/10 | Hồ sơ theo NĐ 356/2025 | Hoàn thành | |
| V06 | Thí điểm AI phân loại 3 lĩnh vực | IOC | Kỹ thuật | 01/11 | 30/11 | Báo cáo thí điểm | Gợi ý đúng ≥ 85% | |
| V07 | Mẫu phản hồi và dự thảo AI | IOC | Đơn vị | 01/11 | 15/11 | Bộ mẫu | Thời gian phản hồi | |
| V08 | Đào tạo 40 cán bộ | IOC | Sở KH&CN | 20/10 | 15/11 | Danh sách đạt | ≥ 80% đạt kiểm tra | |
| V09 | Trình UBND quy chế phối hợp | Giám đốc IOC | Văn phòng UBND | 10/10 | 31/10 | Dự thảo quy chế | Ban hành | |
| V10 | Mở rộng AI toàn bộ lĩnh vực | IOC | Kỹ thuật | 01/12 | 15/12 | Vận hành | Đúng hạn toàn TP | |
| V11 | Đánh giá, báo cáo UBND | IOC | — | 15/12 | 30/12 | Báo cáo | Đúng hạn ≥ 87% | |

---

## Yêu cầu 5 — Bảo mật và nguyên tắc AI an toàn (Phụ lục 3)

**Ẩn danh 3 phản ánh**: đã nêu ở Yêu cầu 1. Quy tắc chung: bỏ định danh trực tiếp (tên, SĐT, CCCD, số nhà, biển số), giữ định danh sự việc (lĩnh vực, tuyến đường, thời gian, tình trạng lặp); ảnh đính kèm che biển số và mặt người trước khi dùng AI nhận dạng.

**Không bao giờ đưa lên AI công cộng**: thông tin người phản ánh; ảnh gốc có mặt người, biển số; toàn văn văn bản chỉ đạo có số hiệu và nội dung nội bộ; danh sách cán bộ xử lý; dữ liệu vị trí chính xác của nhà dân.

**Bốn trục** (từ tệp 04, thêm quy tắc riêng):

| Trục | Quy tắc riêng cho Hue-S |
|---|---|
| Phân quyền dữ liệu | Ẩn danh thực hiện ở hệ thống trước khi tới mô-đun AI; điều phối viên thấy dữ liệu định danh, AI không. Đơn vị xử lý chỉ thấy phản ánh của mình. Mô hình AI chạy trên hạ tầng IOC hoặc dịch vụ có thoả thuận không huấn luyện. |
| Kiểm soát đầu ra | AI gợi ý lĩnh vực, đơn vị, trùng lặp kèm độ tin cậy; dưới 80% bắt buộc xem tay; không tự đóng, tự chuyển, tự phản hồi. Phản hồi tới dân do người ký; ghi rõ có hỗ trợ AI. Đo tỷ lệ gợi ý bị sửa hằng tuần; vượt 15% thì dừng mô-đun. |
| Lưu vết | Mỗi phản ánh lưu: bản gốc (kho định danh), bản ẩn danh, gợi ý AI và độ tin cậy, quyết định điều phối viên, thời điểm từng bước. Nhật ký truy cập kho định danh rà soát tháng. |
| Đào tạo | Điều phối viên học 4 giờ: đọc độ tin cậy, khi nào bác gợi ý, ẩn danh thủ công khi hệ thống lỗi. Cán bộ phường học 2 giờ về dự thảo phản hồi và giới hạn AI. |

Căn cứ: Luật TTNT 134/2025 và NĐ 142/2026 (phân loại rủi ro; hệ thống ảnh hưởng quyền lợi công dân cần đánh giá trước triển khai); Luật BVDLCN 91/2025, NĐ 356/2025; Luật BVBMNN 117/2025; Luật ANM 116/2025; TT 05/2026/TT-BKHCN; CV 557/BKHCN-CĐSQG.

---

## Phần trình bày cách đã dùng AI (Phụ lục 4, nộp kèm)

| STT | Công cụ | Việc | Dữ liệu đưa vào | Không đưa vào | Kiểm chứng |
|---|---|---|---|---|---|
| 1 | Tự làm | Ẩn danh 3 phản ánh | — | Tên, SĐT, CCCD, số nhà | Đối chiếu bảng trước/sau |
| 2 | ChatGPT | Prompt 1 phân tích | Nguồn 2, 3 (tổng hợp), PA-01..03 đã ẩn danh, trích ý văn bản chỉ đạo | Số công văn, toàn văn | Excel tính lại 6 chỉ số: khớp 5, AI tính sai thời gian TB (dùng trung bình cộng 47,1 thay vì trọng số 48,7) → sửa |
| 3 | Claude | Prompt 2 phản biện | Đầu ra 2 + nguồn 2, 3 | — | 7 điểm, xử lý 6, bác 0, hạ cấp 1 (thiếu nhân lực → giả thuyết) |
| 4 | Tự tra | Pháp lý | — | — | Loại NĐ 13/2023 do AI trích; giữ 9 văn bản theo tệp 03 |
| 5 | ChatGPT | Prompt 3 tiến độ | Phương án đã chốt | — | Sửa hạn V09 cho khớp điều kiện áp dụng |

Kết luận cho giám khảo: mọi con số trong báo cáo được Excel tính từ dữ liệu đề; mọi nhận định của AI đều có cột "kiểm bằng dữ liệu"; không có dữ liệu cá nhân nào rời khỏi máy thi.

---

## Tự chấm — chỗ còn yếu

- Số liệu nhân lực và chi phí hoàn toàn giả định; báo cáo đã nói thẳng nhưng nếu đề Bảng C thì cần bảng dự toán chi tiết hơn.
- Bài này chưa có bảng so sánh 3 phương án theo tiêu chí có trọng số như đề Bảng C (chỉ nêu điểm); khi luyện, làm đủ sheet "So sánh phương án".
- Nếu đề thật của Huế cho thêm dữ liệu theo tuần hoặc theo loại thiết bị, cần thêm chiều phân tích mùa vụ (mưa lũ tháng 10–11 ở Huế làm ngập úng tăng).

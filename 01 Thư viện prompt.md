# Thư viện prompt — P0–P14 cho 90 phút

Quy ước:
- `{ĐỀ}` = dán nguyên văn đề thi. `{ĐƠN VỊ}` = tên ngân hàng/phòng ban trong đề (hoặc "một ngân hàng thương mại nhà nước").
- Mỗi prompt dùng **một lần**, chạy theo thứ tự. Đầu ra prompt trước là đầu vào prompt sau.
- Prompt lẻ (P1, P3, P5, P7, P9) chạy ở **ChatGPT**; prompt chẵn phản biện (P4, P13) chạy ở **Claude** với đầu ra của ChatGPT. Đổi chéo cũng được, miễn là **hai mô hình khác nhau** để có "kiểm chứng độc lập".
- Mọi câu trả lời phải giữ hai ký hiệu: `[GIẢ ĐỊNH]` cho số liệu tự đặt, `[CẦN KIỂM CHỨNG]` cho căn cứ pháp lý. Bạn xoá ký hiệu chỉ sau khi đã tra tay.
- Trong phòng thi không có USB: toàn bộ tệp này nằm trong **Claude Project "Hội thi C"** và **Custom GPT**. Trong Project, gọi prompt bằng tên: "Chạy P1 với đề sau: …".
- Quy chế Đ.6 cấm số liệu giả hoặc **lệch với dữ liệu BTC cung cấp**: số liệu đề cho là bất khả xâm phạm; chỉ tự đặt phần đề không có.

---

## P0 — Thiết lập vai (dán đầu mỗi cuộc trò chuyện mới)

```
Bạn là chuyên viên tham mưu cấp phòng tại {ĐƠN VỊ}, có 10 năm kinh nghiệm viết tờ trình, báo cáo đề xuất cho lãnh đạo. Bạn làm việc theo các quy tắc sau, không được vi phạm:
1. Văn phong hành chính Việt Nam: câu ngắn, chủ ngữ rõ, không hoa mỹ, không "hãy cùng", không cảm thán.
2. Số liệu có trong đề bài phải dùng nguyên văn, không làm tròn, không thay thế. Số liệu không có trong đề bài thì phải tự đặt và gắn nhãn [GIẢ ĐỊNH] ngay sau con số.
3. Tên văn bản pháp luật, số hiệu, điều khoản: chỉ nêu khi chắc chắn, và LUÔN gắn nhãn [CẦN KIỂM CHỨNG] để tôi tra lại. Không được bịa số hiệu.
4. Luôn phân biệt rõ "hiện trạng" (có trong đề) và "đề xuất" (do bạn nghĩ ra).
5. Trả lời bằng bảng markdown hoặc danh sách đánh số, không viết đoạn văn dài quá 4 câu.
6. Khi tôi yêu cầu phản biện, bạn phải tìm ít nhất 3 điểm yếu thật sự, không khen.
Xác nhận đã hiểu bằng một dòng, rồi chờ đề bài.
```

---

## KHỐI 1 — PHÂN RÃ BÀI TOÁN

### P1 — Khung bài toán (ChatGPT, phút 3–8)

```
Đề bài:
"""
{ĐỀ}
"""
Phân rã đề bài thành bảng "Khung bài toán" gồm đúng 7 hàng, mỗi hàng 2 cột (Thành phần | Nội dung):
1. Vấn đề cốt lõi (1 câu, nêu được "ai đang chịu thiệt gì vì sao")
2. Mục tiêu (SMART: 2–3 mục tiêu đo được, có số và mốc thời gian; số tự đặt gắn [GIẢ ĐỊNH])
3. Đối tượng tác động (chia 3 nhóm: người dân/khách hàng · cán bộ thực thi · đơn vị phối hợp; mỗi nhóm nêu họ được gì, mất gì)
4. Ràng buộc pháp lý (liệt kê văn bản có thể liên quan, gắn [CẦN KIỂM CHỨNG]; nêu riêng ràng buộc về dữ liệu cá nhân và bí mật ngân hàng nếu có)
5. Ràng buộc nguồn lực (ngân sách, nhân sự, hạ tầng CNTT, thời gian)
6. Dữ liệu cần dùng (bảng con: Tên dữ liệu | Nguồn | Có sẵn hay phải thu thập | Mức nhạy cảm)
7. Tiêu chí đánh giá phương án (5 tiêu chí có trọng số cộng bằng 100%, ví dụ: hiệu quả, chi phí, tính khả thi pháp lý, rủi ro, thời gian triển khai)

Sau bảng, liệt kê 3 câu hỏi mà đề bài chưa nói rõ và bạn phải giả định để làm tiếp, kèm giả định bạn chọn.
```

---

## KHỐI 2 — PHƯƠNG ÁN, SO SÁNH, PHẢN BIỆN

### P2 — Sinh 3 phương án (ChatGPT, phút 8–14)

```
Dựa trên Khung bài toán ở trên, đề xuất đúng 3 phương án theo mức độ thay đổi tăng dần:
- PA1 "Cải tiến tối thiểu": không thay đổi quy trình pháp lý, chỉ dùng AI/công cụ số hỗ trợ cán bộ.
- PA2 "Tái thiết kế quy trình": thay đổi quy trình nghiệp vụ, có AI ở các bước cụ thể, cần sửa quy định nội bộ.
- PA3 "Chuyển đổi toàn diện": tích hợp hệ thống, liên thông dữ liệu liên ngành, cần phối hợp nhiều đơn vị.

Với mỗi phương án, trình bày bảng: Mô tả 3 câu | Các bước quy trình mới (đánh số) | Vai trò của AI ở bước nào (ghi rõ AI làm gì, người quyết định gì) | Nguồn lực (người, tiền [GIẢ ĐỊNH], thời gian) | Rủi ro chính (3 rủi ro) | Điều kiện pháp lý phải thoả [CẦN KIỂM CHỨNG].
Nguyên tắc bắt buộc: AI chỉ đề xuất/dự thảo/phân loại; quyết định cuối cùng và ký duyệt luôn là con người có thẩm quyền.
```

### P3 — Bảng so sánh có trọng số (ChatGPT, phút 14–18)

```
Lập bảng so sánh 3 phương án theo 5 tiêu chí và trọng số đã chốt ở Khung bài toán.
Cột: Tiêu chí | Trọng số | PA1 điểm (1–5) | PA1 lý do 1 câu | PA2 điểm | PA2 lý do | PA3 điểm | PA3 lý do.
Dòng cuối: Điểm tổng có trọng số của mỗi phương án (nêu công thức = Σ trọng số × điểm).
Sau bảng: đề xuất chọn phương án nào, kèm 2 điều kiện để lựa chọn đó đúng, và nêu rõ nếu điều kiện nào không thoả thì rơi về phương án nào.
Xuất thêm bảng này ở dạng CSV (dấu phẩy) để tôi dán vào Excel.
```

### P4 — Phản biện độc lập (CLAUDE, dán đầu ra P1–P3 vào, phút 18–24)

```
Bạn là thành viên hội đồng thẩm định khó tính nhất của {ĐƠN VỊ}, chuyên bác các đề xuất thiếu căn cứ. Dưới đây là khung bài toán, 3 phương án và bảng so sánh do một chuyên viên soạn với sự hỗ trợ của AI:
"""
{dán P1 + P2 + P3}
"""
Hãy phản biện theo 6 mục, mỗi mục tối thiểu 2 ý cụ thể, chỉ vào đúng chỗ trong tài liệu:
1. Lỗi logic hoặc mâu thuẫn nội tại (mục tiêu không khớp tiêu chí, phương án không giải quyết vấn đề cốt lõi…)
2. Số liệu và giả định đáng ngờ: giả định nào nếu sai thì kết luận đổi chiều?
3. Căn cứ pháp lý: văn bản nào có vẻ sai tên/số hiệu/hết hiệu lực, hoặc bị bỏ sót (đặc biệt: dữ liệu cá nhân, bí mật ngân hàng, an toàn thông tin, lưu trữ)?
4. Rủi ro bị bỏ qua (vận hành, con người, pháp lý, uy tín, phụ thuộc nhà cung cấp AI)
5. Chấm điểm thiên vị: điểm nào trong bảng so sánh được cho quá cao/thấp so với lý do?
6. Tính khả thi thực tế tại một ngân hàng thương mại nhà nước (quy trình phê duyệt, đấu thầu, hạ tầng nội bộ, quy định của Ngân hàng Nhà nước)
Kết thúc bằng bảng "Điểm cần sửa": STT | Vấn đề | Mức nghiêm trọng (Cao/Trung/Thấp) | Cách sửa 1 câu.
```

### P5 — Tra pháp lý có chủ đích (ChatGPT hoặc Claude, phút 24–28, chạy song song với tra tay)

```
Với bài toán sau: "{1 câu tóm tắt đề}", tại một ngân hàng thương mại nhà nước ở Việt Nam, năm 2026.
Liệt kê các văn bản pháp luật có khả năng điều chỉnh, chia 4 nhóm: (a) chủ trương về AI/chuyển đổi số, (b) dữ liệu cá nhân và bí mật ngân hàng, (c) an toàn thông tin và an ninh mạng, (d) nghiệp vụ ngân hàng và thể thức văn bản.
Mỗi văn bản: Tên | Số hiệu | Điều khoản liên quan | Nội dung ràng buộc 1 câu | Độ chắc chắn của bạn (Cao/Trung/Thấp).
Đánh dấu [CẦN KIỂM CHỨNG] cho tất cả. Nếu bạn không chắc số hiệu, ghi "không chắc" thay vì đoán.
```
→ Đối chiếu ngay với `03 Căn cứ pháp lý.md`. Văn bản nào không có trong 03 thì tra thuvienphapluat trước khi dùng.

---

## KHỐI 3 — BẢNG TÍNH, DASHBOARD, CHỈ SỐ

### P6 — Dữ liệu và KPI (ChatGPT, phút 28–34)

Hai nhánh, chọn đúng một. Quy chế Đ.6 cấm số liệu lệch với dữ liệu BTC cung cấp.

**P6a — Đề có kèm dữ liệu** (upload file đề; nếu có cột thông tin cá nhân thì ẩn danh hoá trước và ghi nhật ký):

```
File đính kèm là dữ liệu do Ban tổ chức cung cấp. Quy tắc bắt buộc: chỉ dùng dữ liệu trong file; không thêm, sửa, làm tròn hay thay thế bất kỳ dòng hoặc giá trị nào. Nếu cần chỉ số mà file không có cột tương ứng, nói rõ "file không có dữ liệu cho chỉ số này" thay vì tự đặt số.
1. Mô tả file: số dòng, các cột, kỳ dữ liệu, ô trống hoặc giá trị bất thường (liệt kê vị trí, không tự sửa).
2. Bảng KPI: 6 chỉ số then chốt tính được từ file, mỗi chỉ số: Tên | Công thức Excel tính từ các cột | Giá trị hiện trạng | Mục tiêu sau 12 tháng [GIẢ ĐỊNH] | Ngưỡng cảnh báo [GIẢ ĐỊNH].
3. Ước tính hiệu quả phương án: 3 kịch bản (thận trọng / cơ sở / lạc quan) cho 4 chỉ số quan trọng nhất; điểm xuất phát lấy từ file, mức cải thiện gắn [GIẢ ĐỊNH].
Xuất bảng KPI và bảng kịch bản ở dạng CSV. Không xuất lại dữ liệu gốc; tôi dùng file gốc.
```
→ Kiểm tay: chọn ngẫu nhiên 2 giá trị hiện trạng, tính lại bằng công thức Excel trên file gốc.

**P6b — Đề không có dữ liệu**:

```
Đề bài không cung cấp dữ liệu. Hãy thiết kế bộ dữ liệu mô phỏng để đánh giá hiện trạng và đo hiệu quả phương án đã chọn:
1. Bảng dữ liệu thô: 12 dòng (12 tháng gần nhất) × các cột: Tháng | Số hồ sơ/yêu cầu tiếp nhận | Số xử lý đúng hạn | Thời gian xử lý trung bình (ngày) | Số lỗi/trả lại | Số khiếu nại | Giờ công cán bộ | Chi phí (triệu đồng). Số liệu hợp lý, có biến động theo mùa, gắn [GIẢ ĐỊNH] ở tiêu đề bảng.
2. Bảng KPI: 6 chỉ số then chốt, mỗi chỉ số: Tên | Công thức tính từ các cột trên | Giá trị hiện trạng | Mục tiêu sau 12 tháng | Ngưỡng cảnh báo.
3. Ước tính hiệu quả phương án: bảng 3 kịch bản (thận trọng / cơ sở / lạc quan) cho 4 chỉ số quan trọng nhất sau 6 tháng và 12 tháng.
Xuất bảng 1 và 3 ở dạng CSV để tôi dán vào Excel.
```

### P7 — Ý nghĩa quản trị (ChatGPT, phút 40–44, sau khi Excel đã có số)

```
Đây là 6 chỉ số then chốt và giá trị của chúng: {dán bảng KPI}.
Với mỗi chỉ số, viết đúng 3 câu theo cấu trúc: (1) chỉ số này nói lên điều gì về hoạt động; (2) nếu chỉ số vượt/dưới ngưỡng thì lãnh đạo cần quyết định gì; (3) ai chịu trách nhiệm theo dõi và tần suất báo cáo.
Sau đó viết một đoạn 5 câu "Thông điệp cho lãnh đạo" tóm tắt điều dashboard đang nói, kết bằng một kiến nghị hành động.
```

---

## KHỐI 4 — BÁO CÁO THAM MƯU

### P8 — Dự thảo Tờ trình (CLAUDE, phút 45–58, dán tất cả đầu ra đã sửa)

```
Soạn Tờ trình gửi lãnh đạo {ĐƠN VỊ} về việc "{tên phương án đã chọn}", theo đúng dàn ý sau, giữ nguyên tiêu đề các mục, mỗi mục viết vừa đủ, tổng 900–1.200 chữ:
I. Sự cần thiết (hiện trạng có số liệu, hậu quả nếu không làm)
II. Căn cứ pháp lý (chỉ dùng danh sách tôi đưa, không thêm: {dán danh sách đã kiểm chứng})
III. Mục tiêu (từ Khung bài toán)
IV. Nội dung phương án đề xuất (quy trình mới đánh số bước; vai trò AI và vai trò con người ở mỗi bước; hai phương án còn lại nêu 2 câu lý do không chọn)
V. Nguồn lực (nhân sự, kinh phí [GIẢ ĐỊNH], hạ tầng, đơn vị phối hợp)
VI. Rủi ro và biện pháp (bảng: Rủi ro | Khả năng | Tác động | Biện pháp | Đơn vị chịu trách nhiệm) — tối thiểu 5 rủi ro, trong đó bắt buộc có rủi ro về dữ liệu cá nhân, sai lệch đầu ra AI, và phụ thuộc nhà cung cấp
VII. Lộ trình (3 giai đoạn: Thí điểm 3 tháng → Mở rộng 6 tháng → Vận hành chính thức; mỗi giai đoạn: việc, mốc, sản phẩm, tiêu chí đi tiếp)
VIII. Kiến nghị (3 điểm cụ thể lãnh đạo cần quyết)
Văn phong: chủ ngữ là "Phòng…/Ban…", dùng "kính đề nghị", "trân trọng báo cáo". Không dùng gạch đầu dòng trong mục I và VIII.
```

### P9 — Bổ sung lộ trình và nguồn lực chi tiết (ChatGPT, nếu còn thời gian)

```
Từ mục V và VII của tờ trình, lập 2 bảng dán vào phụ lục:
1. Kế hoạch triển khai: Giai đoạn | Công việc | Đơn vị chủ trì | Đơn vị phối hợp | Bắt đầu | Kết thúc | Sản phẩm | Tiêu chí hoàn thành.
2. Dự toán nguồn lực: Hạng mục | Đơn vị tính | Số lượng | Đơn giá [GIẢ ĐỊNH] | Thành tiền | Ghi chú (nêu rõ khoản nào có thể tận dụng hạ tầng sẵn có).
```

---

## KHỐI 5 — AI AN TOÀN

### P10 — Tuỳ chỉnh bộ nguyên tắc (ChatGPT, phút 68–74)

```
Đây là bộ nguyên tắc triển khai AI an toàn chuẩn của tôi: {dán tệp 04}.
Hãy điều chỉnh cho bài toán "{tóm tắt đề}" tại {ĐƠN VỊ}: giữ nguyên 4 trục (phân quyền dữ liệu, kiểm soát đầu ra, lưu vết sử dụng, đào tạo người dùng), nhưng ở mỗi trục thêm 2 quy tắc cụ thể gắn với dữ liệu và quy trình của bài toán này (ví dụ: loại dữ liệu nào tuyệt đối không đưa lên AI công cộng, bước nào bắt buộc người kiểm tra trước khi ban hành). Giữ dạng bảng: Trục | Nguyên tắc | Biện pháp cụ thể | Người chịu trách nhiệm | Bằng chứng kiểm tra.
```

---

## TRỢ LÝ CÔNG VỤ (điểm cộng, phút 74–80)

### P11 — Dựng Custom GPT / Claude Project

Dùng system prompt trong `09 Trợ lý công vụ — system prompt.md`, thay tên đơn vị và bài toán. Nạp file tri thức: tờ trình vừa viết + `03` + `04`. Thử 3 câu hỏi để có ảnh chụp màn hình cho slide.

---

## THUYẾT TRÌNH VÀ RÀ SOÁT

### P12 — Slide 5 trang, 3 phút (ChatGPT, phút 79–82)

```
Từ tờ trình, viết nội dung cho 5 slide, mỗi slide tối đa 5 dòng, mỗi dòng tối đa 12 chữ:
1. Vấn đề và mục tiêu (2 con số đắt nhất)
2. Ba phương án và lý do chọn (bảng điểm rút gọn)
3. Dashboard: 3 chỉ số then chốt và ý nghĩa quản trị
4. Lộ trình, nguồn lực, 3 rủi ro lớn nhất
5. AI an toàn + cách tôi đã dùng và kiểm chứng AI trong bài này (nêu số lần phản biện chéo, số căn cứ đã tra tay)
Kèm lời nói cho mỗi slide, 35 giây/slide.
```

### P13 — Rà soát cuối (CLAUDE, phút 82–85)

```
Đây là toàn bộ bài nộp: {dán tờ trình + bảng KPI + bộ nguyên tắc}. Dữ liệu đề cho: {dán số liệu đề, nếu có}.
Kiểm tra và trả lời dạng danh sách CÓ/KHÔNG kèm vị trí:
0. Có số liệu nào trong bài khác với số liệu đề cho không? (liệt kê từng chỗ lệch)
1. Còn nhãn [GIẢ ĐỊNH] hoặc [CẦN KIỂM CHỨNG] nào chưa được xử lý? (liệt kê)
2. Số liệu ở tờ trình có khớp với bảng KPI không? (liệt kê chỗ lệch)
3. Mỗi mục tiêu ở mục III có ít nhất một chỉ số đo ở dashboard không?
4. Mỗi rủi ro ở mục VI có biện pháp và người chịu trách nhiệm không?
5. Có chỗ nào AI được giao quyền quyết định thay con người không?
6. Có câu nào giọng văn không hành chính (cảm thán, "hãy", "chúng ta cùng")?
7. Thể thức: có đủ số ký hiệu, ngày tháng, nơi nhận, người ký?
```

---

## XUẤT TỆP (thay cho mẫu trên USB)

### P14 — Xuất tệp Word / Excel / PowerPoint theo mẫu (Claude trong Project, khi cần)

```
Dùng mẫu "{05 Mẫu Tờ trình - Báo cáo tham mưu.docx | 06 Mẫu Dashboard.xlsx | 07 Mẫu Slide thuyết trình.pptx}" trong tri thức dự án. Tạo tệp {.docx | .xlsx | .pptx} tên "{tên tệp theo đề}" với nội dung dưới đây, giữ nguyên thể thức, bố cục, phông chữ, công thức của mẫu:
"""
{dán nội dung đã sửa}
"""
Với Excel: mọi ô KPI, tổng, điểm có trọng số phải là công thức tham chiếu sheet Dữ liệu, không ghi giá trị tĩnh.
Không thêm nội dung nào ngoài phần tôi dán.
```
→ Tải về, chuyển ngay vào thư mục `<SBD>`, mở kiểm tra: thể thức, tiếng Việt có dấu, công thức Excel còn chạy. Tệp hỏng → dựng từ tệp trắng, dán nội dung.

---

## Mẹo dùng prompt trong phòng thi

- Mở **2 cửa sổ trình duyệt cạnh nhau**: trái ChatGPT, phải Claude (Project "Hội thi C"). Tab thứ ba: Gemini dự phòng. Không đóng cuộc trò chuyện nào, để còn quay lại; **không xoá lịch sử chat** sau thi (bằng chứng xác minh bài làm, Quy chế Đ.10).
- Không có bộ gõ tiếng Việt → gõ prompt không dấu, thêm "trả lời bằng tiếng Việt có dấu".
- Mỗi đầu ra AI, trước khi dán vào Word/Excel, đọc lướt 20 giây tìm 3 thứ: con số không nhãn, tên văn bản không nhãn, câu "AI sẽ tự động quyết định".
- Bị AI trả lời lan man → thêm vào cuối prompt: "Chỉ trả lời bảng, không mở đầu, không kết luận."
- Bị AI từ chối bịa số → đó là đúng ý; bảo "tự đặt số hợp lý và gắn [GIẢ ĐỊNH]".
- Ghi mỗi lần dùng AI vào Nhật ký **theo mẫu của đề** (không có mẫu thì dùng `02` mục 4) ngay khi chạy, đừng để cuối giờ.

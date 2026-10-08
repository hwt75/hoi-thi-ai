# Checklist kiểm chứng và phản biện độc lập

Thể lệ nói rõ: dùng AI được, nhưng **phải có phần kiểm chứng và phản biện độc lập**. Đây là chỗ giám khảo phân biệt người "biết dùng AI" với người "dán đầu ra AI". Phần này phải **nhìn thấy được trong bài nộp**, không chỉ làm trong đầu.

## 1. Ba tầng kiểm chứng (ghi rõ trong bài là đã làm cả ba)

| Tầng | Ai kiểm | Kiểm gì | Bằng chứng để lại trong bài |
|---|---|---|---|
| 1. Chéo mô hình | AI thứ hai (Claude phản biện ChatGPT hoặc ngược lại) | Logic, giả định, rủi ro bỏ sót, thiên vị chấm điểm | Bảng "Điểm cần sửa" từ P4, kèm cột "Đã xử lý thế nào" |
| 2. Đối chiếu nguồn | Bạn, bằng tay | Số hiệu, tên, hiệu lực văn bản pháp luật; số liệu có trong đề | Mục Căn cứ pháp lý chỉ giữ văn bản đã tra; ghi "tra ngày …/…/2026 tại thuvienphapluat.vn" |
| 3. Kiểm tra nghiệp vụ | Bạn, bằng kinh nghiệm tại đơn vị | Có làm được ở ngân hàng mình không: quy trình duyệt, đấu thầu, hạ tầng, quy định NHNN | Mục Rủi ro và mục "Điều kiện áp dụng" trong tờ trình |

## 2. AI hay sai ở đâu — và cách kiểm nhanh

| AI hay bịa/sai | Dấu hiệu nhận biết | Kiểm trong ≤ 1 phút |
|---|---|---|
| **Số hiệu văn bản** (ví dụ "Thông tư 12/2023/TT-NHNN về AI") | Số hiệu quá tròn trịa, tên quá khớp với câu hỏi | Tra `03 Căn cứ pháp lý.md`; không có → thuvienphapluat.vn, gõ số hiệu; không ra → bỏ |
| **Văn bản đã hết hiệu lực** | Trích Nghị định 13/2023 mà không nhắc Luật Bảo vệ dữ liệu cá nhân 2025; trích NĐ 30/2020 mà không kiểm | Xem cột "Tình trạng" trong `03` |
| **Điều khoản không tồn tại** ("Điều 45 Luật An ninh mạng quy định…") | Trích số điều nhưng không trích nội dung | Mở văn bản, Ctrl+F số điều |
| **Số liệu thống kê** ("theo NHNN, 78% giao dịch…") | Có nguồn mơ hồ, không có năm | Không có trong đề → gắn [GIẢ ĐỊNH], hoặc bỏ |
| **Sửa số liệu của đề** (làm tròn, "chuẩn hoá", thay dòng thiếu bằng số tự đặt) | Số trong bài khác số trong đề; bảng dữ liệu AI xuất lại có số dòng khác file gốc | Dùng file gốc của đề trong Excel, không dùng bản AI chép lại; dò 2–3 giá trị ngẫu nhiên. Quy chế Đ.6 cấm số liệu lệch dữ liệu BTC |
| **Phép tính** (tổng, % thay đổi, điểm có trọng số) | AI tính nhẩm trong văn bản | Bắt Excel tính lại bằng công thức; tờ trình chỉ chép từ Excel |
| **Giao quyền cho AI** ("hệ thống tự động phê duyệt hồ sơ") | Động từ "tự động quyết định/phê duyệt/từ chối" | Sửa thành "AI đề xuất, cán bộ có thẩm quyền quyết định" |
| **Lạc quan về hiệu quả** ("giảm 80% thời gian xử lý") | Không có kịch bản thận trọng | Bắt buộc 3 kịch bản (P6), tờ trình dùng kịch bản cơ sở |
| **Giọng văn** ("Hãy cùng nhau…", "vô cùng cấp thiết") | Cảm thán, khẩu hiệu | P13 mục 6; sửa tay |
| **Rủi ro chung chung** ("rủi ro kỹ thuật") | Không có chủ thể, không có biện pháp | Mỗi rủi ro phải có: khả năng · tác động · biện pháp · người chịu trách nhiệm |
| **Đối tượng tác động thiếu** | Chỉ nói khách hàng, quên cán bộ thực thi và đơn vị phối hợp | P1 hàng 3 bắt buộc 3 nhóm |

## 3. Checklist tự chấm sau mỗi lần luyện (và 5 phút cuối giờ thi)

### Khối 1 — Phân rã
- [ ] Vấn đề cốt lõi viết được trong 1 câu, có chủ thể chịu thiệt
- [ ] Mục tiêu có số và mốc thời gian
- [ ] Đủ 3 nhóm đối tượng tác động, mỗi nhóm có "được/mất"
- [ ] Ràng buộc pháp lý tách riêng nhóm dữ liệu cá nhân / bí mật ngân hàng
- [ ] Bảng dữ liệu cần dùng có cột "mức nhạy cảm"
- [ ] Tiêu chí đánh giá có trọng số cộng đúng 100%

### Khối 2 — Phương án & phản biện
- [ ] Đúng 3 phương án, mức thay đổi tăng dần, mỗi phương án nêu AI làm gì / người làm gì
- [ ] Bảng so sánh có điểm, lý do, tổng có trọng số (tính bằng Excel)
- [ ] Có bảng "Điểm cần sửa" từ mô hình thứ hai, kèm cột đã xử lý
- [ ] Có câu "điều kiện để lựa chọn này đúng; nếu không thoả thì rơi về PA…"

### Khối 3 — Dashboard
- [ ] Sheet Dữ liệu: nguồn hoặc nhãn [GIẢ ĐỊNH] ở tiêu đề
- [ ] Đề có dữ liệu → sheet Dữ liệu là **dữ liệu gốc của đề, không sửa giá trị nào**; số tự đặt (nếu có) để sheet riêng, gắn [GIẢ ĐỊNH]
- [ ] Sheet KPI: mọi ô số là công thức, không gõ tay
- [ ] Sheet Dashboard: ≥ 3 biểu đồ, mỗi biểu đồ có tiêu đề nói được kết luận (không phải "Biểu đồ 1")
- [ ] Mỗi KPI có 3 câu ý nghĩa quản trị: nói gì · quyết gì · ai theo dõi
- [ ] Có 3 kịch bản hiệu quả (thận trọng / cơ sở / lạc quan)

### Khối 4 — Tờ trình
- [ ] Đủ thể thức: tên cơ quan, số/ký hiệu, địa danh ngày tháng, tên loại + trích yếu, nơi nhận, chức vụ người ký
- [ ] Đủ 8 mục I–VIII; mục II chỉ chứa văn bản đã tra
- [ ] Nguồn lực có người + tiền + hạ tầng + đơn vị phối hợp
- [ ] ≥ 5 rủi ro, có rủi ro dữ liệu cá nhân, sai lệch AI, phụ thuộc nhà cung cấp
- [ ] Lộ trình 3 giai đoạn có tiêu chí "đi tiếp"
- [ ] Số liệu trong tờ trình khớp Excel

### Khối 5 — AI an toàn
- [ ] Đủ 4 trục: phân quyền dữ liệu · kiểm soát đầu ra · lưu vết · đào tạo
- [ ] Mỗi trục có biện pháp cụ thể + người chịu trách nhiệm + bằng chứng kiểm tra
- [ ] Có phân loại dữ liệu (công khai / nội bộ / mật / dữ liệu cá nhân) và quy tắc "cái gì không được đưa lên AI công cộng"
- [ ] **Nhật ký sử dụng AI của chính bài thi** được đính kèm (mục 4 dưới đây)

### Tổng thể
- [ ] Không còn nhãn [GIẢ ĐỊNH]/[CẦN KIỂM CHỨNG] chưa xử lý (nhãn [GIẢ ĐỊNH] được phép giữ, nhưng phải có chú thích "số liệu giả định để minh hoạ")
- [ ] Không có chỗ nào AI quyết định thay người
- [ ] Mọi số liệu trong tờ trình, slide, Excel khớp dữ liệu đề cho
- [ ] Nhật ký AI đúng mẫu đề yêu cầu, ghi rõ không đưa dữ liệu không được phép lên AI
- [ ] Mọi tệp nằm trong thư mục `<SBD>`, tên và định dạng đúng đề, tên tệp không chứa mật khẩu; đã nén **1 file duy nhất** và nộp trên PTIT client; đã đọc thông tin xác nhận

## 4. Mẫu Nhật ký sử dụng AI (đính kèm bài thi — chứng minh "lưu vết")

Đây là bằng chứng sống cho tiêu chí 5. Điền ngay khi chạy mỗi prompt, không để cuối giờ.
Quy chế Đ.7: **yêu cầu nhật ký AI được ghi trong đề thi** → đề có mẫu thì làm theo mẫu đề; mẫu dưới đây chỉ dùng khi đề không quy định, hoặc để bổ sung cột đề thiếu.

| STT | Thời điểm | Công cụ | Mục đích (prompt số) | Đầu vào có dữ liệu nhạy cảm không? | Đầu ra được dùng thế nào | Kiểm chứng bởi | Kết quả kiểm chứng |
|---|---|---|---|---|---|---|---|
| 1 | 09:05 | ChatGPT | P1 Khung bài toán | Không (đề bài công khai) | Dùng sau khi sửa tiêu chí | Claude (P4) + tự kiểm | Sửa 2 trọng số |
| 2 | 09:12 | ChatGPT | P2 Ba phương án | Không | Dùng PA2 làm chính | Claude (P4) | Bổ sung rủi ro nhà cung cấp |
| 3 | 09:20 | Claude | P4 Phản biện | Không | Bảng 7 điểm cần sửa, xử lý 6, bác 1 (lý do…) | Tự kiểm | — |
| 4 | 09:26 | Tự tra | Pháp lý | — | Giữ 6 văn bản, loại 2 (không tìm thấy trên thuvienphapluat) | Tự tra | ghi ngày tra |
| … | | | | | | | |

Nguyên tắc ghi: (1) không đưa dữ liệu khách hàng thật vào AI công cộng, kể cả khi đề cho; nếu đề cho dữ liệu cá nhân thì ẩn danh hoá trước và ghi vào nhật ký; (2) mỗi đầu ra AI có ít nhất một dòng kiểm chứng; (3) nêu cả điểm phản biện bị bác và lý do, để chứng minh có tư duy độc lập chứ không nghe AI vô điều kiện.

## 5. Câu hỏi giám khảo có thể hỏi — và cách trả lời

Bảng C không thuyết trình, nhưng Quy chế Đ.10 cho phép BTC **yêu cầu giải thích, thao tác lại trên bản sao bài làm** khi cần xác minh. Luyện trả lời các câu dưới đây sau mỗi buổi luyện; giữ lịch sử chat AI đến khi công bố kết quả.

| Câu hỏi | Ý trả lời |
|---|---|
| "Số này ở đâu ra?" | Nếu giả định: nói thẳng là giả định để minh hoạ, và chỉ ra chỗ trong Excel có thể thay số thật; nêu số thật sẽ lấy từ hệ thống nào |
| "Sao biết AI không bịa?" | Chỉ vào Nhật ký và bảng Điểm cần sửa; nêu số văn bản đã tra tay và số văn bản đã loại |
| "AI sai thì ai chịu trách nhiệm?" | Theo bộ nguyên tắc: AI chỉ đề xuất; người ký chịu trách nhiệm; có lưu vết để truy |
| "Dữ liệu khách hàng đưa lên ChatGPT thì sao?" | Không đưa; phân loại dữ liệu ở trục 1; lộ trình có bước dùng AI nội bộ/ trên hạ tầng riêng cho dữ liệu mật |
| "Nếu không có ngân sách thì sao?" | PA1 là phương án tối thiểu, không cần đầu tư; điều kiện rơi về đã nêu ở bảng so sánh |
| "Phương án này có trái quy định nào không?" | Nêu 2–3 văn bản ràng buộc chính và cách phương án tuân thủ; thừa nhận điểm cần xin ý kiến pháp chế |

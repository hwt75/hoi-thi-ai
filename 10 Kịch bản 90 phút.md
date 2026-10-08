# Kịch bản 90 phút — phân bổ từng phút

Nguyên tắc: **có sản phẩm nộp được ở phút 60**. Từ phút 60 trở đi chỉ nâng cấp. Nếu đến mốc mà chưa xong, chuyển tiếp, quay lại sau nếu còn giờ.

## Trước giờ thi (theo Quy chế)

| Thời điểm | Việc |
|---|---|
| ≥ 30 phút trước | Có mặt, xuất trình thẻ dự thi / CCCD, ngồi đúng SBD. Kiểm tra máy cùng tổ kỹ thuật: Office bản nào, bộ gõ tiếng Việt, thư mục lưu bài, PTIT client chạy. Bất thường → báo ngay |
| 15 phút trước | Dùng điện thoại đăng nhập theo thứ tự: **Claude → ChatGPT → Google/Gemini → thuvienphapluat** (nếu có tài khoản). Tick "duy trì đăng nhập". Mỗi công cụ gửi thử 1 câu. Mở Claude Project "Hội thi C" và Custom GPT. Dán P0 vào ChatGPT |
| Hết 15 phút | Tắt điện thoại, bỏ vào bì thư ghi SBD, nộp giám thị |
| Chờ hiệu lệnh | **Không làm bài trước hiệu lệnh**. Được phép: tạo thư mục `<SBD>` ở vị trí giám thị chỉ định (nếu giám thị đã thông báo) |

Từ phút 0: mọi tệp **lưu thẳng vào thư mục `<SBD>`**. Tệp tải từ AI về (thường nằm ở Downloads) chuyển ngay vào thư mục này. Mẫu Word/Excel không có sẵn trên máy → nhờ Claude xuất tệp từ mẫu trong Project, hoặc dựng từ tệp trắng. Nhật ký AI ghi **theo mẫu của đề**; đề không có mẫu thì dùng mẫu ở `02` mục 4.

| Phút | Việc | Công cụ | Sản phẩm sau bước |
|---|---|---|---|
| 0–3 | Đọc đề 2 lần. Gạch chân: đối tượng, dữ liệu đề cho, yêu cầu nộp, đơn vị. Ghi 1 câu "đề đòi gì" ra giấy | Giấy | Hiểu đề |
| 3–8 | **P1** Khung bài toán. Sửa trọng số tiêu chí theo ý mình | ChatGPT | Bảng 7 hàng → dán vào Word mục I–III và phụ lục |
| 8–14 | **P2** Ba phương án | ChatGPT | Bảng 3 phương án |
| 14–18 | **P3** Bảng so sánh + CSV | ChatGPT | CSV → dán vào sheet "So sánh phương án" của Excel, để Excel tính tổng |
| 18–24 | **P4** Phản biện chéo. Đọc bảng Điểm cần sửa, đánh dấu: sửa / bác (ghi lý do) | Claude | Bảng Điểm cần sửa có cột "Đã xử lý" → phụ lục |
| 24–28 | **P5** + tra tay pháp lý. So với `03`. Chốt danh sách 5–8 văn bản | Claude + thuvienphapluat | Danh sách căn cứ đã kiểm |
| 28–34 | **P6** Dữ liệu và KPI. Đề có dữ liệu → **chỉ dùng dữ liệu đề**, không sinh số thay thế (Quy chế Đ.6) | ChatGPT | CSV → sheet "Dữ liệu" |
| 34–40 | Excel: kiểm công thức KPI chạy đúng với dữ liệu mới; chỉnh 3 biểu đồ; đặt tiêu đề biểu đồ dạng kết luận | Excel | Dashboard chạy |
| 40–44 | **P7** Ý nghĩa quản trị | ChatGPT | Dán vào sheet "Ý nghĩa quản trị" và mục IV tờ trình |
| 44–45 | **Lưu tất cả. Ghi nhật ký AI dòng 1–7** | | Mốc an toàn 1 |
| 45–58 | **P8** Tờ trình. Dán vào mẫu Word, giữ thể thức. Sửa tay: số liệu khớp Excel, tên đơn vị, giọng văn | Claude + Word | Tờ trình đủ 8 mục |
| 58–60 | **Lưu vào thư mục `<SBD>`, đặt tên đúng đề. Có thể nộp được từ đây.** Nếu BTC cho nộp nhiều lần: nén và nộp thử bản đầu | | Mốc an toàn 2 |
| 60–68 | Đọc lại tờ trình một lượt, sửa số, sửa câu. Chèn bảng so sánh và bảng rủi ro | Word | Tờ trình sạch |
| 68–74 | **P10** Bộ nguyên tắc AI an toàn tuỳ chỉnh → phụ lục 3. Nhật ký AI → phụ lục 4 | ChatGPT + Word | Đủ 5 khối |
| 74–79 | **Phụ lục 5: Prompt đã dùng** — dán nguyên văn các prompt chính (P1, P2, P4, P8) và 2 câu về cách kiểm chứng mỗi đầu ra. Ban tổ chức yêu cầu chấm prompt và chấm kiểm chứng | Word | Bằng chứng cho giám khảo |
| 79–82 | **P12** Slide 5 trang (nhờ AI xuất .pptx theo mẫu `07` trong Project), chèn ảnh dashboard. Không có thuyết trình ở Bảng C, slide là sản phẩm nộp. Đề không đòi slide → bỏ | ChatGPT/Claude + PowerPoint | Slide |
| 82–85 | **P13** Rà soát cuối. Sửa những gì trả lời "CÓ". Kiểm riêng hai điểm liệt: có dữ liệu không được phép nào đã đưa lên AI? có nội dung AI nào chưa kiểm chứng mà viết như sự thật hoặc lệch dữ liệu đề? | Claude | Bài sạch |
| 85–88 | **Chốt nộp**: đủ tệp trong `<SBD>`, tên và định dạng đúng đề, tên tệp không chứa mật khẩu → chuột phải thư mục → *Compress to ZIP file* → nộp trên PTIT client → đọc thông tin xác nhận, thiếu tệp báo ngay giám thị | Windows + PTIT client | Đã nộp |
| 88–90 | Dự phòng. Hiệu lệnh hết giờ là dừng sửa. Ký xác nhận bài nộp rồi mới rời phòng | | Xong |
| dư giờ | **P11** Custom GPT "Trợ lý công vụ", chụp màn hình chèn slide 5. Chỉ làm khi mọi thứ trên đã xong | ChatGPT | Điểm cộng |

## Nếu đề khác kỳ vọng

| Tình huống | Điều chỉnh |
|---|---|
| Đề cho **file dữ liệu lớn** | Phút 28–40 thành 28–46: upload lên ChatGPT (ẩn danh hoá cột cá nhân trước, ghi nhật ký), yêu cầu tính KPI và xuất CSV; bỏ P9 |
| Đề đòi **quy trình nghiệp vụ** thay vì chính sách | Mục IV tờ trình thành sơ đồ bước (bảng: Bước | Ai | Làm gì | AI hỗ trợ gì | Kiểm soát | Thời gian); P2 vẫn dùng |
| Đề đòi **cải tiến dịch vụ công** (hướng người dân/khách hàng) | Đối tượng tác động nhóm 1 là trọng tâm; KPI thêm: thời gian chờ, tỷ lệ hài lòng, tỷ lệ làm trực tuyến toàn trình |
| Đề **liên ngành** (ngân hàng + BHXH/thuế/công an…) | Thêm hàng "Cơ chế phối hợp, chia sẻ dữ liệu" trong P1; rủi ro thêm "không thống nhất được chuẩn dữ liệu"; căn cứ thêm Luật Dữ liệu 2024 |
| Đề đòi nộp **slide** thay vì tờ trình | Slide 8–10 trang theo 8 mục tờ trình; vẫn làm Excel |
| Đề bắt **xây trợ lý/agent** | P11 lên phút 45–60; tờ trình rút còn 5 mục (I, III, IV, VI, VIII); trợ lý phải có: system prompt, tri thức nạp, 3 ví dụ hội thoại, giới hạn không trả lời, cách lưu vết |
| Một công cụ AI bị đăng xuất / hết lượt | Không đăng nhập lại được (điện thoại đã nộp). Chuyển sang công cụ còn lại hoặc Gemini; phản biện chéo chạy ở phiên mới (xem tệp 11). Ghi nhật ký "Claude/ChatGPT không khả dụng từ phút…". Lỗi do hệ thống → báo giám thị |
| Mất mạng / máy lỗi | **Giữ nguyên hiện trạng, giơ tay báo giám thị**. Không tự khởi động lại, không chuyển máy (Quy chế Đ.8). Quá 5 phút BTC quyết định bù giờ / đổi máy. Trong lúc chờ: viết tay dàn ý ra giấy nháp |
| AI lỗi nhưng máy chạy | Điền tay theo dàn trong `10`/`01`; ghi vào nhật ký "AI không khả dụng từ phút…" |
| Máy không có Office / Office cũ | Nhờ AI xuất tệp .docx/.xlsx, hoặc dùng Google Docs/Sheets rồi tải về định dạng đề đòi. **Không chia sẻ link, không mở quyền cộng tác** |
| Không có bộ gõ tiếng Việt | Không tự cài Unikey (cấm). Gõ prompt không dấu, yêu cầu AI trả lời có dấu; sửa tay tối thiểu. Hỏi giám thị trước giờ thi |

## Bốn câu tự nhắc

1. Phút 45 phải có Excel chạy. Phút 60 phải nộp được. Phút 85 bắt đầu nén và nộp.
2. Mỗi đầu ra AI: tìm số không nhãn, văn bản không nhãn, câu giao quyền cho AI, số lệch dữ liệu đề.
3. Không đưa dữ liệu khách hàng thật hay tài liệu nội bộ lên AI công cộng, dù đề cho. Vi phạm là **đình chỉ thi**.
4. Hiểu mọi thứ mình nộp: BTC có thể yêu cầu giải thích, thao tác lại (Quy chế Đ.10).

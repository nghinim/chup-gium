# Chụp Giùm

App web giúp người chụp chưa quen căn góc chụp ảnh giúp Nghi dễ hơn.

Mở trên iPhone bằng Safari: https://nghinim.github.io/chup-gium/

## Có gì

- 9 dáng mẫu đo từ ảnh tham khảo thật, kèm khung outline và câu chỉ dẫn cho người cầm máy
- Khung ngắm có lưới chia ba, vạch mốc khoảng trống trên đầu và vạch chân, thước cân máy
- Trợ lý căn khung: nhận dạng dáng người trực tiếp rồi nhắc tiến lại gần, lùi ra xa, nâng máy, hạ máy, dịch trái phải; khớp thì khung chuyển xanh
- Tự bấm khi khớp: giữ đúng khung hơn một giây thì tự chụp ba tấm
- Đọc chỉ dẫn thành tiếng Việt
- Chế độ "Đưa máy cho bạn": giấu bớt nút, chỉ còn khung ngắm, chỉ dẫn in to và nút chụp
- Import ảnh tham khảo riêng để phủ mờ lên camera; ảnh nằm trong máy, không gửi đi đâu

## Kỹ thuật

Một file `index.html` duy nhất, không cần build. Nhận dạng dáng dùng MediaPipe Pose Landmarker
chạy ngay trong trình duyệt, model tải từ CDN lần đầu rồi cache lại.

Camera chỉ chạy trên HTTPS và phải mở ở tab riêng, không nằm trong khung nhúng.

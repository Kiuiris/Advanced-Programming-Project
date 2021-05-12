# Advanced-Programming-Project

Bài tập lớn của mình cho lớp Lập trình nâng cao INT2215 22.
Đây là một game nhỏ có tên Catch 'Em All, dựa theo game hứng trứng.

Video Demo: https://youtu.be/M6YfXbo4CKw (Mở phụ đề để đọc phần giới thiệu)

- Mục tiêu của game: Hứng được càng nhiều đồ vật càng tốt trong khoảng thời gian cho phép. Trong phần Options ngoài menu sẽ có lựa chọn 3 giao diện khác nhau và 3 mốc thời gian khác nhau (30 giây, 60 giây và 90 giây).

- Mô tả: Sau khi nhấn play, các đồ vật (khác nhau tuỳ theo themes khác nhau) sẽ rơi xuống. Người chơi sử dụng hai phím trái phải để di chuyển vật hứng để đỡ được càng nhiều đồ càng được điểm cao.

- Mức điểm tự đánh giá: 8,5 - 9
- Quá trình làm game:
1. Lên ý tưởng: mình có một vài ý tưởng game khác nhau cho bài tập lớn. Sau khi xem qua SDL mình chốt ý tưởng làm game này.
2. Triển khai: mình làm logic của game trước rồi chia nhỏ thành các file tuỳ theo mục đích
  - SDL_Utils: file này gồm các hàm thường dùng của SDL, mình lấy từ code mẫu cô đưa (link dẫn bên dưới) và thêm bớt một số hàm cho phù hợp
  - Game_Utils: chứa các hàm chức năng của game. Hầu hết là cho các nút bấm của menu, cho việc render điểm...
  - SFX: chứa các hàm quản lí âm thanh của game
  - Button: chứa struct Button dùng để khởi tạo các nút của menu và cuối game
  - LTimer: chứa struct thời gian để quản lí việc tính thời gian của game, được lấy từ code của Lazyfoo
  - Catcher: chứa struct Catcher quản lí các chức năng của vật hứng
  - Object: chứa struct Object, chủ yếu để khởi tạo vật

- Code tham khảo:
Code mẫu Snake (tham khảo cách chia files và file SDL_Utils)
Code Dino in Zungle (tham khảo cách dựng game và chia files)
Code về SDL của LazyFoo

Ngoài hai files SDL_Utils và LTimer, toàn bộ phần code còn lại là do mình tự viết.

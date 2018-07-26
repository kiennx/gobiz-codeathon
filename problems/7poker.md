## Đề số 007

Đối với các team Agile, việc estimate bằng Planning Poker là không thể thiếu. Như chúng ta thì đã có bộ bài, nhưng nhiều team khác thì không có điều kiện hoặc không làm được việc này. Gobiz trong quá trình giao lưu với các đơn vị khác quyết định xây dựng một công cụ chơi Planning Poker miễn phí để phục vụ cộng đồng Agile Việt Nam!

Yêu cầu:
- Sử dụng bộ planning poker dựa trên Fibonacci mở rộng (bộ hiện tại chúng ta đang sử dụng)
- User có khả năng tạo một room, các người chơi khác có thể join vào
- Có thể tạo ra các game (tương đương đánh giá point cho 1 US)
- Mỗi game bao gồm nhiều session (mặc định 3 session)
- Mỗi session kéo dài 1 khoảng thời gian, những player nào không đưa ra quyết định trong thời gian này sẽ tính là pass (mặc định 30 giây)
- Sau khi hết giờ mới mở bài của tất cả người chơi, nếu tất cả cùng chọn 1 lá bài thì sẽ kết thúc game, kết quả là con số được chọn. Nếu không, sau mặc định 3 session như vậy sẽ lấy theo số đông. Trong trường hợp có 2 hoặc nhiều lá bài bằng nhau thì sẽ dựa vào lịch sử các lần trước để lấy số đông. Nếu vẫn bằng nhau thì lấy lá bài lớn nhất.
- Tất cả các con số "mặc định" ở trên có thể custom khi tạo game
- Khi kết thúc game, tạo game mới thì sử dụng các thông số ở lượt trước
- Realtime playing
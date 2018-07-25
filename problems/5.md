## Đề số 005

Hiện tại đã đến thời điểm Gobiz mở rộng dịch vụ ra cho nhiều đối tượng khách hàng tiềm năng khác nhau. Khách hàng của Gobiz chủ yếu sẽ là các doanh nghiệp vừa nhỏ, những người tổ chức bán hàng online, đặc biệt là các shop trên các trang thương mại điện tử phổ biến ở Việt Nam (cũng như sau này là quốc tế).

Để thu thập thông tin khách hàng tiềm năng, Gobiz có nhu cầu xây dựng một bộ crawler đi lấy thông khách hàng trên các nguồn là các trang thương mại điện tử này. Tuy nhiên, dữ liệu sau khi crawl được từ nhiều nguồn khác nhau thì khác là khác biệt, ví dụ có site thì lấy được tên shop, email, điện thoại - có site thì lấy được tên shop, điện thoại, địa chỉ... Các thông tin có thể lấy ra được này các bạn tự dự đoán, tìm hiểu hoặc/và liên hệ với team làm đề số 004 để gia tăng độ chính xác.

Với lượng thông tin như vậy, sẽ có rất nhiều khách hàng vốn là trùng nhau (cùng 1 người hoặc cùng 1 shop). Gobiz sẽ cần xây dựng công cụ để gộp những thông tin trùng nhau này lại.

Yêu cầu:
- Từ dữ liệu ban đầu (các thông tin không đầy đủ về người, shop, trong đó sẽ unique theo nguồn thông tin - ví dụ shopee) có thể tự động khớp những chủ thể cùng là một vào
- Nếu với các dữ kiện chưa thể khẳng định 2 đối tượng là cùng 1 khách hàng, cần phải có UI cho phép thể hiện những trường hợp "có khả năng cao là trùng" (có trọng số) và người dùng có vể view so sánh 2 thông tin sau đó xác nhận là trùng hay không. Nếu đã để là "không trùng" sẽ không xuất hiện lại trong danh sách suggest này nữa.
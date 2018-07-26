## Đề số 001

Gobiz hiện đang xây dựng rất nhiều dự án khác nhau, điểm chung là tất cả các dự án này đều sử dụng React để làm Client. Và trong các dự án này có rất nhiều những thao tác UI/UX giống hệt nhau ví dụ như có các bảng biểu, có chức năng download, có select,...

Để giải quyết vấn đề các thành phần dùng chung này không cần phải sao chép qua lại giữa nhiều dự án khác nhau, Gobiz quyết định tự làm một bộ thư viện UI để sử dụng chung giữa các dự án.

Bộ UI này cần:
- Viết dưới dạng thư viện độc lập, để có thể đưa lên private repo cung cấp cho các dự án nội bộ khác sử dụng
- Có thể cung cấp các component như sau (lựa chọn một hoặc nhiều component để làm, không cần làm hết, nhưng càng nhiều sẽ càng được nhiều điểm)

Các component như sau:
1. Download progress bar: 
	- có thể request đến API download
	- thể hiện tình trạng download (% hoàn thành, thời gian dự kiến,...), hỗ trợ download nhiều file cùng lúc - khi ấy sẽ download tuần tự (số lượng file download song song cần cấu hình được).
2. Select:
	- select có thể enable filter (tìm kiếm trong danh sách - hỗ trợ cả tìm kiếm client-side lẫn server-side)
	- giá trị khi select được và giá trị hiển thị có thể khác nhau (value <> text)
	- từng item trong select có thể disable (vẫn hiển thị nhưng không chọn được)
	- cho phép bật/tắt việc thể hiện item đang được select bằng icon
3. Number input
	- chỉ cho phép nhập số và dấu phân cách thập phân
	- format lại input để hiển thị số với format cả phân cách hàng nghìn và phân cách thập phân
	- có thể custom format (dấu phân cách là gì, số lượng số đằng sau dấu phân cách thập phân)
4. Switch
	- Checkbox nhưng thể hiện dạng switch on/off
5. Date Picker
	- Hỗ trợ đa ngôn ngữ
	- Có thể custom format ngày tháng hiển thị ra
	- Cho phép lựa chọn có Time Picker hay không

**Yêu cầu đặc biệt: không sử dụng các thư viện có các component trên sẵn, chỉ sử dụng các thư viện tối thiểu của React. Làm tương thích trên cả React-Native là một điểm cộng.**
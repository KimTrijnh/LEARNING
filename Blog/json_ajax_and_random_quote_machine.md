# Sử dụng JSON và AJAX trong RANDOM QUOTE MACHINE PROJECT của FreeCodeCamp.

Là một người mới tự học javascrip theo chương trình của FCC, khi đến 1st project của JS mình đã rất rối rắm vì ko hiểu JSON, AJAX, API là gì?
Nó có nhiệm vụ gì cho project này và làm thể nào để tạo ra nó. Yêu cầu của project là xuất ra ngẫu nhiên 1 quote mỗi khi bấm nút "new quote".
Trình độ đơn giản thì chỉ cần làm ngẫu nhiên cho quote, nhưng mình thấy có nhiều coder còn chạy cả ngẫu nhiên background, kèm theo tác giả của quote
mỗi khi quote thay đổi. những quote này được collect như thế nào, tạo biến array rồi manually nhét chúng vô array hay sao?
Dùng JSON, AJAX có lược bỏ được những bước này hay ko? Rối tung rối mù cả lên. Thế rồi mình đành tạm gác lại project và tìm hiểu JSON, AJAX,API
Bài viết này để cho những người mù IT như mình, không bị bỡ ngỡ mà bỏ cuộc, có thể có 1 bước đầu tham khảo về JSON, AJAX và ứng dụng và tạo cái 
RANDOM QUOTE MACHINE. 

Dưới đây là các useful source về JSON:
- https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON
- checkJSON error https://jsonlint.com/

Túm gọn:
1. JSON là gì?
- JSON: javascript object notation
- là 1 file text đơn giản, gọn, human readable dùng để chứa thông tin như objects, array, varibale. Nhưng vì đơn giản nó không chứa được method hay function. 
- Có syntax tương tự như javascrip object/array nên dễ viết, cách truy xuât các đối tượng/propery cũng tương tự như javascript. 
- Để chuyển đổi syntax giữa JS và JSON ta dùng method stringify / parse trong JS. 

2. Vậy JSON dùng để làm gì, và chỗ nào tốt mà ta nên dùng nó?
- Để chứa thông tin. objects sẽ được viết dưới dạng json và lưu dưới file tenfile.json
- Vì nó dễ đọc, truy xuất đơn giản. Kết hợp với phương pháp load thông tin bất đồng bộ (AJAX), ta có thể load 1 mẩu thông tin từ sever về bằng JS mà ko cần phải load cả page.

3. Cách tạo và load file JSON:
- đọc trong link https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON

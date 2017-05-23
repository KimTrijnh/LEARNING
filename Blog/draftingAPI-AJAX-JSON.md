### HƯỚNG DẪN API-AJAX-JSON CƠ BẢN (drafting)

[web App bất kỳ cung cấp ** API tool ** cho phép người khác access vô data của họ, data này sẽ có dạng file info (vd. JSON, XML, JSONP)
- ví dụ: facebook API, twitter API, openweather API...
- Cách sử dụng API của họ sẽ được giải thích trong API document, bao gồm cả cấu trúc file info.
- Thường user sẽ được cung cấp 1 API key, hướng dẫn sử dụng API key tìm trong API document của nhà cung cấp ]

[ AJAX - bất đồng bộ- là 1 phương thức để transfer data về client server. 
[đọc thêm](). Ta dùng AJAX để load data từ 1 remote server về local server]

[ Phần còn lại là viết Js và Jquery cho ajax get/post data với server chứa file info cần sử dụng]


### Tutoral
1. Sử dụng API
Ở đây mình sẽ sử dụng openweather API để tạo current weather app (link:demo), vào https://openweathermap.org/api
Chọn current weather data: 
- Hướng dẫn sử dụng weather data API doc: 
- signup để lấy API key
- Hướng dẫn sử dụng API key
Sau khi đọc qua các phần trên mình có API key là "12345",trong phần hướng dẫn sử dụng API key->ulr:"...apikey"(ulr này sẽ được dùng trong JS để truy cập vào data- phần JS/jquery), trong phần API doc-> giới thiệu cấu trúc file JSON của họ, ở đây mình chọn cách sử dụng tọa độ. 
=> Link api mình cần sẽ có dạng http://.....;


2. Sử dụng JS/JQuery để get file.

- Nếu dùng JS

- Nếu dùng Jquery


## Beginning
### Responsive là gì?? và tại sao phải responsive
Responsive design nghĩa là thiết kế web cho sử dụng được với tất cả các loại màn hình và thiết bị. 
  Một số điểm được cho là không nên khi thiết kế: 
  -  Người dùng phải zoom để đọc được nội dung
  -  Người dùng phải scroll ngang để đọc được trọn vẹn nội dung
  -  Layout không cân đối và ko tự thay đổi khi thay đổi thiết bị xem.
  
### Vậy làm thế nào để reponsive gọn gẽ, từ đầu đến đuôi. 

#### Quy tắc cơ bản:
  - Sử dụng relative length (%, em, vh, vw...) thay vì dùng absolute length (px,...). Giúp tạo ra 1 flexible layout và các component khác tự điều chỉnh khi kích thước màn hình thay đổi. 
  - Sử dụng media query tương đương cho các kích thước khác nhau. 
  - Sử dụng các kỹ thuật tạo layout: grid/flexbox. 
  - Hoặc sử dụng các framework có 1 hệ thống grid tối ưu: ví dụ bootstrap, foundation, etc...
  
## Step-by-step layout design

### Layout & modules
1. setting the viewport
  ```
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ```
  Giải thích: 
  - thẻ meta
  - 
  - 
 2. Nếu không sử dụng framework có sẵn grid system, thì tự set grid
  -  Nên set box-sizing về box-border, tiện cho việc set height và width sau này
  ```
  * {
    box-sizing: border-box;
   }
   ```
  -  Grid chia theo 12 cột của w3: https://www.w3schools.com/css/css_rwd_mediaqueries.asp
  
 3. Tiếp theo dùng media query theo kích thước screen khác. ( tạo break points)
  - Ưu tiên thiết kế mobile first
  - màn hình cho table 
  ```@media only screen and (min-width: 600px)```
  - màn hình cho desktop
  ```@media only screen and (min-width: 768px) ```
  - lanscape mode 
  ```@media only screen and (orientation: landscape)```

 ### Các components khác
 1. image/video
 ```
 img/video {
    max-width: 100%;
    height: auto;
 }
```
  -  img background
  - sử dụng `min-device-width` thay vì `min-width`
  ```
  @media only screen and (min-device-width: 400px)
  ```
 



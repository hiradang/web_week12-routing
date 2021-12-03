1. Cài đặt các module cần thiết
    $ npm i
2. Khởi chạy server
    $ npm start
    Một pop-up sẽ hiện lên thông báo rằng ứng dụng đang chạy ở port 3000.
    Chọn "Open browser" để follow đến trang chạy ứng dụng. Tại đây sẽ thực hiện các thao tác như bình thường.
3. Truy cập vào các file frontend theo các đường dẫn và kiểm tra chức năng hoạt động của Backend
    (các file này nằm trong folder views nhưng không cần thêm views vào đường dẫn)
    /get.html
    /update.html
    /list.html


Các thức hoạt động
#1 Khi khởi chạy, nếu là một file hợp lệ trong folder views thì frontend tương ứng sẽ được hiển thị.
#2 Nếu không, nó sẽ chuyển đến file index.js. Trong này, route(app) sẽ chuyển đến phần định tuyến trong folder routes.
#3 Trong /routes/index.js, với từng đường dẫn sẽ dẫn đến những bộ xử lý tương ứng, bao gồm:
+ student.js - khi đường dẫn có bắt đầu dưới dạng "/student/*". students.js sẽ đưa ra các hành động phù hợp với những đường dẫn và phương thức cụ thể.
+ fallBack.js - với các trường hợp khác.



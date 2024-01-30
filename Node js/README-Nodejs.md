1. ### Nodejs là gì?

   Nodejs là một nền tảng (Platform) phát triển độc lập được xây dựng ở trên Javascript Runtime của Chrome mà chúng ta có thể 
   xây dựng được các ứng dụng mạng một cách nhanh chóng và dễ dàng mở rộng. 

2. ### Lợi ích của việc sử dụng nodejs

   1. **Không đồng bộ và hướng sự kiện**: Tất cả API của Nodejs không đồng bộ và không bị chặn. Máy chủ dựa trên Nodejs không 
   đợi API trả về dữ liệu mà sẽ chuyển sang API tiếp theo sau khi gọi nó và cơ chế thông báo về sự kiện của Nodejs giúp máy 
   chủ nhận được phản hồi từ lệnh gọi API trước đó.
   2. **Rất nhanh**: Được xây dựng trên công cụ Javascript V8 của Google Chrome, nên thực thi code rất nhanh
   3. **Đơn luồng nhưng có khả năng mở rộng cao**: Nodejs sử dụng mô hình đơn luồng với vòng lặp sự kiện. Cơ chế sự kiện giúp 
   máy chủ không bị nghẽn và giúp máy chủ có khả năng mở rộng cao, trái ngược với máy chủ truyền thống tạo ra các luồng hạn chế
   xử lý request. Nodejs sử dụng 1 chương trình đơn luồng và có thể xử lý số lượng request lớn hơn nhiều so với máy chủ truyền
   thống như HTTP Apache.
   4. **Không buffering**: Xuất dữ liệu theo từng khối nên không đệm

3. ### Cài đặt global
   
   Các packages global được lưu trữ trong npm, để cài đặt thì sử dụng -g

4. ### Các tính năng của Nodejs

   1. IO điều khiển sự kiện không đồng bộ giúp xử lý yêu cầu đồng thời
   2. Thực thi code nhanh
   3. Đơn luồng nhưng có khả năng mở rộng cao
   4. No buffering

5. ### Control flow function

   Là một đoạn mã chung chạy giữa một số lệnh gọi hàm không đồng bộ 

6. ### Event Listeners là gì?

   Trình xử lý sự kiện là một hàm trong JavaScript, chờ sự kiện xảy ra và sau đó phản hồi sự kiện

7. ### Callback hell là gì?

   Hàm không đồng bộ yêu cầu hàm gọi lại làm tham số trả về. Khi nhiều hàm không đồng bộ được liên kết với nhau thì tình huống callback hell sẽ xảy ra.

8. ### Chạy quy trình bên ngoài bằng Node.js
 
   1. spawn - child_process.spawn khởi chạy một quy trình mới bằng một lệnh nhất định. 
   2. exec - phương thức child_process.exec chạy lệnh trong shell/console và đệm đầu ra.
   3. fork - Phương thức child_process.fork là trường hợp đặc biệt của spawn() để tạo các tiến trình con. 

9. ### Module của Node js 
   
   1. EventEmitter 
   2. Stream 
   3. FS 
   4. Net 
   5. Global Objects 

10. ### V8 là gì?

    Là một JavaScript engine, V8 được Google duy trì để sử dụng trong Chrome.

    V8 Chrome:
    1. V8 được viết bằng C++ và được sử dụng trong Chrome và Nodejs.
    2. Nó triển khai ECMAScript như được chỉ định trong ECMA-262.
    3. V8 có thể chạy độc lập, có thể nhúng nó vào chương trình C++ của riêng mình.

11. ### libuv là gì?

    là thư viện C được sử dụng để trừu tượng hóa các hoạt động I/O không chặn thành một giao diện nhất quán trên tất cả các nền tảng được hỗ trợ. 
    Nó cung cấp các cơ chế để xử lý hệ thống tệp, DNS, mạng, child processes, pipes, signal handling, polling and streaming

12. ### I/O?

    Là quá trình giao tiếp(Lấy dữ liệu vào, trả dữ liệu ra) giữa 1 hệ thống thông tin và môi trường bên ngoài
    ví dụ đọc ghi dữ liệu từ ổ cứng đều được coi là tác vụ I/O.

    1. Blocking I/O: Yêu cầu thực thi một IO operation, sau khi hoàn thành thì trả kết quả lại. Pocess/Theard gọi bị block cho đến 
    khi có kết quả trả về hoặc xảy ra ngoại lệ.
    2. Nonblocking I/O: Yêu cầu thực thi IO operation và trả về ngay lập tức (timeout = 0). Nếu operation chưa sẵn sàng để thực hiện
    thì thử lại sau. Tương đương với kiểm tra IO operatio có sẵn sàng ngay hay không, nếu có thì thực hiện và trả về, nếu không thì 
    thông báo thử lại sau.

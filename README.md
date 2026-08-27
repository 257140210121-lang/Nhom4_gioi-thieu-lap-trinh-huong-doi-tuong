# gioi-thieu-lap-trinh-huong-doi-tuong
# Nhom 4 gioi-thieu-lap-trinh-huong-doi-tuong
-Lập trình hướng đối tượng (Object-Oriented Programming - OOP) là một diễn trình lập trình (programming paradigm) dựa trên khái niệm "đối tượng" (object). Dữ liệu được đóng gói dưới dạng các thuộc tính (attributes / properties), và mã nguồn được đóng gói dưới dạng các phương thức (methods / procedures) gắn liền với đối tượng đó.
-Kiến trúc của OOP được cấu thành từ 6 yếu tố cơ bản:
-Lớp (Class): Kiểu dữ liệu mẫu do người dùng định nghĩa.
+ Đối tượng (Object): Thể hiện thực tế của Lớp trong bộ nhớ RAM.
+ Thuộc tính (Attributes / State): Các biến lưu trữ dữ liệu, trạng thái của đối tượng.
+ Phương thức (Methods / Behavior): Các hàm xử lý thực hiện hành vi của đối tượng.
+ Hàm khởi tạo & Hàm hủy (Constructor va Destructor): Các phương thức đặc biệt dùng để tạo lập và giải phóng vùng nhớ cho đối tượng.
+ 4 Nguyên lý vận hành: Đóng gói, Trừu tượng, Kế thừa và Đa hình.
-Lớp( Class):
Lớp là một kiểu dữ liệu do người dùng định nghĩa (User-defined Data Type), đóng vai trò là một mẫu dựng (blueprint) hoặc tập bản vẽ kỹ thuật xác định toàn bộ thuộc tính và phương thức mà mọi đối tượng thuộc lớp đó sẽ sở hữu
-Cấu trúc hoàn chỉnh của một Class:
+ Thuộc tính (Attributes / Properties / Fields): Các biến đại diện cho dữ liệu hoặc trạng thái của Class.
+ Phương thức (Methods / Functions): Các hàm định nghĩa tập hợp các hành vi, xử lý tác động lên dữ liệu của Class.
+ Phạm vi truy cập (Access Modifiers): Các từ khóa quy định quyền hạn truy cập vào thuộc tính và phương thức từ bên ngoài Class.
+ Phương thức đặc biệt (Constructor va Destructor):
*Constructor (Hàm khởi tạo): Tự động chạy khi một Object được tạo ra để gán giá trị ban đầu.
*Destructor (Hàm hủy): Tự động chạy khi Object bị dọn dẹp khỏi bộ nhớ RAM để giải phóng tài nguyên.
-Ba cấp độ truy cập (Access Modifiers) trong Class:
Cơ chế này giúp Class thực hiện Tính đóng gói (Encapsulation)
+ private: Chỉ cho phép các phương thức nội bộ bên trong Class đó truy cập; thường dùng để đóng gói và bảo vệ thuộc tính dữ liệu tránh bị truy cập hoặc sửa đổi tự do từ bên ngoài.
+ protected: Cho phép nội bộ Class đó và các Class con kế thừa từ nó truy cập; thường dùng khi muốn chia sẻ dữ liệu hoặc phương thức nội bộ cho các lớp trong cùng cây kế thừa.
+ public: Cho phép truy cập tự do từ bất kỳ đâu trong chương trình; thường dùng cho các phương thức hoặc giao tiếp mà Class cung cấp ra bên ngoài.
-Đối tượng( Object):
Đối tượng là một thể hiện (instance) cụ thể của một Lớp, được cấp phát không gian trong bộ nhớ (memory instantiation) tại thời điểm chương trình thực thi (runtime) để lưu trữ các giá trị dữ liệu thực tế.
-Mọi đối tượng trong OOP luôn được xác định bởi 3 yếu tố:
+Trạng thái (State / Attributes): Là tập hợp các dữ liệu hiện tại được lưu trữ trong các biến thuộc tính của đối tượng đó.
+ Hành vi (Behavior / Methods): Là tập hợp các phương thức (hàm) mà đối tượng có thể thực hiện để thao tác trên dữ liệu của chính nó hoặc tương tác với đối tượng khác.
+ Định danh (Identity): Là địa chỉ ô nhớ riêng biệt (memory address) do hệ điều hành cấp phát cho đối tượng, giúp phân biệt đối tượng này với đối tượng khác ngay cả khi chúng có cùng toàn bộ dữ liệu trạng thái.
-Một đối tượng trải qua 3 giai đoạn chính trên bộ nhớ RAM:
+ Khởi tạo (Instantiation & Initialization):
Toán tử new (hoặc khai báo biến) yêu cầu hệ thống cấp phát vùng nhớ RAM (thường nằm trên vùng Heap hoặc Stack tùy ngôn ngữ).
Hàm khởi tạo (Constructor) được tự động kích hoạt để gán các giá trị ban đầu cho các thuộc tính
+ Sử dụng (Usage):
Chương trình truy cập dữ liệu hoặc gửi thông điệp tới đối tượng thông qua lời gọi phương thức (ví dụ: doiTuong.phuongThuc()).
Trạng thái nội bộ của đối tượng có thể thay đổi liên tục trong quá trình vận hành.
+ Hủy bỏ (Destruction / Garbage Collection):
Khi đối tượng không còn được tham chiếu hoặc ra khỏi phạm vi truy cập (scope), nó sẽ bị thu hồi vùng nhớ.
Trong C++, Hàm hủy (Destructor) được gọi để giải phóng tài nguyên. Trong Java/C#, bộ thu gom rác (Garbage Collector) sẽ tự động dọn dẹp.
  

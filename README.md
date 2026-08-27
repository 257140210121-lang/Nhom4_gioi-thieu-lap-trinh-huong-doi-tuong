# Nhom 4 gioi-thieu-lap-trinh-huong-doi-tuong
sự kế thừa:
Kế thừa là cơ chế cho phép một lớp mới (gọi là lớp dẫn xuất / lớp con) tái sử dụng và mở rộng các đặc tính (thuộc tính) và hành vi (phương thức) từ một lớp đã có (gọi là lớp cơ sở / lớp cha).
Cho phép việc chỉ cần cài đặt phương thức ở một lớp cơ sở, mà có thể sử dụng được ở tất cả các lớp dẫn xuất.
Cho phép tránh sự cài đặt trùng lặp mã nguồn của chương trình.
Cho phép chỉ phải thay đổi một lần khi cần 2 phải thay đổi dữ liệu của các lớp.
lợi ích:
Tái sử dụng mã nguồn: Lớp con tự động có các tính năng của lớp cha mà không cần viết lại.
Tránh trùng lặp code: Gom các đặc điểm chung vào một nơi duy nhất.
Dễ dàng bảo trì: Khi cần sửa đổi logic chung, chỉ cần sửa ở lớp cha. Các lớp con sẽ tự động cập nhật theo.
Dễ dàng mở rộng: Thêm lớp con mới cực kỳ nhanh chóng dựa trên nền tảng lớp cha sẵn có.
Sự đóng gói:
Che giấu sự cài đặt chi tiết bên trong: Người sử dụng đối tượng chỉ cần biết phương thức đó làm gì, không cần biết nó được viết như thế nào.
Che giấu dữ liệu bên trong đối tượng: Ngăn chặn việc truy cập hoặc sửa đổi trực tiếp các thuộc tính (dữ liệu) của đối tượng từ bên ngoài.
Hạn chế tối đa việc sửa lại mã chương trình: Khi bạn cần thay đổi logic bên trong một lớp, bạn chỉ cần sửa mã nguồn của lớp đó. Tất cả các nơi khác đang gọi đối tượng này hoàn toàn không bị ảnh hưởng và không cần viết lại.
lợi ích:
Bảo mật và kiểm soát dữ liệu:Ngăn dữ liệu bị thay đổi tùy tiện từ bên ngoài.
Tăng tính tái sử dụng:Các lớp được đóng gói độc lập, dễ dàng mang sang dự án khác để sử dụng lại.
Tính đa hình (Polymorphism) cho phép các lớp được định nghĩa các phương thức trùng nhau, bao gồm:
• Cùng tên.
• Cùng số lượng và kiểu tham số.
• Cùng kiểu giá trị trả về.
Việc định nghĩa các phương thức trùng nhau giữa các lớp kế thừa nhau còn được gọi là sự nạp chồng phương thức.
Khi gọi các phương thức trùng tên, dựa vào đối tượng đang gọi, chương trình sẽ thực hiện phương thức của lớp tương ứng. Có thể hiểu đơn giản như sau:
• Một lớp cha định nghĩa một phương thức chung.
• Các lớp con kế thừa lớp cha có thể định nghĩa lại phương thức đó theo cách riêng.
• Khi gọi cùng một phương thức, kết quả thực hiện sẽ khác nhau tùy thuộc vào đối tượng thực tế.
Ví dụ minh họa
Giả sử có lớp cha Hình với phương thức:
• Tính diện tích()
Các lớp con có thể là:
• Hình chữ nhật → tính diện tích theo công thức dài × rộng.
• Hình tròn → tính diện tích theo công thức π × bán kính². Mặc dù đều gọi là Tính diện tích(), nhưng mỗi lớp con thực hiện phương thức theo cách khác nhau.
Ý nghĩa: Tính đa hình giúp chương trình có thể gọi cùng một phương thức nhưng thực hiện hành vi khác nhau tùy đối tượng.
Thành phần private
• là khu vực dành riêng cho lớp, không chia sẻ với bất kì lớp khác từ bên ngoài.
• Thành phần private chỉ cho phép truy nhập trong phạm vi nội bộ lớp.
• Thông thường các thành phần sau sẽ được đặt vào khu vực private của lớp:
 – Tất cả các thuộc tính dữ liệu của lớp
 – Các phương thức trung gian, được sử dụng như các bước tính toán đệm cho các phương thức khác. Thành phần public
• là khu vực mà Lớp có thể chia sẻ với tất cả các chương trình và đối tượng bên ngoài. Có thể truy nhập
 – Bên trong lớp
 – Bên ngoài lớp
• Các thành phần sẽ được đặt vào vùng chia sẻ public của lớp:
 – Các phương thức để nhập/xem (set/get) các thuộc tính dữ liệu của lớp.
 – Các phương thức cung cấp chức năng hoạt động, cách cư xử của đối tượng vớ
 i môi trường bên ngoài. Các phương thức này thể hiện chức năng của các đối tượng lớp.

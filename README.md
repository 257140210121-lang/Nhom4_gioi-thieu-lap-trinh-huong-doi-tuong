# Nhom 4 gioi-thieu-lap-trinh-huong-doi-tuong
1. Trừu tượng hóa đối tượng theo chức năng

Khái niệm:
Là cách trừu tượng hóa tập trung vào những chức năng mà đối tượng cung cấp, không quan tâm đến cách thực hiện bên trong.

Ví dụ:
Đối tượng ATM có các chức năng:

rutTien()
napTien()
kiemTraSoDu()

Người dùng chỉ cần biết ATM làm được gì, không cần biết hệ thống xử lý bên trong như thế nào.

2. Trừu tượng hóa đối tượng theo dữ liệu

Khái niệm:
Là cách trừu tượng hóa tập trung vào dữ liệu và các thuộc tính của đối tượng, đồng thời che giấu cách dữ liệu được lưu trữ và xử lý bên trong.

Ví dụ:
Đối tượng SinhVien có:

maSV
hoTen
diem

Người dùng có thể xem hoặc thay đổi điểm thông qua các phương thức như getDiem() và setDiem(), nhưng không cần biết dữ liệu được lưu trữ bên trong như thế nào.


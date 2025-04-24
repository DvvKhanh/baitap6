# baitap6
# Đậu Văn Khánh - K225480106099
Bài tập 6: Hệ quản trị CSDL
Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

DEADLINE: 23H59:59 NGÀY 25/4/2025

Ghi chú: Giải thích tại sao lại có SQL như vậy.

# BÀI LÀM
## 1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
+ Tạo Database sv_tnut
![image](https://github.com/user-attachments/assets/0ee0876d-8b3a-4648-9b67-8fffa359273d)

+ Vào File -> Chọn Open -> Chọn File rồi mở file sv_tnut.sql thầy gửi(đã download về)
![image](https://github.com/user-attachments/assets/c90240ae-8689-4388-aa6b-3a408b83ebf9)

+ Kết quả sau khi mở file sv_tnut.sql
![Screenshot 2025-04-24 164812](https://github.com/user-attachments/assets/5d769048-0e0c-4cc6-a38b-a714dd830623)

+ Nhấn execute để tạo bảng và cập nhật dữ liệu cho bảng
![image](https://github.com/user-attachments/assets/ace46210-ed54-4455-abc6-b711a7ffd24b)

+ Kết quả sau khi import thành công: hiển thị dữ liệu trong bảng SV
![image](https://github.com/user-attachments/assets/448a9769-e27c-49e9-9c82-938640c55206)

## 2. Dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
+ Dữ liệu đầu vào
![image](https://github.com/user-attachments/assets/2f4d7cea-928d-4485-b0b9-17995451c694)
+ Tuy nhiên,dữ liệu đầu vào của sinh viên đã có sẵn trong cơ sở dữ liệu được import từ file sv_tnut.sql. Do đó, không thể insert vào bảng SV bởi vì thuộc tính masv là khóa chính (PK) trong bảng SV, nên mỗi sinh viên sẽ chỉ có một mã số duy nhất.
+ Để truy xuất chính xác thông tin của sinh viên đang thực hiện bài tập, cách tốt nhất là dựa vào mã số sinh viên (masv), thay vì chỉ dùng họ tên hay ngày sinh vì có thể sẽ bị trùng lặp giữa nhiều sinh viên. Việc truy vấn theo masv sẽ đảm bảo độ chính xác tuyệt đối và tránh được mọi trường hợp nhầm lẫn.
+ Kết quả sau khi truy vấn
![image](https://github.com/user-attachments/assets/1fe20c87-194e-43ea-aa22-f85ffa03bec7)

## 3. Nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
![image](https://github.com/user-attachments/assets/2c95ac46-ecf6-4525-9570-2ac15cff6e50)

## 4. Nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
![Screenshot 2025-04-24 172459](https://github.com/user-attachments/assets/22258090-3271-428b-8d8c-4b6dc650f124)

## 5. Nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
![image](https://github.com/user-attachments/assets/aa53826c-c505-44d0-9935-b98f1bf6607f)

## 6. Nhập sql để tìm xem có những sv nào trùng tên với em?
![image](https://github.com/user-attachments/assets/0aaa9ced-03db-4f01-b84e-01f761eb5210)

## 7. Nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
![image](https://github.com/user-attachments/assets/a3c0e015-7b2d-4b6f-b3c9-1e6daf84c66b)

## 8. Nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.

# F Gỡ lỗi:<br>

Bước 1: Nếu có lỗi xẩy ra trong quá trình triển khai docker compose up -d<br>
 -Sửa lỗi kết nối mạng (DNS Fix)<br>
Thêm dòng nameserver 8.8.8.8<br>
<img width="613" height="238" alt="image" src="https://github.com/user-attachments/assets/9c74335b-8419-4226-8d95-6d72632b2c69" /><br>
Kết quả:<br>
<img width="945" height="113" alt="image" src="https://github.com/user-attachments/assets/6179c6d3-a0cc-4191-94fe-ed6d0a6c0a31" /><br>
Bước 2: Thêm healthcheck cho myapi trong file docker-compose.yml<br>
-Thêm thuộc tính healthcheck cho dịch vụ myapi để kiểm tra phản hồi tại cổng 9630.<br>
<img width="945" height="76" alt="image" src="https://github.com/user-attachments/assets/350311fb-b0ce-445d-ab60-515b2674c6f5" /><br>
Bước 3: giới hạn resource cho một service: (tránh việc 1 service chiếm quá nhiều ram)<br>
<img width="519" height="169" alt="image" src="https://github.com/user-attachments/assets/a130e407-1119-47c3-8bc9-10388b311338" /><br>
-sử dụng lệnh: docker compose stats để quan sát lượng ram sử dụng bởi mỗi service<br>
<img width="945" height="106" alt="image" src="https://github.com/user-attachments/assets/10b282f9-3009-478a-a73e-fd551ab1fb84" /><br>


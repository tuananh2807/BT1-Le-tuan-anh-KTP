# E. Triển khai (level test) ứng dụng<br>

# Bước 1+2+3:<br>

-Chuyển vào trong thư mục ~/myapp<br>
-Gõ lệnh để docker compose chạy: sẽ run tất cả các service khai báo trong file docker-compose.yml<br>
-Kiểm tra các container đang chạy trong docker, nếu có cái nào bị restart cần tìm lỗi rồi edit lại docker-compose.yml<br>
<img width="945" height="237" alt="image" src="https://github.com/user-attachments/assets/096f6fc0-9fa1-453e-bfd8-229225e9e732" /><br>

# Bước 4: Kiểm tra kiểm thử các service đang chạy độc lập thông qua ip và port của nó: ví dụ mở trình duyệt ip_ubuntu:1880 để check nodered đã chạy chưa<br>

ảnh 1<br>

<img width="945" height="62" alt="image" src="https://github.com/user-attachments/assets/f605db0c-49ee-4eba-b551-eacfd24a3a75" /><br>

ảnh 2<br>

<img width="945" height="445" alt="image" src="https://github.com/user-attachments/assets/25c71da1-7f6c-45d1-b013-e6621c585e3a" /><br>

# Bước 5: Sử dụng nodered: kéo nodered http_in , http_response, function : để tạo api get đơn giản (dùng cho /api proxy_pass của nginx)<br>
<img width="945" height="445" alt="image" src="https://github.com/user-attachments/assets/64a8a293-cade-4eb6-8292-ce7a0506f86a" /><br>

# Bước 6: Sửa file ./myweb/index.html : thêm code html+js để sử dụng được api đã khai báo proxy_pass (thực ra là sử dụng nodered http_in hoặc sử dụng service myapi)<br>
<img width="945" height="414" alt="image" src="https://github.com/user-attachments/assets/fd4834cd-e930-4d01-bff3-ddc9d618b187" /><br>






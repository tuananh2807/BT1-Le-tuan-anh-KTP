# C Cấu hình docker compose:<br>

Bước 1+2+3:<br>
-Tạo thư mục: ~/myapp<br>
-Chuyển vào trong thư mục ~/myapp<br>
-Tạo thư mục: ./myweb<br>
<img width="945" height="168" alt="image" src="https://github.com/user-attachments/assets/23fef44e-f8a3-44d5-8657-e24ed0df7ac6" /><br>
Bước 4: Tạo file ./myweb/index.html (với nội dung là thông tin cá nhân của em)<br>
<img width="945" height="800" alt="image" src="https://github.com/user-attachments/assets/8bd94180-a6fa-4a17-af7c-e485852e2d86" /><br>
Bước 5: Tạo file docker-compose.yml để nó sẽ có các dịch vụ sau:<br>
-Khai báo sử dụng nodered/node-red, cổng 1880, dữ liệu nằm tại thư mục ./nodered<br>
-Khai báo sử dụng nginx, cổng 80, cấu hình trong file ./nginx/nginx.conf<br>
-Mount thư mục ./myweb thành thư mục /myweb trong nginx<br>
-Mount file ./nginx/nginx.conf vào file /etc/nginx/nginx.conf trong nginx<br>
<img width="945" height="628" alt="image" src="https://github.com/user-attachments/assets/023d5ef6-69bd-4a22-836c-2acd6ab23bd3" /><br>
Bước 6: Edit file ./nginx/nginx.conf để:<br>
-Cấu hình web server cổng 80<br>
-server_name là sub-domain (sub-domain tuỳ ý của em)<br>
-location / trỏ tới root là thư mục /myweb<br>
-location /api dùng proxy_pass trỏ tới 1 (hoặc nhiều) node http_in của nodered<br>
<img width="945" height="646" alt="image" src="https://github.com/user-attachments/assets/67ef18da-d7cd-4691-b42a-cd2c3ab6a849" /><br>
Bước 7: Edit file ./nodered/settings.js để nodered bắt buộc đăng nhập<br>
-Chạy hệ thống lần đầu (để sinh file)<br>
<img width="989" height="94" alt="image" src="https://github.com/user-attachments/assets/d7c9aa6c-40c5-4864-a36c-b6250a99fb59" /><br>
-file settings.js đã xuất hiện<br>
<img width="945" height="86" alt="image" src="https://github.com/user-attachments/assets/43cee22e-1441-4bd9-9e1b-8e67187a32d9" /><br>
-Trang web cá nhân<br>
<img width="945" height="347" alt="image" src="https://github.com/user-attachments/assets/2e8bd72a-0493-425d-84a8-f6c024e5deca" /><br>
-Node-red bắt buộc đăng nhập<br>
<img width="945" height="547" alt="image" src="https://github.com/user-attachments/assets/1400513a-5dad-4080-9598-96036506ceda" /><br>








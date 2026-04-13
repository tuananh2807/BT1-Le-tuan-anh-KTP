# D (Bonus - không bắt buộc)<br>

# Bước 1:Tạo thư mục cho API<br>
-Đảm bảo đang ở trong thư mục myapp<br>

# Bước 2: Viết code Python cho API<br>
<img width="945" height="544" alt="image" src="https://github.com/user-attachments/assets/4a285026-5879-46ef-b158-c7219f6528b1" /><br>

# Bước 3: tạo file ./myapi/requirements.txt chứa các thư viện mà app.py sử dụng (theo như app.py ví dụ thì requirements.txt chỉ cần có nội dung: flask)<br>
<img width="945" height="98" alt="image" src="https://github.com/user-attachments/assets/00c4b615-5840-458d-8aa8-8cf50b390883" /><br>

# Bước 4: tạo file ./myapi/Dockerfile để khai báo sử dụng Python 3.9 slim<br>
<img width="945" height="277" alt="image" src="https://github.com/user-attachments/assets/890350e4-d501-4447-a72b-4aa30c80d783" /><br>

# Bước 5: Sửa đổi docker-compose để sử dụng myapp<br>
<img width="945" height="351" alt="image" src="https://github.com/user-attachments/assets/c88d0b77-076a-485b-b055-b83bde5c2ffe" /><br>

# Bước6: Sửa đổi nginx/nginx.conf để /api trỏ tới service myapp cổng 9630<br>
<img width="945" height="100" alt="image" src="https://github.com/user-attachments/assets/1aaf1971-508d-4533-b482-aa8e0c148387" /><br>





# G. Triển khai ứng dụng đến End-user<br>

-Tạo Tunnel và lấy Token<br>
Em đã cài đặt cloudflared trên Windows, thực hiện đăng nhập và xác thực thành công tên miền letuananh123pl.id.vn.<br>
Em đã lấy được mã Tunnel ID/Token: 00d1e170-45d9-4969-9fdd-34814984adf5. Đây là chìa khóa để "thông" mạng ra ngoài Internet.<br>
<img width="791" height="74" alt="image" src="https://github.com/user-attachments/assets/77fa639a-6da8-4698-89d0-58740371ef88" /><br>
-Convert lệnh sang Docker Compose<br>
Em đã chuyển đổi thành công từ lệnh chạy đơn lẻ của Cloudflare sang cấu trúc tệp YAML chuyên nghiệp.<br>
Việc này giúp hệ thống của em chạy đồng bộ (Web, Database, Tunnel) chỉ với một lệnh duy nhất.<br>
do máy ảo bị lỗi nên em không thể kết nối mạng, em không thể hoàn thiện phần G này. em sẽ khắc phục sớm ạ<br>

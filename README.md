🛍️ 22688861 – Lê Thái Hòa – EProject
🧾 Giới thiệu

Thực hiện bởi: Lê Thái Hòa – MSSV: 22688861
Mô tả: Đây là một hệ thống thương mại điện tử được phát triển dựa trên mô hình kiến trúc Microservices.
Mục tiêu của dự án là mô phỏng quy trình hoạt động của một hệ thống bán hàng trực tuyến có khả năng mở rộng linh hoạt, dễ bảo trì và triển khai thông qua Docker.

💻 Công nghệ & Công cụ sử dụng
Node.js & Express.js: Nền tảng xây dựng backend cho từng microservice.
MongoDB: Cơ sở dữ liệu chính của hệ thống.
RabbitMQ: Hỗ trợ truyền thông giữa các dịch vụ (message broker).
Docker & Docker Compose: Đóng gói và triển khai toàn bộ hệ thống dễ dàng.
Nginx / HTTP Proxy: Đóng vai trò là cổng giao tiếp trung gian (API Gateway).
JWT & API Key: Dùng cho xác thực và phân quyền người dùng.
⚙️ Thành phần chính của hệ thống
🧩 API Gateway
Là điểm truy cập duy nhất của client.
Chịu trách nhiệm định tuyến request đến các dịch vụ tương ứng.
🔐 Auth Service
Cung cấp chức năng đăng ký, đăng nhập và quản lý xác thực người dùng bằng JWT.
📦 Product Service
Xử lý các nghiệp vụ liên quan đến sản phẩm như:
Tạo mới
Chỉnh sửa
Hiển thị danh sách sản phẩm
🧾 Order Service
Quản lý đơn hàng của khách hàng.
Kết nối với các dịch vụ khác để đảm bảo luồng xử lý đơn được đồng bộ.
🗄️ MongoDB
Hệ quản trị cơ sở dữ liệu NoSQL.
Lưu trữ thông tin sản phẩm, người dùng và đơn hàng.
📨 RabbitMQ
Hệ thống message broker giúp các microservice giao tiếp bất đồng bộ.
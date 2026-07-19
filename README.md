# job-recruitment-system
Website kết nối nhà tuyển dụng và ứng viên sử dụng ReactJS và Spring Boot
Hệ thống cung cấp:

- Giao diện web thân thiện cho ứng viên và nhà tuyển dụng.
- Hệ thống xác thực và phân quyền bằng Spring Security + JWT.
- Quản lý tin tuyển dụng, hồ sơ ứng viên và quá trình ứng tuyển.
- API REST kết nối giữa ReactJS và Spring Boot.
- Cơ sở dữ liệu MySQL lưu trữ toàn bộ thông tin hệ thống.

---

# Chức năng hiện tại

### Trang chủ

- Hiển thị thông tin giới thiệu hệ thống.
- Danh sách việc làm nổi bật.
- Danh sách doanh nghiệp tuyển dụng.

### Ứng viên

- Đăng ký tài khoản.
- Đăng nhập / Đăng xuất.
- Quản lý hồ sơ cá nhân.
- Tìm kiếm việc làm.
- Ứng tuyển trực tuyến.
- Theo dõi trạng thái hồ sơ.
- Lưu việc làm yêu thích.

### Nhà tuyển dụng

- Quản lý thông tin doanh nghiệp.
- Đăng tin tuyển dụng.
- Chỉnh sửa hoặc xóa tin tuyển dụng.
- Xem danh sách ứng viên.
- Duyệt hoặc từ chối hồ sơ ứng tuyển.

### Quản trị viên

- Quản lý người dùng.
- Quản lý doanh nghiệp.
- Quản lý danh mục.
- Quản lý tin tuyển dụng.
- Thống kê dữ liệu hệ thống.

---

# Yêu cầu môi trường

- Java 21+
- Node.js 20+
- Maven
- MySQL 8+
- Git

---

# Hướng dẫn cài đặt

Clone dự án

```bash
git clone https://github.com/<username>/job-recruitment-system.git
```

Khởi động Backend

```bash
cd backend
./mvnw spring-boot:run
```

Khởi động Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend:

```
http://localhost:5173
```

Backend:

```
http://localhost:8080
```

---

# Cơ sở dữ liệu

Tạo database

```sql
CREATE DATABASE job_portal;
```

Cấu hình `application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/job_portal
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
```

Hệ thống sẽ tự động tạo bảng khi khởi động.

---

# Kiến trúc hệ thống

| Thành phần | Công nghệ | Vai trò |
|------------|-----------|----------|
| Frontend | ReactJS | Giao diện người dùng |
| Backend | Spring Boot | Xử lý nghiệp vụ và cung cấp REST API |
| Xác thực | Spring Security + JWT | Đăng nhập và phân quyền |
| Cơ sở dữ liệu | MySQL | Lưu trữ dữ liệu |
| ORM | Spring Data JPA | Thao tác với cơ sở dữ liệu |

---

# Cấu trúc dự án

```
job-recruitment-system/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── controller/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── entity/
│   │   ├── dto/
│   │   ├── config/
│   │   └── security/
│   ├── pom.xml
│   └── application.properties
│
└── README.md
```

---

# Cách sử dụng

Chạy Backend

```bash
cd backend
./mvnw spring-boot:run
```

Chạy Frontend

```bash
cd frontend
npm run dev
```

Sau đó truy cập:

```
http://localhost:5173
```

---

# Công nghệ sử dụng

### Frontend

- ReactJS
- React Router
- Axios
- HTML5
- CSS3
- Bootstrap / Material UI

### Backend

- Spring Boot
- Spring Security
- Spring Data JPA
- JWT

### Database

- MySQL

### Công cụ phát triển

- Git
- GitHub
- Visual Studio Code
- Postman

---

# Định hướng phát triển

- Xác thực email.
- Quên mật khẩu.
- Gợi ý việc làm phù hợp.
- Phân tích CV.
- Thông báo thời gian thực.
- Đặt lịch phỏng vấn.
- Hệ thống chat giữa ứng viên và nhà tuyển dụng.
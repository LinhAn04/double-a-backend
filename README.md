# Double A Restaurant - Backend

Dự án Spring Boot REST API cho hệ thống quản lý nhà hàng.

---

## Công nghệ sử dụng

### Môi trường cài đặt

| Công nghệ | Loại | Mục đích |
|-----------|------|---------|
| Java 21 | Ngôn ngữ lập trình | Ngôn ngữ và môi trường chạy ứng dụng backend |
| Spring Boot 3 | Framework backend | Framework giúp xây dựng ứng dụng web/API Java nhanh, cấu hình tự động |
| Maven Wrapper | Công cụ build | Dùng để build project và quản lý thư viện |
| MySQL | Database | Hệ quản trị cơ sở dữ liệu quan hệ lưu trữ dữ liệu |

### Thư viện hỗ trợ backend

| Thư viện | Mục đích |
|---------|---------|
| Lombok | Tự động tạo getter, setter, constructor giúp code Java ngắn gọn |
| Spring Data JPA | Giúp thao tác database bằng Java object |
| Spring Security + JWT | Xác thực và phân quyền người dùng bằng token JWT |
| Hibernate Validator | Kiểm tra dữ liệu đầu vào |
| JJWT | Thư viện tạo và kiểm tra JSON Web Token |
| Spring Mail | Dùng để gửi email từ ứng dụng |

---

## Hướng dẫn cài đặt

### 1. Clone source

Clone source code từ repository: https://github.com/LinhAn04/double-a-backend.git

---

### 2. Thay đổi cấu hình

Chỉnh sửa các tài khoản và key trong file:

```
application-dev.properties
```

Cấu hình bao gồm:

**MySQL database**

```
username
password
```

**Spring Mail**

```
spring.mail.username
spring.mail.password
```

**Cloudinary**

```
cloudinary.cloud-name
cloudinary.api-key
cloudinary.api-secret
```

**Google OAuth2**

```
client-id
client-secret
```

---

### 3. Tạo database

Đảm bảo trong MySQL có database:

```
double_a_db
```

---

### 4. Chạy ứng dụng

Chạy file:

```
DoubleARestaurantApplication
```

---

## Cấu trúc thư mục dự án

```
src/
├── main/
│   ├── java/com/BE
│   │   ├── config/
│   │   ├── controller/
│   │   ├── dto/
│   │   ├── enums/
│   │   ├── exception/
│   │   ├── mapper/
│   │   ├── model/
│   │   ├── service/
│   │   ├── repository/
│   │   ├── security/
│   │   ├── service/
│   │   ├── util/
│   │   └── Application
│   └── resources/
│       ├── application.properties
│       └── application-dev.properties
└── test/

    └── ...
```

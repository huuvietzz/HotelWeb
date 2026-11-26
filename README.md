# Hotel Booking – Hệ thống đặt phòng khách sạn

Website đặt phòng khách sạn trực tuyến, gồm 2 phần:

- **Trang khách hàng:** xem phòng, đặt phòng, thanh toán, xem lịch sử đặt phòng.
- **Trang quản trị:** quản lý phòng, đặt phòng, tài chính, khách hàng, nhân viên và thống kê.

---

## Công nghệ sử dụng

- **Backend:** Java 17, Spring Boot
- **Database / Cache:** MySQL, Redis
- **Frontend:** HTML, CSS, JavaScript, Bootstrap 5
- **Công cụ:** Maven, Docker

---

## Chức năng

### Khách hàng

- Xem thông tin phòng
- Đặt phòng
- Thanh toán đặt phòng
- Xem lịch sử đặt phòng

### Quản trị

#### ADMIN

- Quản lý phòng
- Quản lý loại phòng
- Quản lý đặt phòng
- Quản lý tài chính
- Quản lý tiện ích
- Báo cáo & Thống kê
- Quản lý khách hàng
- Quản lý nhân viên

#### Nhân viên

- Quản lý phòng
- Quản lý loại phòng
- Quản lý đặt phòng
- Quản lý tài chính
- Quản lý tiện ích
- Báo cáo & Thống kê
- Quản lý khách hàng

---

## Cài đặt và chạy

### Yêu cầu

- JDK 17
- Maven 3.9+
- MySQL 8.0
- Docker (để chạy Redis)

### Các bước

**1. Clone dự án**

```bash
git clone https://github.com/huuvietzz/HotelWeb.git
```

**2. Tạo database**

```sql
CREATE DATABASE hotel_booking;
```

**3. Chạy Redis bằng Docker**

```bash
docker run -d --name redis -p 6379:6379 redis:latest
```

**4. Chạy ứng dụng**

Cấu hình kết nối MySQL trong `application.properties`, sau đó chạy class `main` trong IntelliJ hoặc:

```bash
mvn spring-boot:run
```

Truy cập: `http://localhost:8080`

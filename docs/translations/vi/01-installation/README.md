# cài đặt

Cách sao chép kho mã nguồn, cài đặt các phụ thuộc và chạy Vinyl trên máy cục bộ.

> [!NOTE]
> Hỗ trợ Docker hiện đang được phát triển. Tạm thời, vui lòng làm theo hướng dẫn thiết lập cục bộ bên dưới.

### Yêu cầu trước khi cài đặt

Trước khi bắt đầu, hãy đảm bảo bạn đã cài đặt các công cụ sau:

- **Node.js** (phiên bản 20 trở lên)
- **Git**
- **npm** (hoặc trình quản lý gói ưa thích của bạn: `pnpm`, `yarn`, `bun`)

---

### 1. Sao chép kho lưu trữ (Clone)

```bash
git clone https://github.com/araujoio/vinyl.git
cd vinyl
```

### 2. Cài đặt các gói phụ thuộc

Chạy lệnh sau tại thư mục gốc của dự án:

```bash
npm install
```

### 3. Khởi động máy chủ phát triển

```bash
npm run dev
```

Sau khi khởi động, hãy mở [http://localhost:3000](http://localhost:3000) trên trình duyệt của bạn để trải nghiệm Vinyl.

<br />

<div align="left">
  <a href="../00-quickstart/README.md"><strong>← Trước: Bắt Đầu Nhanh</strong></a>
</div>
<div align="right">
  <a href="../02-configuration/README.md"><strong>Tiếp theo: Cấu hình →</strong></a>
</div>

---

*Tuyên bố từ chối trách nhiệm: Tài liệu này được dịch bằng quy trình tự động hóa AI nội bộ và có thể chứa lỗi hoặc điểm không chính xác. Tài liệu gốc bằng tiếng Anh là nguồn tham khảo chính thức.*

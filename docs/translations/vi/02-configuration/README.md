# cấu hình

Cách thiết lập các biến môi trường và tích hợp dịch vụ cho Vinyl.

### Cài đặt môi trường

Tạo tệp `.env` tại thư mục gốc và thêm biến sau:

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### Nhận khóa API YouTube

1. Truy cập [Google Cloud Console](https://console.cloud.google.com/) và vào mục **APIs & Services**.

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. Ở thanh điều hướng bên trái, nhấp vào **Library** (Thư viện).

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. Tìm kiếm **YouTube Data API v3**, chọn từ danh mục và nhấn **Enable** (Bật).

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. Sau khi kích hoạt, chuyển sang mục **Credentials** ở thanh bên trái, nhấn **+ Create Credentials** và chọn **API Key**.

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. Trong bảng điều khiển **Create API key**, cấu hình các tùy chọn và nhấn **Create**:
   - **Name:** Nhập tên dễ nhận biết (ví dụ: `vinyl-key`).
   - **API restrictions:** Chọn **YouTube Data API v3**.
   - **Application restrictions:** Giữ nguyên là **None**.

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. Sao chép khóa API vừa tạo và đặt vào tệp `.env` của bạn dưới dạng `YOUTUBE_API_KEY`:

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud cung cấp hạn mức miễn phí hàng ngày cho YouTube Data API, hoàn toàn đủ cho nhu cầu phát triển cục bộ và sử dụng cá nhân.

<div align="left">
  <a href="../01-installation/README.md"><strong>← Trước: Cài đặt</strong></a>
</div>

---

*Tuyên bố từ chối trách nhiệm: Tài liệu này được dịch bằng quy trình tự động hóa AI nội bộ và có thể chứa lỗi hoặc điểm không chính xác. Tài liệu gốc bằng tiếng Anh là nguồn tham khảo chính thức.*

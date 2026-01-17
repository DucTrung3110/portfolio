# Hướng Dẫn Sử Dụng Portfolio Website

Portfolio của bạn đã được thiết kế với giao diện hiện đại, hiệu ứng đẹp mắt và hỗ trợ cả máy tính lẫn điện thoại. Dưới đây là hướng dẫn để bạn tùy chỉnh và đưa website lên mạng.

## Cấu Trúc Thư Mục
```
portfolio-website/
├── index.html          # File chính chứa nội dung (Tiếng Việt)
├── css/
│   └── style.css      # File giao diện (màu sắc, bố cục)
├── js/
│   └── main.js        # File xử lý hiệu ứng, tương tác
└── README.md          # Hướng dẫn này
```

## 1. Tùy Chỉnh Nội Dung

Bạn cần mở file `index.html` bằng một trình soạn thảo code (như VS Code, Notepad) và thay đổi các thông tin sau:

- **Tên của bạn**: Tìm `[Tên Của Bạn]` và thay bằng tên thật.
- **Role/Vị trí**: Tìm `Software Engineer` thay bằng vị trí mong muốn của bạn.
- **Mạng xã hội**: Thay các link `#` trong phần `href="#"` bằng link GitHub, LinkedIn, Facebook thật của bạn.
- **Projects/Thành tích**: Thay đổi nội dung mô tả dự án và thành tích thật của bạn.
- **Email**: Thay `email@example.com` bằng email thật.

## 2. Thay Đổi Hình Ảnh

Để thay ảnh đại diện:
1. Tạo thư mục `assets/images` (nếu chưa có).
2. Đặt ảnh của bạn vào thư mục đó (ví dụ: `profile.jpg`).
3. Trong file `index.html`, tìm đoạn:
   ```html
   <div class="profile-image-container">
       <!-- Placeholder image, will be replaced -->
       <div class="profile-placeholder">
   ```
4. Thay thế thẻ `div.profile-placeholder` bằng thẻ `img`:
   ```html
   <div class="profile-image-container">
       <img src="assets/images/profile.jpg" alt="Tên của bạn" style="width:100%; height:100%; object-fit:cover; border-radius:50%;">
   </div>
   ```

## 3. Cách Deploy (Đưa lên mạng) miễn phí

Cách đơn giản nhất là dùng **GitHub Pages**:

1. Đăng nhập vào GitHub và tạo một **Repository** mới (ví dụ: `my-portfolio`).
2. Upload tất cả các file trong thư mục này lên Repository đó.
3. Vào phần **Settings** của Repository -> chọn mục **Pages** (ở menu bên trái).
4. Ở phần **Source**, chọn nhánh `main` (hoặc `master`) và folder `/ (root)`. Nhấn **Save**.
5. Đợi khoảng 1-2 phút, GitHub sẽ cung cấp cho bạn một đường link (dạng `https://username.github.io/my-portfolio`).

## 4. Tạo QR Code cho CV

Khi đã có đường link website (ví dụ: `https://username.github.io/my-portfolio`), bạn làm như sau:

1. Truy cập trang tạo QR miễn phí như: `qr-code-generator.com` hoặc `goqr.me`.
2. Dán đường link website của bạn vào.
3. Tải file hình ảnh QR Code về (định dạng PNG hoặc SVG).
4. Chèn hình ảnh QR Code đó vào CV của bạn với chú thích "Quét để xem Portfolio".

## Tính Năng Nổi Bật
- **Giao diện Glassmorphism**: Hiệu ứng kính mờ thời thượng.
- **Dark/Light Mode**: Chuyển đổi chế độ sáng/tối.
- **Responsive**: Hiển thị đẹp trên mọi thiết bị (Mobile/Tablet/PC).
- **Smooth Animations**: Hiệu ứng chuyển động mượt mà.

Chúc bạn có một chiếc portfolio ấn tượng và thành công trong công việc!

# Auto Translate On Selection (VI ⇄ EN)

Một Userscript siêu nhẹ, tối ưu hiệu năng giúp tự động dịch thuật hai chiều **Anh ⇄ Việt** ngay khi bạn bôi đen văn bản trên bất kỳ trang web nào.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-Tampermonkey%20%7C%20Violentmonkey-green.svg)

## 🌟 Tính năng nổi bật

- **Dịch tự động 2 chiều (VI ⇄ EN):** Tự động nhận diện tiếng Việt (qua dấu câu) để chuyển sang tiếng Anh và ngược lại mà không tốn request detect ngôn ngữ.
- **Tốc độ cực nhanh & Tiết kiệm tài nguyên:**
  - **Debounce 80ms:** Tránh spam API khi đang kéo thả chọn văn bản.
  - **In-memory Cache:** Lưu tạm các đoạn đã dịch, bôi lại không cần tốn request gọi lại API.
  - **Single Request:** Chỉ gửi đúng 1 request cho mỗi lần bôi đen.
- **Bản vệ CSP (Content Security Policy):** Áp dụng CSS trực tiếp qua JavaScript DOM Style, chạy mượt mà trên cả các trang có chính sách bảo mật khắt khe như PDF.js Viewer.
- **Cơ chế Fallback thông minh:** Ưu tiên dùng `fetch()` để đạt tốc độ cao nhất, tự động chuyển sang `GM_xmlhttpRequest` nếu bị trang web chặn Cross-Domain.
- **Giao diện Dark Mode:** Nhỏ gọn, tối giản, đẹp mắt và tự động đóng khi nhấn `ESC` hoặc click ra ngoài.

## 🚀 Hướng dẫn cài đặt

1. Cài đặt tiện ích mở rộng quản lý script trên trình duyệt của bạn:
   - [Tampermonkey](https://www.tampermonkey.net/) (Khuyên dùng) hoặc [Violentmonkey](https://violentmonkey.github.io/).
2. Nhấp vào nút tạo Script mới (`Create a new script`).
3. Dán toàn bộ nội dung file `auto-translate.user.js` vào trình chỉnh sửa và nhấn `Ctrl + S` (hoặc `Cmd + S`) để lưu.

## 💡 Cách sử dụng

1. Truy cập bất kỳ trang web nào.
2. Dùng chuột bôi đen đoạn văn bản cần dịch.
3. Bảng dịch sẽ tự động hiển thị ngay bên dưới đoạn văn bản được chọn.

## 📜 License

Dự án được phân phối dưới giấy phép [MIT License](LICENSE).

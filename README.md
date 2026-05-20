# Stealth LMS - Tab Visibility Bypass

Một đoạn script nhỏ gọn giúp vô hiệu hóa các cơ chế theo dõi trạng thái tab (Tab Tracking) trên trình duyệt. Script này ngăn chặn trang web phát hiện khi người dùng chuyển sang tab khác, thu nhỏ cửa sổ hoặc click ra ngoài phạm vi trang web.

##  Tính năng cốt lõi

* **Block Visibility Change:** Ghi đè sự kiện `visibilitychange` của Document, buộc trang web luôn hiểu rằng nó đang hiển thị (`document.visibilityState === 'visible'`).
* **Anti-Blur:** Vô hiệu hóa các event `blur` và `mouseleave` trên `window` và `document`.
* **Focus Lock:** Giả lập trạng thái luôn luôn `focus` cho cửa sổ trình duyệt.

## Hướng dẫn sử dụng (Console Injection)

Cách nhanh nhất để chạy script này là thông qua DevTools của trình duyệt:

1. Truy cập vào trang web/hệ thống mục tiêu.
2. Mở **Developer Tools** (Nhấn `F12` hoặc `Ctrl + Shift + I` / `Cmd + Option + I`).
3. Chuyển sang tab **Console**.
4. Mở file `auto.txt` trong repository này, copy toàn bộ nội dung code.
5. Dán code vào Console và nhấn `Enter` để thực thi.
6. Hoàn tất! Từ lúc này bạn có thể thoải mái chuyển tab mà trang web không thể nhận diện được.

## Lưu ý (Disclaimer)

Việc sử dụng tool này trong các môi trường thi cử thực tế là một sự **đánh đổi** giữa sự tiện lợi khi tra cứu tài liệu và rủi ro vi phạm quy chế của hệ thống. 

Dự án chỉ mang tính chất nghiên cứu an toàn thông tin, Proof of Concept (PoC) về Web Exploitation và cơ chế hoạt động của DOM Events. Người dùng tự chịu trách nhiệm về mọi rủi ro khi sử dụng.

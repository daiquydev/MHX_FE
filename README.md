Hướng dẫn Build và Chạy Dự Án MXH_FE
1. Cài đặt các phần mềm yêu cầu
Node.js: Cài đặt phiên bản Node.js (khuyến nghị dùng phiên bản LTS  16).

Kiểm tra cài đặt Node.js:
node -v
Nếu chưa cài, tải và cài đặt từ Node.js official website.
Yarn: Đảm bảo bạn đã cài Yarn (trình quản lý gói thay thế npm).

Kiểm tra phiên bản Yarn:
yarn -v
Nếu chưa cài, cài đặt Yarn bằng lệnh sau:

npm install -g yarn
2. Clone dự án
Tải mã nguồn về máy:

git clone <repository-url>
Di chuyển vào thư mục dự án:

cd MXH_FE
3. Cài đặt dependencies
Chạy lệnh sau để cài đặt tất cả dependencies cần thiết:

yarn install
Lưu ý: Nếu gặp cảnh báo về package-lock.json, bạn có thể xóa file package-lock.json để tránh xung đột với Yarn.

4. Chạy dự án trong môi trường phát triển
Khởi động ứng dụng React bằng lệnh:


yarn start
Dự án sẽ chạy tại http://localhost:3000.
Ghi chú: Nếu gặp lỗi ERR_OSSL_EVP_UNSUPPORTED, thêm biến môi trường như sau:

set NODE_OPTIONS=--openssl-legacy-provider && yarn start

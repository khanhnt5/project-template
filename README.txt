KHUNG CHIA FILE DÙNG CHUNG CHO DỰ ÁN

Đây là bộ khung tổ chức thư mục, rút từ cách chia tính năng của
app-legendverse và khái quát để dùng cho Android, web, desktop hoặc backend.
Đây chưa phải ứng dụng chạy được; chọn công nghệ rồi thêm file mã nguồn,
cấu hình build và thư viện tương ứng. Các file .gitkeep giữ thư mục trống.

CÁCH DÙNG
1. Copy cả folder project-template, đổi tên thành tên dự án mới.
2. Đọc STRUCTURE.txt để biết mỗi loại file đặt ở đâu.
3. Đọc docs/architecture/CODE-FLOW.txt để hiểu hướng phụ thuộc và luồng chạy.
4. Đổi features/example thành tính năng đầu tiên của dự án.
5. Chỉ giữ những tầng/thư mục cần dùng. Backend và shared là tùy chọn.
6. Bổ sung cấu hình của công nghệ đã chọn; không dùng tài khoản, khóa hoặc
   cấu hình máy của dự án nguồn cho dự án mới.

QUY TẮC CHÍNH
- Chia theo tính năng trước; trong tính năng chia presentation/domain/data.
- bootstrap nối các thành phần; navigation quản lý điều hướng.
- core chỉ chứa nền tảng và thành phần dùng chung trong một ứng dụng.
- shared chỉ chứa phần thực sự cần dùng giữa nhiều ứng dụng hoặc server.
- Mỗi trạng thái/nghiệp vụ có một nơi chịu trách nhiệm chính.
- Không cần tạo đủ mọi tầng cho tính năng đơn giản, không thêm Base/Utils
  khi chưa có nhu cầu cụ thể.

NGUỒN THAM CHIẾU
../app-legendverse/docs/architecture/README.md
../app-legendverse/app/src/main/java/com/example/myapplication/

Đây là khung đã khái quát, không phải bản sao nguyên trạng của dự án nguồn.
Tên feature, mã trò chơi, tranh, dữ liệu người dùng, cấu hình Firebase,
cache và build của Legendverse không thuộc bộ khung này.

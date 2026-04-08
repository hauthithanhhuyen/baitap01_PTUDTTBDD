# baitap01_PTUDTTBDD
# Phần A: Đăng ký tên miền và cấu hình Cloudflare
B1.Truy cập vào trang web của nhà cung cấp tên miền (ví dụ: Mắt Bão, Tenten, iNet...)
Đăng kí tên miền thành công
<img width="1879" height="800" alt="image" src="https://github.com/user-attachments/assets/cd8f73ce-0b09-4492-a018-42bfa7973feb" />
Bước 2: Tạo tài khoản Cloudflare
Truy cập dash.cloudflare.com/sign-up
Nhập Email và Mật khẩu để tạo tài khoản miễn phí.
Vào email của bạn để bấm link xác thực tài khoản từ Cloudflare gửi tới.
<img width="1282" height="821" alt="image" src="https://github.com/user-attachments/assets/10ccde04-c68e-4261-8422-5fbd51c7244b" />
Bước 3: Thêm Domain vào Cloudflare
Đăng nhập vào Cloudflare, tại trang chủ (Dashboard), bấm vào nút "Add a Site" hoặc "Add a Domain".
Nhập tên miền bạn vừa đăng ký thành công (vd: ten-cua-ban.id.vn) và bấm Continue.
Ở màn hình chọn gói cước (Plan), hãy cuộn xuống dưới cùng và chọn gói Free ($0), sau đó bấm Continue.
Cloudflare sẽ quét các bản ghi DNS hiện tại (cứ để mặc định và bấm Continue).
<img width="1914" height="1042" alt="image" src="https://github.com/user-attachments/assets/82638665-d24b-420b-b137-051cbe1c1edd" />
Bước 4: Trỏ Nameserver từ Mắt Bão về Cloudflare
Đăng nhập vào trang quản lý dịch vụ (id.matbao.net) của Mắt Bão.
Tìm đến mục Quản lý tên miền -> Chọn tên miền bạn vừa đăng ký.
Tìm phần Cập nhật Nameserver (hoặc Đổi máy chủ DNS).
Xóa các Nameserver mặc định của Mắt Bão và dán 2 dòng Nameserver của Cloudflare bạn vừa copy ở Bước 3 vào.
Lưu lại. Quá trình cập nhật DNS có thể mất từ 15 phút đến vài tiếng.
<img width="1899" height="903" alt="image" src="https://github.com/user-attachments/assets/030fa804-c536-4564-a596-e93ca6657280" />
# B. Cài đặt Ubuntu + Docker
1.Ubuntu+Doker e đã cài từ kì trước 
<img width="1266" height="637" alt="image" src="https://github.com/user-attachments/assets/2795452a-6912-4903-8fcf-27d1726f65f7" />
<img width="1910" height="1004" alt="image" src="https://github.com/user-attachments/assets/1a5c0b34-ef33-4c4e-90a1-1cf810118e45" />
2.B2. Cấu hình SSH
<img width="1718" height="946" alt="image" src="https://github.com/user-attachments/assets/fa5c07e4-cd3f-4105-b709-535337a00130" />
Cấu hình mạng trong Ubuntu (và công cụ giả lập) để cho phép truy cập SSH vào Ubuntu từ cmd của windows thành công.
<img width="1393" height="736" alt="image" src="https://github.com/user-attachments/assets/37658545-973c-411c-8c94-838de8a01cfe" />
3.CÀI DOCKER
<img width="1912" height="988" alt="image" src="https://github.com/user-attachments/assets/b519f44f-52cb-4adb-874a-59881151133a" />
 4.Kiểm tra cài thành công
<img width="719" height="166" alt="image" src="https://github.com/user-attachments/assets/dfd9a184-010f-4121-9022-44d4c5c8a610" />
5.Cấu hình để docker chạy mà không cần tiền tố sudo
<img width="1140" height="585" alt="image" src="https://github.com/user-attachments/assets/518552cd-c417-4b10-b755-ad1edb3be822" />
6.Đảm bảo tường lửa trên Ubuntu đã cho phép các cổng 80, 1880, 9630 (Lệnh: sudo ufw allow ...)
# C. Cấu hình docker compose
1.Tạo thư mục: ~/myapp
2.Tạo web cá nhân
<img width="1919" height="986" alt="image" src="https://github.com/user-attachments/assets/b10d18e3-bb70-4abc-ac3f-a1832f98bce1" />




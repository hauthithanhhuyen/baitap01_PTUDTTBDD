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
2.Cài container đã chạy
<img width="1429" height="93" alt="image" src="https://github.com/user-attachments/assets/706b4c18-88e5-4591-90b9-68d7daecc39b" />
3.Cấu hình nginx.conf
<img width="1078" height="625" alt="image" src="https://github.com/user-attachments/assets/f7222c8b-654b-444b-86e8-555f6c60986a" />
4. Sửa docker-compose.yml
<img width="955" height="579" alt="image" src="https://github.com/user-attachments/assets/2ac5caea-e8e7-414d-8095-d10852f7e176" />
5.Tạo web tĩnh
<img width="718" height="442" alt="image" src="https://github.com/user-attachments/assets/c497d420-5029-41b0-bb9f-fb3f8fafa115" />
6.Kiểm tra web tĩnh
<img width="799" height="347" alt="image" src="https://github.com/user-attachments/assets/8250520b-23a1-4d76-96b3-a254132dc6fd" />
http://localhost:8080
<img width="1891" height="934" alt="image" src="https://github.com/user-attachments/assets/140a79b2-52dc-4969-a2c5-a846381add33" />
Tạo API và cấu hình
<img width="778" height="347" alt="image" src="https://github.com/user-attachments/assets/c6ecdd73-a3d3-4c28-aaaa-6e4276b3abc7" />
# D.tạo thư mục ./myapi
<img width="1481" height="380" alt="image" src="https://github.com/user-attachments/assets/43d772d7-217e-4bd8-a5b4-c9287a1e6d1a" />
1.Test Flask trực tiếp
<img width="1005" height="347" alt="image" src="https://github.com/user-attachments/assets/95d99d6f-035a-4372-bb09-fb051beb3837" />
2. Test qua nginx 
<img width="1472" height="730" alt="image" src="https://github.com/user-attachments/assets/b99640f7-7126-44b9-8bea-b20e6be5ccc1" />
 truy cập qua http://localhost:8080/api/funny
<img width="737" height="358" alt="image" src="https://github.com/user-attachments/assets/1487f4f0-99da-4b37-81bf-035fee034273" />
# E. Triển khai (level test) ứng dụng
Tạo api trong nodered
<img width="1624" height="804" alt="image" src="https://github.com/user-attachments/assets/e8078011-58de-4cce-a1b5-9683793edb86" />
Test
<img width="1228" height="517" alt="image" src="https://github.com/user-attachments/assets/f29ad29f-d0bc-4742-85ac-e6ba99144156" />
<img width="1741" height="440" alt="image" src="https://github.com/user-attachments/assets/82805827-3367-4446-b4f6-26ab1d4fed8d" />
# Sửa file ./myweb/index.html : thêm code html+js để sử dụng được api đã khai báo proxy_pass (thực ra là sử dụng nodered http_in hoặc sử dụng service myapi)
Sửa file
<img width="1437" height="677" alt="image" src="https://github.com/user-attachments/assets/fc2fa3ae-0aa8-4be3-8c19-878be9489341" />
# chạy trên :http://localhost:8080
<img width="1320" height="541" alt="image" src="https://github.com/user-attachments/assets/8f72a2f9-ecad-4f2c-a592-20e9c54aa258" />
# F SỬA LỖI
1.1. Kiểm tra container nhanh
<img width="1472" height="273" alt="image" src="https://github.com/user-attachments/assets/0b2992e4-e9fd-4f05-90a5-5b42981e549a" />
2. Thêm HEALTHCHECK cho myapi
<img width="1407" height="902" alt="image" src="https://github.com/user-attachments/assets/3ead68aa-d31b-47f1-bda5-99df99354670" />
Đã có đủ các dữ liệu đã cài thành công
<img width="1843" height="172" alt="image" src="https://github.com/user-attachments/assets/55696aa6-83d0-49a2-8c99-8fe16206d538" />
# G. Triển khai ứng dụng đến End-user
1. Tạo Cloudflare Tunnel
<img width="1639" height="640" alt="image" src="https://github.com/user-attachments/assets/5127b1b2-337d-460f-839f-6fe4a5115bb4" />
<img width="1888" height="617" alt="image" src="https://github.com/user-attachments/assets/06089ea4-37b5-44e8-98c1-7e331409612b" />
<img width="1916" height="617" alt="image" src="https://github.com/user-attachments/assets/a1558cc8-34a0-4426-aebf-45913c923a27" />
<img width="909" height="594" alt="image" src="https://github.com/user-attachments/assets/f7636d6f-e818-4cde-b7a5-6147cebdb94a" />
Chuyển sang
<img width="1889" height="1044" alt="image" src="https://github.com/user-attachments/assets/1b998c6c-bbed-473d-9bcf-96f7ba5224e4" />




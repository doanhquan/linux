# Thiết lập môi trường Linux
  * Có thể cài hệ điều hành nhân Linux hoặc dùng phần mềm ảo hóa cho window như WSL hay Vitural Box
  * Có thể sử dụng Ubuntu hoặc CentOS
  * Sau khi cài đặt xong hệ điều hành chúng ta sẽ tạo mật khẩu root user -> có thể đặt mật khẩu hoặc không (nên đặt vì đây là tài khoản full quyển)
  * Tiếp tục tại 1 tài khoản user (đây là tào khoản làm việc)
# Phân vùng Linux
  * Có ít nhất 3 phân vùng cơ bản '/', boot, swap
  * Swap không có điểm truy cập và là nơi lưu trữ dự liệu tạm thời, là hệ thống quản lí file tên swap, dung lượng bằng ram vật lí (là vitural memory)
  * Phân vùng quan trong nhất là '/' quản lí tất cả các phân vùng . Ví dụ muốn tạo ra phân vùng boot thì tạo ra folder boot bên trong folder '/' sau đo mount phân vùng boot vào folder boot vừa tạo
  * Tất cả các phân vùng được tạo ra thì điểm truy cập đều nằm trong '/' => bất kỳ đường dẫn của đối tượng nào đều bắt đầu bằng '/'
  * ![markdown](https://i.ibb.co/GFn7tzn/Capture.png)

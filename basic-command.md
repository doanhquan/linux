## Kiểm tra kết nối internet
  * ping ip or domain (khi ping cả 2 đều được mới đồng nghĩa với việc cấu hình internet thành công vì đôi khi ping ip thì được doamin thì không là do lỗi cấu hình DNS
## Kiểm tra địa chỉ ip
  * ifconfig, ip addr, ip a
## Kiểm tra hostname
  * hostname (lưu ý không nên đặt tên host có dấu '.' mà phải là không gian tên phẳng ví dụ: hostname thay vì host.name; nếu không khi join vào domain sẽ bị lỗi)
## Cấu hình IP
  1. Cấu hình IP vào file
      * Cấu hình IP ở file: vi /etc/sysconfig/network-scripts/ifcfg-ens33
      * ![markdown](https://i.ibb.co/TK5ZBhZ/ipcfg.png)  
  2. Cấu hình Getway ở file 
      * vi /etc/sysconfig/network
          * NETWORKING=yes
          * HOSTNAME=localhost
          * GETWAY=10.1.1.253
  3. Cấu hình DNS ở file
      * /etc/resolv.conf
          * nameserver 8.8.8.8 
          * nameserver 8.8.4.4
## Khởi động lại network
  * systemctl restart network

Cài đặt debug php 
<br><br>
# B1: Xem thông tin phiên phản của php
``` PHP
<?php
    phpinfo();
?>
```
<br><br>
# B2: Ctrl A và copy trang phpinfo()
<image src="./img/phpinfo.png"></image><br><br>
# B3: Truy cập <a href="https://xdebug.org/wizard.php">https://xdebug.org/wizard.php</a><br>
Paste nội vừa copy vào đây:
<image src="./img/wizard.png"></image><br>
Sau đó kích vào <b>Analyse my phpinfo() output</b>, ta được kết quả:
<image src="./img/1.png"></image><br><br>
# B4: Download <a href="https://xdebug.org/files/php_xdebug-3.2.0-8.1-vs16-x86_64.dll">php_xdebug-3.2.0-8.1-vs16-x86_64.dll</a><br><br>
# B5: Di chuyển file <b>php_xdebug-3.2.0-8.1-vs16-x86_64.dll</b> vào thư mục <b>D:\xampp\php\ext</b><br><br>
# B6: Vào thư mục chứa xampp, chỉnh sửa file php.ini.<br>Ví dụ: <b>D:\xampp\php\php.ini</b><br>
Thêm nội dung sau:

[XDebug]<br>
xdebug.remote_enable = 1<br>
xdebug.remote_autostart = 1<br>
zend_extension = D:\xampp\php\ext\php_xdebug-3.2.0-8.1-vs16-x86_64.dll<br>
<image src="./img/phpinitdebug.png"></image>
<br><br>
# B7: Tải extension PHP debug trong VSCode.
<image src="./img/ext.png"></image>
# Thử nghiệm:<br>
- Cho một file <b>a.php</b> có nội dung:<br>
<image src="./img/test1.png"></image><br>
- Để bật chế độ debug nhân tổ hợp phím <b>Ctrl+Shift+D</b><br>
<image src="./img/test2.png"></image><br>
- Chọn 2 vị trí Breakpoint là điểm đầu và điểm kết thúc.<br>
<image src="./img/test4.png"></image>
<br>
<video src="./img/bandicam 2023-02-09 16-02-44-815.mp4" controls="controls" style="max-width: 730px;">Video
</video>
<a href="./img/bandicam 2023-02-09 16-02-44-815.mp4">Video</a>

# lab37_html
37lab's html

nginx作反向代理的时候
在/etc/ngnix/sites-enable/   新建lab37文件
 lab37内容如下:
  server {
      listen 80;
	  listen [::]:80;
	  root /var/www/html/lab37; #lab37文件夹中放此网站的静态文件
	  index  index.html;
	  server_name lab37.cn www.lab37.cn  37lab.cn  www.37lab.cn;
  }
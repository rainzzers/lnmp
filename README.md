安装
============
```bash
git clone https://github.com/dantinr/lnmp.git
cd ezhttp-master
chmod +x start.sh
```
Interactive installation
```bash
./start.sh
```

Non-interactive installation
```bash
./start.sh -h #  option h to print help info
```

Default Location
=============================
| Nginx Location             |                                  |
|----------------------------|----------------------------------|
| Install Prefix             | /usr/local/nginx                 |
| Main Configuration File    | /usr/local/nginx/conf/nginx.conf |
| Virtual Host Configuration | /usr/local/nginx/conf/vhost/     |

| Apache Location            |                                   |
|----------------------------|-----------------------------------|
| Install Prefix             | /usr/local/apache                 |
| Main Configuration File    | /usr/local/apache/conf/httpd.conf |
| Virtual Host Configuration | /usr/local/nginx/conf/vhost/      |

| PHP Location           |                               |
|------------------------|-------------------------------|
| Install Prefix         | /usr/local/php                |
| Ini Configuration File | /usr/local/php/etc/php.ini    |
| FPM Configuration File | /usr/local/apache/conf/vhost/ |

| MySQL Location            |                                       |
|---------------------------|---------------------------------------|
| Install Prefix            | /usr/local/mysql                      |
| Data Location             | /usr/local/mysql/data                 |
| my.cnf Configuration File | /usr/local/mysql/etc/my.cnf           |
| Error Log Location        | /usr/local/mysql/data/mysql-error.log |
| Slow Log Location         | /usr/local/mysql/data/mysql-slow.log  |

Process Management
==================
| Process | Command                                  |
|---------|------------------------------------------|
| nginx   | /etc/init.d/nginx (start\|stop\|restart)   |
| apache  | /etc/init.d/httpd (start\|stop\|restart)   |
| php-fpm | /etc/init.d/php-fpm (start\|stop\|restart) |
| mysql   | /etc/init.d/mysqld (start\|stop\|restart)  |

ez command description
=======================
| Command | Description                                  |
|---------|------------------------------------------|
| ez vhost add   | create virtual host   |
| ez vhost list  | list all virtual host   |
| ez vhost del | remove a virtual host |
| ez mysql reset  | reset mysql password  |
| ez mysql add  | create a mysql user   |
| ez mysql mod  | modify a mysql user   |
| ez mysql del  | delete a mysql user   |
| ez ftp add  | add a ftp user   |
| ez ftp list  | list ftp user   |
| ez ftp del  | delete a ftp user   |
| ez ftp mod  | modify a ftp user   |

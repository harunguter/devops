```sh
sudo apt update
sudo apt install apache2 -y
sudo apt install php -y
sudo apt install php-mysql -y
sudo apt install mysql-server -y
```

```sh
sudo mysql
```

```sql
SELECT user,authentication_string,plugin,host FROM mysql.user;
ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'Abc12345.';
CREATE USER 'admin'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'Abc54321.';
GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;
```

```sh
sudo /etc/init.d/apache2 restart
sudo apt install phpmyadmin -y
sudo ln -sf /usr/share/phpmyadmin /var/www/html/phpmyadmin
```

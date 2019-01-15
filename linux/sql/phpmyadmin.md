can not show phpmyadmin after installation
sudo -H gedit /etc/apache2/apache2.conf
Then add the following line to the end of the file:
Include /etc/phpmyadmin/apache.conf
Then restart apache: 
/etc/init.d/apache2 restart

change password of user root
mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'feav';
Query OK, 0 rows affected (0.00 sec)

mysql> exit
Bye
feav@embolo:~$ sudo service mysql restart


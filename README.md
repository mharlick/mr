sudo apt update

sudo apt upgrade

sudo apt install apache2

sudo systemctl status apache2

sudo apt install mysql-server

sudo apt-get install mysql-common

sudo mysql

use mysql; # use mysql table
update user set authentication_string=PASSWORD("m") where User='root'; 
update user set plugin="mysql_native_password" where User='root'; 

flush privileges;
quit;


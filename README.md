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

sudo apt install php libapache2-mod-php

sudo systemctl restart apache2

sudo apt install mysql-workbench

sudo apt updatesudo apt install software-properties-common apt-transport-https wget

wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

sudo apt install code

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

sudo apt-get install php-common php-mbstring php-xml php-zip

sudo apt install php-bcmath

sudo systemctl restart apache2

sudo apt install mysql-workbench

sudo apt updatesudo apt install software-properties-common apt-transport-https wget

wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

sudo apt install code

sudo mysql

update mysql.user set plugin = 'mysql_native_password' where User='root';
// to change the password too (credits goes to Pothi Kalimuthu)
// UPDATE mysql.user SET plugin = 'mysql_native_password', Password = PASSWORD('secret') WHERE User = 'root';
FLUSH PRIVILEGES;



php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

php -r "if (hash_file('sha384', 'composer-setup.php') === '93b54496392c062774670ac18b134c3b3a95e5a5e5c8f1a9f115f203b75bf9a129d5daa8ba6a13e2cc8a1da0806388a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

php composer-setup.php

php -r "unlink('composer-setup.php');"

mv composer.phar /usr/local/bin/composer

composer global require laravel/installer

add: export PATH=$HOME/.config/composer/vendor/bin:$PATH to .bashrc

laravel new web-app

sudo a2enmod rewrite

sudo systemctl restart apache2

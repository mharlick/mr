## Creating a DEV server
#### Download and install Ubuntu 18.04.1 desktop image
**run the following from a commmand prompt**

$ sudo apt update

$ sudo apt upgrade

$ sudo apt install apache2

$ sudo apt install mysql-server mysql-common mysql-client

mysql> use mysql; # use mysql table
mysql> update user set plugin="mysql_native_password" where User='root'; 
mysql> update user set authentication_string=PASSWORD("m") where User='root'; 
mysql> flush privileges;
mysql> quit;

$ sudo apt install php libapache2-mod-php

$ sudo apt-get install php-common php-mbstring php-xml php-zip

$ sudo apt install php-bcmath

$ sudo apt-get install php7.0-mysql

$ sudo systemctl restart apache2

$ sudo apt install mysql-workbench

$ sudo apt install software-properties-common apt-transport-https wget

$ php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"

$ php -r "if (hash_file('sha384', 'composer-setup.php') === '93b54496392c062774670ac18b134c3b3a95e5a5e5c8f1a9f115f203b75bf9a129d5daa8ba6a13e2cc8a1da0806388a8') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

$ php composer-setup.php

$ php -r "unlink('composer-setup.php');"

$ sudo mv composer.phar /usr/local/bin/composer

$ composer global require laravel/installer

add-> export PATH=$HOME/.config/composer/vendor/bin:$PATH to .bashrc

$ laravel new web-app

$ sudo a2enmod rewrite

$ sudo systemctl restart apache2

% sudo vi /etc/apache2/sites-enabled/000-default.conf

<VirtualHost *:80>
       ServerAdmin webmaster@localhost
       DocumentRoot /home/m/web-app/public
        ServerName m

         <Directory /home/m/web-app/public>
                Options +FollowSymLinks
                AllowOverride All
                Require all granted
         </Directory>
</VirtualHost>

$ sudo systemctl restart apache2

update .env with db settings

create meetingroom schema and user

$ cd web-app/storate

$ sudo apt install nodejs npm

$ composer global require laravel/installer

$ sudo apt install git

$ git clone https://github.com/laravel/spark-installer.git

$ cd spark-installer

$ composer install

$ chmod -R 777 *

$ sudo apt-get install php-curl

add: export PATH=$HOME/spark-installer:$HOME/.config/composer/vendor/bin:$PATH to .bashrc

$ spark register token-value

$ spark new web

change dir wen-app to web1 and web to web-app

$ sudo systemctl restart apache2

$ cd storage

$ chmod -R 777 *

#### Optional : vscode

$ wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

sudo apt install code


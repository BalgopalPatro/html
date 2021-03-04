### LAMP on Ubuntu - [Source](https://web.archive.org/web/20180323030918/https://howtoubuntu.org/how-to-install-lamp-on-ubuntu) [PHP](https://web.archive.org/web/20200923164429/https://www.cloudbooklet.com/upgrade-php-version-to-php-7-4-on-ubuntu/)

````

sudo apt-get install apache2
sudo apt-get install mysql-server
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update && sudo apt-get upgrade && sudo apt update && sudo apt upgrade
sudo apt install php8.0 libapache2-mod-php8.0
sudo apt install php8.0-fpm libapache2-mod-fcgid
sudo a2enmod proxy_fcgi setenvif
sudo a2enconf php8.0-fpm
sudo service apache2 restart
php -r 'echo "\n\nYour PHP installation is working fine.\n\n\n";'
cd /var/www
sudo rm -r html
sudo git clone https://github.com/BhadooCloud/html
cd /var/www/html
````

https://certbot.eff.org/lets-encrypt/ubuntufocal-apache

### Rapidleech [RAR Fix](https://web.archive.org/web/20201011110252/https://github.com/Th3-822/rapidleech/issues/71)

````
cd /var/www/html
````

````
sudo rm -rf rar && sudo wget https://rarlab.com/rar/rarlinux-x64-5.6.0.tar.gz && sudo tar -xvf rarlinux-x64-5.6.0.tar.gz && sudo rm -f rarlinux-x64-5.6.0.tar.gz && sudo chmod -R 777 rar && sudo chmod -R 777 rar/*
````

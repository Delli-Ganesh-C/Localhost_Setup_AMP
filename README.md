# Localhost_Setup_AMP( Ubundu )
Steps to setup localhost with Apache, MySql and Php

**Apache Web Server Installation**

- sudo apt-get update
- sudo apt-get upgrade
- sudo apt-get install apache2 apache2-utils
- sudo systemctl enable apache2
- sudo systemctl start apache2
- sudo systemctl status apache2
- sudo ufw allow in "Apache"
- sudo ufw status

You can check the webserver by hitting localhost in the browser.

**MySQL Database Server Installation**

- sudo apt-get install mysql-client mysql-server
- sudo apt-get install mariadb-server mariadb-client
- sudo mysql_secure_installation 

Done. Now you can access the MySql through terminal using the credentials which you provided in the above steps

**PHP Installation**

- sudo apt-get install php libapache2-mod-php php-mysql php-curl php-gd php-mbstring php-xml php-xmlrpc php-soap php-intl php-zip
- sudo systemctl restart apache2
- sudo vi /var/www/html/info.php
- Add phpinfo(); inside the info file to check the Php information.

That's it :).

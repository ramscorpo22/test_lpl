to run the following test you must install symfony client+lampp/xampp enviroment
for windows:
install xampp, prefered, run, use shell located in the app and run symfony --version to ensure installation.
if not, install through the shell the client.
access to the project folder and comand serve eg. "symfony test serve"
for linux:
install lampp using terminal  using command: 
-sudo apt install apache2
verify its running
sudo systemctl status apache2
update firewall
sudo ufw allow in "Apache Full"
install sql server (optional)
sudo apt install mysql-server
# or to install MariaDB (recommended on some distros)
sudo apt install mariadb-server
install php
sudo apt install php libapache2-mod-php php-mysql
restart apache
sudo systemctl restart apache2
install dependencies
sudo apt install php php-cli php-json php-ctype php-curl php-mbstring php-xml php-zip php-tokenizer libpcre3 git zip unzip
install symfony
# Using wget
wget https://get.symfony.com/cli/installer -O - | bash

# Or using curl
curl -sS https://get.symfony.com/cli/installer | bash
move to global permissions
mv ~/.symfony5/bin/symfony /usr/local/bin/symfony
after
cd my_project_name
symfony server:start

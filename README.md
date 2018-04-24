# Reference: https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04
# Here we go

    sudo apt-get update
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/img.png)
    
    sudo apt-get install apache2
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/img.png)
    
    sudo apache2ctl configtest
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/3.png)
    
    sudo nano /etc/apache2/apache2.conf
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/4.png)
    
    sudo apache2ctl configtest
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/5.png)
        
    sudo systemctl restart apache2    
    
    sudo ufw app list
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/6.png)
        
    sudo ufw app info "Apache Full"
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/7.png)
    
    sudo ufw allow in "Apache Full"
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/8.png)
    
    Running it http://localhost/ in your URL bar
    
    sudo apt-get install mysql-server
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/9.png)
    
    mysql_secure_installation
    Password: Abc@123456 (yes and 1)
    
    sudo apt-get install php libapache2-mod-php php-mcrypt php-mysql
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/10.png)
        
    sudo nano /etc/apache2/mods-enabled/dir.conf
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/11.png)
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/12.png)
    
    Ctrl + X => Y => Enter
    
    sudo systemctl restart apache2
    sudo systemctl status apache2
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/13.png)
    
    apt-cache search php- | less
    ![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/to/14.png)
    
    sudo nano /var/www/html/info.php
    type code:
    <?php
      phpinfo();
    ?>
    
    
        
    
    

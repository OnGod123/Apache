pawnshopp.conf


# Assuming DocumentRoot is set to /var/www/html/pawesome_pets

<VirtualHost *:80>
  ServerName pawsomepets.local  # Replace with your domain name (if applicable)
  ServerAlias www.pawsomepets.local  # Optional alias

  DocumentRoot /var/www/html/pawesome_pets

  <Directory /var/www/html/pawesome_pets>
    Require all granted
  </Directory>

  ErrorLog ${APACHE_LOG_DIR}/error.log
  CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>

sudo a2ensite tikiwiki.conf
sudo a2enmod rewrite
sudo systemctl restart apache2.service
README.md


APACHE is the biggest webserver the Task focus on working with and configuriung
Apache
yourDomain.conf


<VirtualHost *:80>
     ServerAdmin admin@YourDomain.com
     DocumentRoot /var/www/html/tikiwiki
     ServerName YourDomain.com

     <Directory /var/www/html/tikiwiki/>
          Options FollowSymlinks
          AllowOverride All
          Require all granted
     </Directory>

     ErrorLog ${APACHE_LOG_DIR}/error.log
     CustomLog ${APACHE_LOG_DIR}/access.log combined

</VirtualHost>
sudo a2ensite tikiwiki.conf
sudo a2enmod rewrite
C:\Users\Grizzy_bear\apache_deployment>



























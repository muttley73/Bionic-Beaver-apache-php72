ubuntu 7.10 apache + php7.1
dev enviroment setup.
php error reporting enabled on E_ERROR | E_WARNING | E_PARSE/

installed modules:

php7.2-mysql
libapache2-mod-php7.2
php7.2-curl
php7.2-cli
php7.2-json
php7.2-sqlite3
php7.2-intl
php7.2-dev
php7.2-gd
php7.2-mbstring
php7.2-mcrypt
php7.2-zip

volumes:

/var/www/html
/var/log/apache2
/etc/apache2/sites-enabled
/etc/apache2/
/etc/php/7.0/apache2/

apache-user: webmgr uid 1000
expose port: 80
start: apache2ctl (not supervisord)


This is a basic LEMP set-up to use WordPress with docker-compose.

It includes these containers:
- wordpress:php7.4-fpm-alpine
- mariadb:10
- nginx:1.17-alpine
- phpmyadmin/phpmyadmin

For the DB, please fix an .env file that includes:
```
MYSQL_ROOT_PASSWORD=password
MYSQL_USER=wordpress
MYSQL_PASSWORD=1
```
Change these values for your own.

Once in phpmyadmin, you can log in as root, to check all the databases, or 
as WordPress user, and be able to check only your WordPress database.

I used port 80 for the site, and 8080 for phpmyadmin, please feel free to
change these as by your needs.
# my_laradock

# [laravel](https://g3n1k.wordpress.com/2021/07/31/setup-laravel-dengan-laradock/)
# https://codesyariah122.github.io/environment-development-dengan-laradock/

# add on file .env
DB_HOST=mysql
REDIS_HOST=redis
QUEUE_HOST=beanstalkd

# change on file default.conf
server_name localhost;
    root /var/www/your project/public;

# add section location
location / {
         try_files $uri $uri/ /index.php$is_args$args;
    }

# delete or commnet
location ~ \.php$ {
        # try_files $uri /index.php =404;

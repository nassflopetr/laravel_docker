FROM php:7.4-fpm

RUN apt-get update && apt-get install -y cron \
    && docker-php-ext-install pdo_mysql

COPY ./root /var/spool/cron/crontabs/

RUN crontab /var/spool/cron/crontabs/root

CMD ["cron", "-f"]

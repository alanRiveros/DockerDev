FROM ubuntu:14.04

RUN apt-get update && apt-get install -y php5-fpm php5-json php5-intl php5-mysqlnd

ADD entrypoint.sh /entrypoint.sh

EXPOSE 900php5-json ph php5-mysqlnd

ADD entrypoint.sh /entrypoint.sh

EXPOSE 9000

WORKDIR /var/www

ENTRYPOINT["/entrypoint.sh"]

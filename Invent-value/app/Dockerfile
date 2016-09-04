FROM php:5.6-apache
RUN apt-get update \
    && apt-get install -y \
        libmcrypt-dev \
        libzmq-dev \
        php5-mysql \
        supervisor \
    && pecl install zmq-beta \
    && docker-php-ext-install -j$(nproc) mcrypt \
    && docker-php-ext-enable zmq
RUN mkdir -p /var/log/supervisor
ADD ./supervisor/invent-value.conf /etc/supervisor/conf.d/

FROM debian:squeeze
MAINTAINER Claudio Amaral "claudio.amaral@africainternetgroup.com"

RUN apt-get update && apt-get install --no-install-recommends -y wget curl ca-certificates

RUN echo "deb http://packages.dotdeb.org squeeze all\ndeb-src http://packages.dotdeb.org squeeze all" > /etc/apt/sources.list.d/dotdeb.list  && \
    wget http://www.dotdeb.org/dotdeb.gpg -O /tmp/dotdeb.gpg && apt-key add /tmp/dotdeb.gpg

RUN apt-get update && apt-get install --no-install-recommends -y php5-cli php5-fpm php5-gd php5-curl php5-intl php5-mysql php5-sqlite php5-xmlrpc php5-xsl php5-apc php5-imagick nginx-extras php5-xdebug


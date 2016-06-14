FROM aokinobu/apache
MAINTAINER Nobuyuki Aoki "aokinobu@gmail.com"

RUN a2enmod proxy
RUN a2enmod proxy_http
 
ADD sites-available /etc/apache2/sites-available
 
RUN a2ensite 000-default.conf
RUN a2ensite 010-d2rq.conf
 
CMD ["/run.sh"]

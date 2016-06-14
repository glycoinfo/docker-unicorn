FROM aokinobu/apache
MAINTAINER Nobuyuki Aoki "aokinobu@gmail.com"
 
ADD sites-available /etc/apache2/sites-available
 
RUN a2ensite 000-default.conf
 
CMD ["/run.sh"]

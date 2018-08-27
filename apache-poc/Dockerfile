FROM httpd

MAINTAINER rupalib
COPY httpd.conf /usr/local/apache2/conf/
COPY .htaccess /usr/local/apache2/htdocs
COPY index.html /usr/local/apache2/htdocs
RUN apt-get update
RUN /usr/local/apache2/bin/htpasswd -b -c /home/.htpasswd ruser2 ruser2
RUN chown daemon:root /home/.htpasswd
RUN chmod 0660 /home/.htpasswd

EXPOSE 80



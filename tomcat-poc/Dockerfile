FROM tomcat

MAINTAINER rupalib
RUN apt-get update
RUN wget https://tomcat.apache.org/tomcat-7.0-doc/appdev/sample/sample.war
RUN cp sample.war /usr/local/tomcat/webapps/

EXPOSE 8080



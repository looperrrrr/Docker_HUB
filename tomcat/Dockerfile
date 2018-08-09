FROM tomcat:8.5

COPY ./lib/     /usr/local/tomcat/lib
COPY ./context/ /usr/local/tomcat/webapps/manager/META-INF
COPY ./conf/  /usr/local/tomcat/conf
COPY ./software/ /usr/local/tomcat/webapps

EXPOSE 8080

RUN /usr/local/tomcat/bin/shutdown.sh && /usr/local/tomcat/bin/startup.sh

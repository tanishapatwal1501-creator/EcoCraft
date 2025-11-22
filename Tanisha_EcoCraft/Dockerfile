FROM tomcat:9.0-jdk11

RUN rm -rf /usr/local/tomcat/webapps/ROOT
RUN mkdir -p /usr/local/tomcat/webapps/ROOT

COPY ./*.jsp /usr/local/tomcat/webapps/ROOT/
COPY ./WEB-INF /usr/local/tomcat/webapps/ROOT/WEB-INF
COPY ./css /usr/local/tomcat/webapps/ROOT/css
COPY ./js /usr/local/tomcat/webapps/ROOT/js
COPY ./assets /usr/local/tomcat/webapps/ROOT/assets
COPY ./uploads /usr/local/tomcat/webapps/ROOT/uploads

EXPOSE 8080

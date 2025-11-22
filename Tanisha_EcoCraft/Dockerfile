FROM tomcat:9.0-jdk11

# Clean default ROOT app in Tomcat
RUN rm -rf /usr/local/tomcat/webapps/ROOT

# Create ROOT directory
RUN mkdir -p /usr/local/tomcat/webapps/ROOT

# Copy JSP files
COPY ./*.jsp /usr/local/tomcat/webapps/ROOT/

# Copy WEB-INF
COPY ./WEB-INF /usr/local/tomcat/webapps/ROOT/WEB-INF

# Copy static files
COPY ./css /usr/local/tomcat/webapps/ROOT/css
COPY ./js /usr/local/tomcat/webapps/ROOT/js
COPY ./assets /usr/local/tomcat/webapps/ROOT/assets
COPY ./uploads /usr/local/tomcat/webapps/ROOT/uploads

EXPOSE 8080

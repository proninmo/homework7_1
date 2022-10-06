FROM alpine:3.14
RUN apk update
RUN apk add openjdk8
ENV CATALINA_HOME /usr/local/tomcat
ENV PATH $CATALINA_HOME/bin:$PATH
RUN mkdir -p "$CATALINA_HOME"
WORKDIR $CATALINA_HOME
RUN wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.67/bin/apache-tomcat-9.0.67.tar.gz
RUN tar xvzf apache-tomcat-9.0.67.tar.gz --strip-components 1 --directory /usr/local/tomcat
RUN rm -rf apache-tomcat-9.0.67.tar.gz
CMD ["catalina.sh", "run"]
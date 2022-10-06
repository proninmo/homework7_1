FROM alpine:3.14
RUN apk update
RUN apk add maven git
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
RUN mvn package -f boxfuse-*/
FROM ubuntu:20.04

RUN apt-get update && apt-get install git -y
RUN DEBIAN_FRONTEND=noninteractive apt-get install maven -y 

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/boxfuse-sample-java
WORKDIR /tmp/boxfuse-sample-java
RUN mvn package

RUN mkdir /tmp/art && cp /tmp/boxfuse-sample-java/target/hello-1.0.war /tmp/art

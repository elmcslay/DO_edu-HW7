FROM maven:3.8.7-openjdk-18-slim

RUN apt-get update && apt-get install git -y

RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp/boxfuse-sample-java
WORKDIR /tmp/boxfuse-sample-java
RUN mvn package
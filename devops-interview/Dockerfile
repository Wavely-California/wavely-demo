FROM openjdk:8-jdk-alpine

RUN addgroup -S wavely && adduser -S wavely -G wavely
USER wavely:wavely
WORKDIR /home/wavely

ARG JAR_FILE=target/demo.jar

COPY ${JAR_FILE} app.jar

ENTRYPOINT ["java","-jar","app.jar"]
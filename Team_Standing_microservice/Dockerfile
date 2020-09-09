# Base image as jdk version 14  
FROM openjdk:14

# Refer to Maven build 
ARG JAR_FILE=target/Team_Standing_microservice-0.0.1-SNAPSHOT.jar

# cd /opt/app
WORKDIR /opt/app

# cp target/footballApp.jar /opt/app/app.jar
COPY ${JAR_FILE} app.jar

# java -jar /opt/app/app.jar
ENTRYPOINT ["java","-jar","app.jar"]
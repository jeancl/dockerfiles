FROM openjdk:8-jre-slim
ARG JAR_NAME
ARG JAR_PATH=./target/$JAR_NAME
ADD $JAR_PATH app.jar
VOLUME [ "/tmp", "/target" ]
EXPOSE 8080
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

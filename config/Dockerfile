FROM eclipse-temurin:21-jdk-alpine
RUN apk update && apk add --no-cache tzdata
ENV TZ=America/Bogota
COPY ./target/config-1.0.jar config-service.jar
ENTRYPOINT ["java","-jar","/config-service.jar"]
EXPOSE 8888
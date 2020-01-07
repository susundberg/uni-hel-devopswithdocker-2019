
FROM openjdk:8
ADD spring-example-project /app
WORKDIR /app
RUN ./mvnw package
CMD java -jar ./target/docker-example-1.1.3.jar


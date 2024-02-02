FROM maven:3.9-eclipse-temurin-8 AS builder

WORKDIR /app

COPY . .

RUN mvn clean package -DskipTests

FROM eclipse-temurin:8-jre

WORKDIR /app

COPY --from=builder /app/target/*.jar back_java.jar

CMD ["java", "-jar", "back_java.jar"]

LABEL maintainer=ayoub
FROM java:8

ADD /build/libs/first-microservice-0.0.1-SNAPSHOT.jar first-microservice-0.0.1-SNAPSHOT.jar

EXPOSE 8761

ENTRYPOINT ["java", "-jar", "first-microservice-0.0.1-SNAPSHOT.jar"]

#CMD ["sh", "-c", "java $JVM_ARGS -jar /app/application.jar"] ????? CMD VS ENTRYPOINT
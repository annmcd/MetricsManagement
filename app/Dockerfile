
FROM openjdk:11-jre-slim
COPY target/app-0.0.1-SNAPSHOT.jar app.jar
RUN mkdir -p /recordings
EXPOSE 8080
ENTRYPOINT ["java","-XX:StartFlightRecording:filename=/recordings/recording.jfr,dumponexit=true","-jar","app.jar"]


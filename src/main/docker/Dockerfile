FROM openjdk:8-jre-alpine

ENV SPRING_OUTPUT_ANSI_ENABLED=ALWAYS \
    SLEEP_TIME=0

# add directly the war
ADD *.jar /app.jar

VOLUME /tmp
EXPOSE 9191
CMD echo "The application will start in ${SLEEP_TIME}s..." && \
    sleep ${SLEEP_TIME} && \
    java -jar /app.jar

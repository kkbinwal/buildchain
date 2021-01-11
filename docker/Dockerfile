FROM openjdk:8u131-jre-alpine
#COPY ./build/libs/buildchain.jar /app/buildchain.jar
COPY ./buildchain.jar /app/buildchain.jar
CMD ["java", "-jar", "/app/buildchain.jar"]
EXPOSE 8080
HEALTHCHECK --timeout=40s --interval=1m --retries=3 CMD wget http://localhost:8080/rest/health -O /dev/null

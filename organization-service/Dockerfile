FROM openjdk:8-jre-alpine
ARG APP_VER
ENV APP_FILE organization-service-$APP_VER.jar
ENV APP_HOME /usr/apps
EXPOSE 8080
COPY target/$APP_FILE $APP_HOME/
WORKDIR $APP_HOME
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar $APP_FILE"]
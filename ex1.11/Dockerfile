FROM openjdk:8

WORKDIR /usr/src/app

COPY /material-applications/spring-example-project/ ./

RUN ./mvnw package

EXPOSE 8080

ENTRYPOINT [ "java", "-jar", "./target/docker-example-1.1.3.jar" ]

#commands:
#git clone git@github.com:docker-hy/material-applications.git
#docker build . -t "java-spring-project"
#docker run -p 8080:8080 java-spring-project

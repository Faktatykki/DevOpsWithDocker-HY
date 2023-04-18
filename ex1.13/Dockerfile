FROM golang:1.16

WORKDIR /usr/src/app

COPY /material-applications/example-backend/ ./

RUN go build

EXPOSE 8080

ENV REQUEST_ORIGIN=https://example.com

CMD [ "./server" ]

#commands
#git clone git@github.com:docker-hy/material-applications.git
#docker build . -t "backend-example"
#docker run -p 8080:8080 backend-example

FROM node:16

WORKDIR /usr/src/app

COPY /material-applications/example-frontend/ ./

RUN curl -sL https://deb.nodesource.com/setup_16.x | bash && apt-get install -y nodejs

run npm install

RUN npm run build

RUN npm install -g serve

EXPOSE 5000

CMD [ "serve", "-s", "-l", "5000", "build" ]

#commands:
#git clone git@github.com:docker-hy/material-applications.git
#docker build . -t "frontend-example"
#docker run -p 5000:5000 frontend-example

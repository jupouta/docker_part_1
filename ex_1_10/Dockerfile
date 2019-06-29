FROM ubuntu:16.04
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/path


COPY frontend ./


RUN apt-get update
RUN apt-get -y install curl 


RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install


RUN npm install -g serve


RUN npm install -g webpack webpack-cli


EXPOSE 5000


CMD ["npm", "start"]
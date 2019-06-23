FROM ubuntu:16.04
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/path


COPY backend ./


RUN apt-get update
RUN apt-get -y install curl 


RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN npm install



EXPOSE 8000


CMD ["npm", "start"]
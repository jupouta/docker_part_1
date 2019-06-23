FROM ubuntu:16.04

COPY myscript.sh /
RUN apt-get update && apt-get -y install curl

CMD ["/myscript.sh"]
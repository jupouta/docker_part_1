FROM ruby:latest

COPY rails ./

EXPOSE 3000

RUN apt-get update && apt install -y --allow-unauthenticated nodejs
#RUN apt-get -y install curl

#RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
#RUN apt -y install nodejs

RUN nodejs -v

RUN gem install bundler
RUN bundle install
RUN rails db:migrate
#RUN rake assets:precompile

CMD ["rails", "s"]
#CMD ["rails", "s", "-e", "production"]
FROM ruby:2.6.0
ADD rails-example-project /app
WORKDIR /app
EXPOSE 3000/tcp
RUN bundle install
RUN apt-get update && apt-get install -y nodejs
RUN rails db:migrate
CMD rails s


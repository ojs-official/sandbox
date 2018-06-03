FROM ruby:2.2.2
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /myapp
WORKDIR /myapp
ADD Gemfile Gemfile
ADD Gemfile.lock Gemfile.lock
RUN bundle install 
RUN rails new .
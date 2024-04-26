FROM ruby:2.3.0
RUN apt-get install -y --force-yes
RUN mkdir /myapp
WORKDIR /myapp
COPY Gemfile /myapp/Gemfile
COPY Gemfile.lock /myapp/Gemfile.lock
RUN bundle install
CMD ["rails", "server"]
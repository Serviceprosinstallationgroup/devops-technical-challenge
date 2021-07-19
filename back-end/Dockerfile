#FROM docker.io/library/rails:5
FROM docker.io/library/ruby:2.7.0
#RUN apt-get update -qq && apt-get install -y nodejs postgresql-client
#WORKDIR /myapp
COPY . . 
#Gemfile /myapp/Gemfile
#COPY Gemfile.lock /myapp/Gemfile.lock
RUN gem install bundler:1.17.2
RUN bundle install

# Add a script to be executed every time the container starts.
#COPY entrypoint.sh /usr/bin/
#RUN chmod +x /usr/bin/entrypoint.sh
#ENTRYPOINT []
EXPOSE 3000

# Configure the main process to run when running the image
CMD ["rails", "server"] 
#, "-b", "0.0.0.0"]

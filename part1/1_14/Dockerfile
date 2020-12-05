# docker build --file Dockerfile --tag 1_14 .  
# docker run -it --rm -p 3000:3000 1_14:latest 

FROM ruby:2.6.0-stretch

WORKDIR  /workdir

RUN apt-get update && apt-get install -y nodejs

COPY . .

RUN gem install bundler
RUN bundle install
RUN rails db:migrate

EXPOSE 3000

CMD rails s

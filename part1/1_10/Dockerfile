# Build container inside https://github.com/laojala/frontend-example-docker
# docker build --file Dockerfile --tag 1_10 .
# docker run --rm -p 5000:5000 1_10

FROM node:erbium-buster-slim

EXPOSE 5000

COPY . .

RUN npm install

CMD npm start

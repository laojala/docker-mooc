FROM node:current-alpine3.10

ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools


WORKDIR /robot


#RUN node -v
#RUN npm -v

RUN pip install robotframework robotframework-browser

RUN rfbrowser init

ENTRYPOINT [ "bin/bash" ]
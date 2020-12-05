FROM ubuntu:16.04
WORKDIR /mydir
RUN apt-get update && apt-get install -y curl

COPY script_for_1_7.sh .
RUN chmod +x ./script_for_1_7.sh

ENTRYPOINT  ["./script_for_1_7.sh"]

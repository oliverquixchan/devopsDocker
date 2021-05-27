FROM ubuntu:18.04
WORKDIR /usr/usr/app/
RUN apt-get update && apt-get install curl -y
COPY script.sh .
RUN chmod +x script.sh
CMD ./script.sh
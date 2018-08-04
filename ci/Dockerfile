FROM node:10

RUN apt-get update && \
    apt-get install -y curl unzip && \
    curl -s https://codecov.io/bash > /usr/local/bin/codecov && \
    chmod +x /usr/local/bin/codecov
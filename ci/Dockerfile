FROM node:10

RUN apt-get update && \
    apt-get install -y curl && \
    curl -sSLO https://github.com/codecov/enterprise/releases/download/v4.1.3.zip && \
    unzip v4.1.3.zip && rm v4.1.3.zip && mv ./linux/codecov ./
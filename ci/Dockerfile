FROM node:10
    
RUN apt-get update && \
    apt-get install -y curl unzip apt-transport-https && \
    curl -s https://codecov.io/bash > /usr/local/bin/codecov && \
    chmod +x /usr/local/bin/codecov

RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - && \
    echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list && \
    apt-get update && \
    apt-get install -y yarn

# add greenkeeper lockfile
RUN yarn global add greenkeeper-lockfile
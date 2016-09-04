FROM node:4.4.5

RUN mkdir -p /srv/www/maddog/src/frontend
WORKDIR /srv/www/maddog/src/frontend

RUN apt-get update && apt-get install -y git && rm -rf /var/lib/apt/lists/* \
    && npm install -g bower polymer-cli@0.16.0

RUN echo '{ "allow_root": true }' > /root/.bowerrc
ENV DOCKER_FIX=' '
EXPOSE 8080

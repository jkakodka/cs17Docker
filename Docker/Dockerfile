FROM node:20-alpine
RUN apk add --no-cache python3 make g++ bash bash-doc bash-completion
USER node
ENV NPM_CONFIG_PREFIX=/home/node/.npm-global
ENV PATH=$PATH:/home/node/.npm-global/bin
RUN npm install -g bs-platform
USER root
RUN mkdir -p /home/node/app
VOLUME [ "/cs17volume" ]
WORKDIR /home/node/app`
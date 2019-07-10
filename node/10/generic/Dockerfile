FROM node:dubnium-alpine

RUN apk add --no-cache \
  bash \
  ca-certificates \
  curl \
  git \
  gzip \
  jq \
  openssh \
  tar \
  wget \
  zip

RUN curl -H 'Cache-Control: no-cache' https://raw.githubusercontent.com/fossas/fossa-cli/master/install.sh | bash

RUN curl -L https://codeclimate.com/downloads/test-reporter/test-reporter-latest-linux-amd64 > ./cc-test-reporter

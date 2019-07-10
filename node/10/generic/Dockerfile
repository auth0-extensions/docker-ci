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

RUN mkdir -p ~/fossa && curl -L https://github.com/fossas/fossa-installer/archive/v0.0.21.tar.gz | tar -zxv -C ~/fossa --strip-components=1 && chmod a+x ~/fossa/boot.sh && ln -sf ~/fossa/boot.sh /usr/local/bin/fossa && ~/fossa/setup.sh

RUN curl -L https://codeclimate.com/downloads/test-reporter/test-reporter-latest-linux-amd64 > ./cc-test-reporter

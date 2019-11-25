FROM node:12.13-alpine3.10
USER root
RUN adduser --disabled-password docker && \
  apk add curl && \
  curl -L https://unpkg.com/@pnpm/self-installer | node && \
  mkdir -p /opt/app && \
  chown -R docker /opt/app
USER docker
WORKDIR /opt/app

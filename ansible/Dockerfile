FROM hashicorp/vault:1.18.4
ARG UID
ARG GID
RUN echo http://dl-2.alpinelinux.org/alpine/edge/community/ >> /etc/apk/repositories
RUN apk add -U shadow
RUN groupmod -g $GID vault && usermod -u $UID -g $GID vault
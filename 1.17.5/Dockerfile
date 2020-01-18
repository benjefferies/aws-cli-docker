FROM python:3.8.1-alpine

# Versions: https://pypi.python.org/pypi/awscli#downloads
ENV AWS_CLI_VERSION 1.17.5

RUN apk --no-cache update && \
    apk --no-cache add ca-certificates groff less && \
    pip3 --no-cache-dir install awscli==${AWS_CLI_VERSION} && \
    rm -rf /var/cache/apk/*

WORKDIR /data

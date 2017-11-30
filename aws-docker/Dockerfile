FROM python:3.6.3-alpine3.4
LABEL maintainer="dag.heradstveit@sonat.no"
 
RUN apk update && \
    apk upgrade  && \
    apk add python python-dev py-pip && \
    pip install awscli

RUN apk add curl && \
    curl -o /usr/local/bin/ecs-cli https://s3.amazonaws.com/amazon-ecs-cli/ecs-cli-linux-amd64-latest && \
    chmod +x /usr/local/bin/ecs-cli
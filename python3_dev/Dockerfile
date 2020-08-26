# Dockerfile to create an image based on stock Ubuntu 16.04 image
#
# Your source directory is to be mounted on /src at container instantiation.
#
FROM ubuntu:18.04

LABEL Maintainer="ReThought Ltd"
LABEL Description="Ubuntu and Python3 environment"
LABEL Version="1.0"

RUN apt-get update -y && \
    apt-get install -y apt-utils apt-transport-https && \
    apt-get install -y python3 python3-pip python3-dev && \
    apt-get install -y libffi-dev libssl-dev postgresql-client && \
    apt-get install -y curl wget vim && \
    apt-get install -y git-core && \
    apt-get autoremove -y && \
    apt-get autoclean -y

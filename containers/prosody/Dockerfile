FROM ubuntu:20.04

RUN apt update

ARG DEBIAN_FRONTEND=noninteractive

RUN apt upgrade -y

RUN apt install -y links tor prosody lua-bitop lua-zlib nano vim

COPY $PWD/volume/scripts /scripts

RUN chmod 700 /scripts/init.sh

ENTRYPOINT ["/scripts/init.sh"]

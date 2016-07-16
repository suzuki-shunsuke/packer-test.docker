FROM ubuntu:16.04
RUN apt-get update && \
    apt-get install -y software-properties-common && \
    apt-add-repository ppa:ansible/ansible && \
    apt-get update && \
    apt-get install -y ansible && \
    apt-add-repository --remove ppa:ansible/ansible && \
    apt-get purge -y software-properties-common && \
    rm -rf /var/lib/apt/lists/*

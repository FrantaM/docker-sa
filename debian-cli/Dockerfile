FROM jenkins/agent:latest-jdk11

USER root
RUN apt-get update && apt-get install -y --no-install-recommends \
        rsync wget \
    && rm -rf /var/lib/apt/lists/*

# https://github.com/KostyaSha/yet-another-docker-plugin/issues/217
RUN echo "export LANG=C.UTF-8" >> /etc/environment

RUN groupadd -g 999 docker
RUN usermod -aG docker jenkins

USER jenkins

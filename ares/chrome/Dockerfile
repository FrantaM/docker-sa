FROM openjdk:8

USER root

RUN apt-get update -y \
	&& apt-get install -y --no-install-recommends chromium chromium-driver xvfb \
	&& rm -rf /var/lib/apt/lists/* /var/cache/apt/*

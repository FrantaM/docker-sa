FROM frantam/sa-docker-cli:11

USER root

RUN apt-get update -y \
	&& apt-get install -y --no-install-recommends libgtk2.0-0 libgtk-3-0 libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb \
	&& rm -rf /var/lib/apt/lists/* /var/cache/apt/*

USER jenkins

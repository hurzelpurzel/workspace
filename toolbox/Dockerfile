FROM wbitt/Network-Multitool

RUN apk -y install openssl skopeo docker-ce
RUN wget https://github.com/rs/curlie/releases/download/v1.6.9/curlie_1.6.9_linux_amd64.tar.gz -O - | tar xzf - \
    && mv curlie /usr/local/bin
RUN mkdir /opt/workdir && chmod 777 /opt/workdir
ENV HOME /opt/workdir
WORKDIR /opt/workdir
ENTRYPOINT  ["/bin/sh", "-c", "sleep infinity"]

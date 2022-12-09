FROM redhat/ubi9-minimal

RUN microdnf -y install wget openssl skopeo podman
RUN wget https://github.com/rs/curlie/releases/download/v1.6.9/curlie_1.6.9_linux_amd64.tar.gz -O - | tar xzf - \
    && mv curlie /usr/local/bin 
ENTRYPOINT  ["/bin/sh", "-c", "sleep infinity"]

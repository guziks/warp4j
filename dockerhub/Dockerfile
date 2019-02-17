FROM debian:stable-slim
RUN apt-get update && apt-get install -y \
        curl \
        file \
        unzip \
        zip \
    && rm -rf /var/lib/apt/lists/*
RUN curl -fsSL -o /tmp/warp-packer \
        https://github.com/dgiagio/warp/releases/download/v0.3.0/linux-x64.warp-packer \
    && install -D \
        --mode=755 \
        --owner=root \
        --group=root \
        /tmp/warp-packer \
        /usr/local/bin \
    && rm /tmp/warp-packer
RUN curl -fsSL -o /tmp/warp4j \
        https://raw.githubusercontent.com/guziks/warp4j/stable/warp4j \
    && install -D \
        --mode=755 \
        --owner=root \
        --group=root \
        /tmp/warp4j \
        /usr/local/bin \
    && rm /tmp/warp4j
WORKDIR /workdir
ENTRYPOINT [ "/usr/local/bin/warp4j" ]

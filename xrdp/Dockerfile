FROM debian:stable-slim

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        xrdp \
        && rm -rf /var/lib/apt/lists/*

EXPOSE 3389

CMD ["/usr/sbin/xrdp", "--nodaemon"]

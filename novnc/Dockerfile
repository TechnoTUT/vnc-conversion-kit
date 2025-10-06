FROM debian:stable-slim

RUN apt-get update && \
    apt-get install -y novnc python3-websockify \
        && rm -rf /var/lib/apt/lists/*

EXPOSE 6080

ENTRYPOINT [ "websockify", "-D", "--web", "/usr/share/novnc/"]

CMD ["6080", "localhost:5900"]
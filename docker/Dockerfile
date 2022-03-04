FROM golang:latest

# install updates
RUN apt-get update \
  && apt-get dist-upgrade -y \
  && rm -rf /var/lib/apt/lists/*

# install lmd
RUN go install github.com/sni/lmd/v2/lmd@latest

# install example configuration
COPY lmd.ini.example /etc/lmd.ini

# prepare ports
EXPOSE 6557/tcp

# default command
CMD ["/go/bin/lmd", "-config", "/etc/lmd.ini"]

FROM alpine:3.17

RUN apk add --no-cache \
    bash \
    bind-tools \
    iptables \
    ip6tables \
    openvpn3

COPY . /usr/local/bin

ENV KILL_SWITCH=off
ENV VPN_CONFIG_FILE=radicalsubject.ovpn

ENTRYPOINT [ "entry.sh" ]

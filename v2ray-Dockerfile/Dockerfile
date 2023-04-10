FROM alpine:latest
LABEL maintainer "svk salvikie@163.com"

WORKDIR /root
ARG TARGETPLATFORM=linux/amd64
COPY v2ray.sh /root/v2ray.sh

RUN set -ex \
	&& apk add --no-cache tzdata openssl ca-certificates \
	&& mkdir -p /etc/v2ray /usr/local/share/v2ray /var/log/v2ray \
	&& chmod +x /root/v2ray.sh \
	&& /root/v2ray.sh "${TARGETPLATFORM}"

#VOLUME /etc/v2ray
COPY config.json /etc/v2ray/config.json

CMD [ "/usr/bin/v2ray", "run", "/etc/v2ray/config.json" ]

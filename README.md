# v2ray

cd v2ray-docker-export
cat docker-salvikie-v2ray.tar | docker import - salvikie/v2ray
docker run -itd --restart=always --name=59028.v2ray.server -p 59028:59028 -p 59028:59028/udp salvikie/v2ray /usr/bin/v2ray --config /etc/v2ray/config.json


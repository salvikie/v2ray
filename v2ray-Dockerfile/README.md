# Docker salvikie

docker build -t salvikie/v2ray:latest .

docker run -d --restart=always --name=59028.v2ray.server -p 59028:59028 -p 59028:59028/udp salvikie/v2ray

docker exec -it 59028.v2ray.server /bin/sh

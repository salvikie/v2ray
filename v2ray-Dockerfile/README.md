# install docker
```
curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun


curl https://get.docker.com | bash -s docker
```


# Docker salvikie

docker build -t salvikie/v2ray:latest .

docker run -d --restart=always --name=59028.v2ray.server -p 59028:59028 -p 59028:59028/udp salvikie/v2ray

docker exec -it 59028.v2ray.server /bin/sh


```
docker build -t salvikie-v2ray .

docker run -d --name svk-v2ray --restart always -p 59028:59028 -p 59028:59028/udp salvikie-v2ray

docker exec it svk-v2ray sh

```


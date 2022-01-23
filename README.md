# ddns-dnspod fork from stilleshan/ddns-dnspod

## 简介
基于腾讯云 dnspod.cn DDNS 的 docker 镜像.

## 部署
### docker

```bash
docker run -d --name=ddns-dnspod -e "login_token=123456,35c5abcd08b5bda2600031b090b2f67a" -e "domain=xxx.com" -e "sub_domain=www" -e "interval=10" -e "ip_count=1" ddns-dnspod
```

## 打包

```bash
docker build . -t ddns-dnspod:latest
```



```bash
docker tag ddns-dnspod:latest tza17313/ddns-dnspod:latest
```

```bash
docker push tza17313/ddns-dnspod:latest
```




# caddy-web
## 安装docker
### 1. 创建web_net网络
```bash
docker network create \
  --driver=bridge \
  --subnet=172.22.0.0/16 \
  --gateway=172.22.0.1 \
  --label=com.docker.compose.network=net \
  --label=com.docker.compose.project=web \
  --label=com.docker.compose.version=2.21.0 \
  web_net
```
### 2.启动容器
```bash
docker compose up -d
```

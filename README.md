### 一键设置镜像加速
修改文件 `/etc/docker/daemon.json`（如果不存在则创建）
```shell
sudo mkdir -p /etc/docker
sudo tee /etc/docker/daemon.json <<-'EOF'
{
  "registry-mirrors": ["https://docker.uykb.eu.org"] 
}
EOF
sudo systemctl daemon-reload
sudo systemctl restart docker
```
# 第三方Docker官方镜像服务

### 白嫖哥镜像服务 
```shell
docker.registry.cyou
docker-cf.registry.cyou
```

### Free镜像服务 
```shell
dockercf.jsdelivr.fyi
docker.jsdelivr.fyi
dockertest.jsdelivr.fyi
```

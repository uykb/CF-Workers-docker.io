## 如何使用？

例如您的Workers项目域名为：`docker.fxxk.dedyn.io`；

### 1.官方镜像路径前面加域名
```shell
docker pull docker.fxxk.dedyn.io/stilleshan/frpc:latest
```
```shell
docker pull docker.fxxk.dedyn.io/library/nginx:stable-alpine3.19-perl
```

### 2.一键设置镜像加速
修改文件 `/etc/docker/daemon.json`（如果不存在则创建）
```shell
sudo mkdir -p /etc/docker
sudo tee /etc/docker/daemon.json <<-'EOF'
{
  "registry-mirrors": ["https://docker.fxxk.dedyn.io"]  # 请替换为您自己的Worker自定义域名
}
EOF
sudo systemctl daemon-reload
sudo systemctl restart docker
```

## 变量说明
| 变量名 | 示例 | 必填 | 备注 | 
|--|--|--|--|
| URL302 | https://t.me/CMLiussss |❌| 主页302跳转 |
| URL | https://www.baidu.com/ |❌| 主页伪装(设为`nginx`则伪装为nginx默认页面) |


# 第三方Docker官方镜像服务

### 白嫖哥镜像服务 https://t.me/bestcfipas/1900
```shell
docker.registry.cyou
docker-cf.registry.cyou
```

### Free镜像服务 https://t.me/zero_free/80
```shell
dockercf.jsdelivr.fyi
docker.jsdelivr.fyi
dockertest.jsdelivr.fyi
```

# 鸣谢

[muzihuaner](https://github.com/muzihuaner)、[V2ex网友](https://global.v2ex.com/t/1007922) 、[ChatGPT](https://chatgpt.com/)、[白嫖哥](https://t.me/bestcfipas/1900)、[Free镜像服务](https://t.me/zero_free/80)


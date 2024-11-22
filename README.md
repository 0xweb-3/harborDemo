# harborDemo
harborDemo
```angular2html
wget https://github.com/goharbor/harbor/releases/download/v2.11.2/harbor-online-installer-v2.11.2.tgz
tar -xvzf harbor-online-installer-v2.11.2.tgz
cd harbor

cp harbor.yml.tmpl harbor.yml
```

```angular2html
hostname: 127.0.0.1  # 设置为 localhost 或你的 macOS IP 地址

http:
  port: 8082  # 设置为你希望的服务端口

# 数据存储路径
data_volume: /path/to/harbor/data  #⚠️ 替换为你的本地目录

harbor_admin_password: MySecurePassword  # 设置管理员密码
```

```angular2html
./prepare
docker-compose up -d

docker ps
```
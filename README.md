原项目地址：https://github.com/vveg26/sing-box-reality-hysteria2  
参考项目：https://github.com/liuoqu444/sing-box-reality-hysteria2  

# 提示事项

- 更新源
```bash
apt update -y && apt install -y 
```

- 关闭防火墙
```bash
sudo ufw disable
```

- 查看应用占用的端口
```bash
sudo netstat -tuln
```
没有netstat包处理  
- net-tools安装：
Ubuntu / Debian:  
sudo apt-get install net-tools  
  
Amazon Linux / CentOS / RHEL:  
sudo yum install net-tools  
  
- 启动
```bash
# 启动服务
systemctl start sing-box.service

# 查看启动状态
systemctl status sing-box.service

# 设置开机启动
systemctl enable sing-box.service

# 运行 -c 指定一个配置文件
sing-box run -c /etc/sing-box/config.json
```
  
# 域名推荐  
    gateway.icloud.com (推荐)  
    itunes.apple.com  
    download-installer.cdn.mozilla.net  
    airbnb【这个不同的区有不同的域名建议自己搜索】  
    addons.mozilla.org  
    www.microsoft.com  
    www.lovelive-anime.jp  
  
- CDN  
    Apple:  
    swdist.apple.com  
    swcdn.apple.com  
    updates.cdn-apple.com  
    mensura.cdn-apple.com  
    osxapps.itunes.apple.com  
    aod.itunes.apple.com  
  
- Microsoft:  
    cdn-dynmedia-1.microsoft.com  
    update.microsoft  
    software.download.prss.microsoft.com  
  
- Amazon:  
    s0.awsstatic.com  
    d1.awsstatic.com  
    images-na.ssl-images-amazon.com  
    m.media-amazon.com  
    player.live-video.net  
  
- Google:  
    dl.google.com  

### 三合一脚本  

```bash
bash <(curl -fsSL https://github.com/mijaclan/sing-box-reality-hysteria2/raw/main/beta.sh)
```
  
# 建议  
- 强烈建议开启bbr加速，可大幅加快节点reality和vmess节点的速度
- 安装完成后终端输入 mianyang 可再次调用本脚本


# 新增功能（排序从新到旧）
- 新增sing-box正式版和测试版版本切换
- 任意门，ss解锁流媒体，任意门中转（仅在二合一版本中）
- 全面适配sing-box1.8.0
- 新增更多warp解锁功能，geo和domain_keword,全局接管等
- 新添加了hysteria2端口跳跃功能

# 简介
- Reality Hysteria2 （vmess ws）一键安装脚本
  
## 使用教程

### reality和hysteria2 vmess ws三合一脚本

```bash
bash <(curl -fsSL https://github.com/vveg26/sing-box-reality-hysteria2/raw/main/beta.sh)
```

### reality hysteria2二合一脚本

```bash
bash <(curl -fsSL https://github.com/vveg26/sing-box-reality-hysteria2/raw/main/install.sh)
```

## 功能

- 无脑回车一键安装或者自定义安装
- 完全无需域名，使用自签证书部署hy2，（使用argo隧道支持vmess ws优选ip（理论上比普通优选ip更快））
- 支持修改reality端口号和域名，hysteria2端口号
- 无脑生成sing-box，clash-meta，v2rayN，nekoray等通用链接格式
- 支持warp，任意门，ss解锁流媒体
- 支持任意门中转
- 支持端口跳跃

### warp自定义解锁功能
![](https://img.mareep.net/blog/2023/12/d6fbf369c96dbabb160e67f76dac0d6d.jpg)


## Credit
- [sing-box-example](https://github.com/chika0801/sing-box-examples)
- [sing-reality-box](https://github.com/deathline94/sing-REALITY-Box)
- [sing-box](https://github.com/SagerNet/sing-box)


## 尝鲜区
### tcp-brutal reality(双端sing-box 1.7.0及以上可用)

[文档](https://github.com/apernet/tcp-brutal/blob/master/README.zh.md)

```bash
bash <(curl -fsSL https://github.com/vveg26/sing-box-reality-hysteria2/raw/main/tcp-brutal-reality.sh)
```
### brutal reality vision reality hysteria2三合一(双端sing-box 1.7.0及以上可用)，warp分类，端口跳跃等功能

```bash
bash <(curl -fsSL https://github.com/vveg26/sing-box-reality-hysteria2/raw/main/brutal-reality-hysteria.sh)
```

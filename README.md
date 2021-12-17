# v2ray-conf

v2ray 配置文件仓库  
没有outbounds配置，需要手动添加  

# init
> 启动v2ray之前需要执行的初始化操作

## log
> 因为log.json中写的不是绝对路径，所以启动前需要初始化下日志路径

### mac
> ln -s  ~/Library/Logs/v2ray /Users/zyloong/Cellar/v2ray/4.44.0/bin

## rules
> 规则文件
从[v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)下载路由规则文件  
下载 `geoid.dat` 和 `geosite.dat` 两个文件, 替换v2ray原来的规则文件文件

# 启动v2ray服务时使用如下命令：

**bash**
> nohup v2ray -confdir /usr/local/etc/v2ray &> /dev/null

**windows**
> wv2ray.exe -configdir /conf-path

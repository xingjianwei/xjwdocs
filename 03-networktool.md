# 网络工具

## 访问国外网站工具

### 本机安装软件


### 无线路由器

#### 硬件选择和固件安装

[华硕（ASUS）RT-AC68U 1900M AC双频](https://item.jd.com/1035733.html)

[华硕（ASUS）RT-AC88U 3167M AC 双频](https://item.jd.com/2104499.html)

[Koolshare 论坛](http://koolshare.cn/forum.php)

https://github.com/koolshare/koolshare.github.io

#### 手动安装shadowsocks:

[梅林固件安装SS【shadowsocks】插件教程](https://blog.xtrboy.com/?post=8852)

首先刷好梅林之后进入系统设置界面，在Enable SSH里选择LAN ONLY。

登录无线路由器，用户名填路由器管理员，默认是admin。

```
cd /tmp
wget --no-check-certificate https://raw.githubusercontent.com/koolshare/koolshare.github.io/acelan_softcenter_ui/shadowsocks/shadowsocks.tar.gz
tar -zxvf /tmp/shadowsocks.tar.gz
chmod +x /tmp/shadowsocks/install.sh
sh /tmp/shadowsocks/install.sh
```

重启路由器你就会在软件中心中看见了shadowsocks了。

#### 软件中心插件

http://koolshare.cn/thread-36824-1-1.html

#### 参数设置

MU-MIMO默认是打开的，关掉MU-MIMO有可能解决无线速度跑不满的问题。

2.4G频道带宽是20/40MHz时，300M网卡的连接速度会减半为150M，但据说无线穿透性会强那么一点。2.4G频道带宽改成40MHz时，300M网卡就能满速连接了。

同理，5G频道带宽是20/40/80MHz时，867M网卡的连接速度减半为433M。5G频道带宽改成80MHz时，867M网卡就能满速连接了。

## 网盘

https://115.com

https://pan.baidu.com

## 文件下载工具

### Aria2

[Mac下使用Aria2下载教程----迅雷和百度盘终极解决方案](http://blog.csdn.net/skymyxvincent/article/details/75009226)

直接下载：
`aria2c -c -s10 -x10 --out xxx.file --header 'Cookie: gdriveid=74B66B9A77EE6A3EFB2C70C2F4DDA7AD;'  'url'`

后台模式启动：
`aria2c -D`

#### UI

[ Aria2 WebUI](https://ziahamza.github.io/webui-aria2/)

#### 百度网盘的下载地址导出：

https://github.com/acgotaku/BaiduExporter.git

唯一需要注意的是User-agent需要设置为： netdisk;5.2.7;PC;PC-Windows;6.2.9200;WindowsBaiduYunGuanJia

referer 设置为：http://pan.baidu.com/disk/home 

#### 115网盘

https://github.com/acgotaku/115/

添加额外的Tracker：
`https://github.com/ngosang/trackerslist.git`

`bt-tracker=http://mgtracker.org:2710/announce,http://tracker.istole.it/announce,http://tracker.coppersurfer.tk:6969/announce`
# 网络工具



## 文件下载工具

### Aria2

[Mac下使用Aria2下载教程----迅雷和百度盘终极解决方案](http://blog.csdn.net/skymyxvincent/article/details/75009226)

直接下载：
`aria2c -c -s10 -x10 --out xxx.file --header 'Cookie: gdriveid=74B66B9A77EE6A3EFB2C70C2F4DDA7AD;'  'url'`

后台模式启动：
`aria2c -D`

百度网盘的下载地址导出：

https://github.com/acgotaku/BaiduExporter.git

唯一需要注意的是User-agent需要设置为： netdisk;5.2.7;PC;PC-Windows;6.2.9200;WindowsBaiduYunGuanJia

referer 设置为：http://pan.baidu.com/disk/home 


添加额外的Tracker：
`bt-tracker=http://mgtracker.org:2710/announce,http://tracker.istole.it/announce,http://tracker.coppersurfer.tk:6969/announce`
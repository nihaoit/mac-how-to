# 在终端下无法ping通域名

## 问题现象

终端下无法ping通域名，返回如下的提示

```shell
ping: sendto: No route to host
```

不过可以ping通路由器，所以我想是不是DNS的配置出问题了？

## 解决方法

到系统偏好设置，找到当前正在使用的网卡，在DNS下面默认有一行

```
192.168.1.1
```

在这行的下面添加一行

```
8.8.8.8
```

保存后就可以ping通域名了。







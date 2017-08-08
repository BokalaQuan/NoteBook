# 解决Windows10和Ubuntu16.04时间同步问题



双系统**windows**时间不能正常同步？

* 旧的解决方案

```shell
sudo vim /etc/default/rcS
```

将 utc=yes 改为 utc=no，不可行。

* 新的解决方案

```shell
sudo apt-get install ntpdate
sudo ntpdate time.windows.com
sudo hwclock --localtime --systohc
```

重启进入**windows**， OK！！！
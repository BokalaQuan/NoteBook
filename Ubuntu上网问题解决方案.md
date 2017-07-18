__Ubuntu 16.04__
1. 在终端运行：
```shell
$ sudo gedit /etc/modprobe.d/iwlwifi.conf
```
2. 在配置文件末端空白处添加：
> options iwlwifi 11n_disable=1
3. 保存文件并重启。


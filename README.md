>一个alfred的workflow，它可以通过配置的ssh用户名和密码来进行登录。

#使用方法
1. 下载gsg_alfred_ssh.alfredworkflow，并进行安装。
2. 在新增~/.ssh/ssh_conf文件，并使用以下方式进行添加
```
docker    192.168.59.103    22    root    11    测试用的

```
使用***四个空格***来进行分隔，每个域的意思如下，

- docker，这个ssh的名称
- 192.168.59.103, ssh的ip地址
- 22, ssh的端口
- root,ssh的用户名
- 11，ssh的密码
- 测试用的，ssh的描述

#注意项
1. 使用了python的json模块，如果没有这个模块可能没有办法使用
2. 使用了expect命令来进行登录，需要看看系统是否支持这个命令
3. 使用的是4个空格进行分隔

#建议
如果你是用的是iterm，建议进行以下的设置
https://github.com/stuartcryan/custom-iterm-applescripts-for-alfred
# 命令监控
监控Linux 命令和ssh操作, 并邮件发送报告

### inst.sh
执行安装shell文件 
注意: 安装后请重启ssh登录

### mc.cnf
配置文件路径 /etc/mc/mc.conf

```c
# 记录命令日志的路径 
logPath=/tmp/.s/.his_command.log

# 发送邮件的邮件账号 
mailSender=

# 发送邮件的邮箱账号密码
# 注意: 请使用mcpwd去加密你的密码  
mailPwd=(eg. U2FsdGVkX18/rFRWPNp/dBoD3hPxmPyft+0NJF2lUWg=)

# 邮件服务的 SMTP
mailServer=smtps://smtp.mxhichina.com (enterprise mail)
mailServer=smtps://smtp.aliyun.com (person mail)

# 邮件服务的 PORT
mailPort=465
```

### mccomm 
记录命令的文件

### mcenv 
环境变量 

### mcmail 
发送邮件  
eg. 
```shell
# 发送mc.conf配置的文件
mcmail file: subject recipient
# 发送指定的文件
mcmail file:YOURFILE subject recipient
# 发送附件 
mcmail file:YOURFILE subject recipient accessnory
# 发送文本
mcmail YOURMSG  subject recipient
# 发送文件 & 附件
mcmail YOURFILE subject recipient accessnory
```
### mcpwd 
用于加密邮件账号密码的文件  
eg.  
```shell
1. mcpwd -e YOURMAILPASSWORD
```


### mcuser
记录 用户,IP,和ip相关的实际地址
注: 转换地址需要semi.so扩展,或自行转换

### mccert
生成连接邮箱的证书 用于CA,SSL,-G

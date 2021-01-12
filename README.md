# mc
monitor Linux  command or ssh operate  and mail report

### inst.sh
execute install mc  
NOTE: restart ssh  login after install mc

### config file
/etc/mc/mc.conf
```c
# log path 
# record log file
logPath=/tmp/.s/.his_command.log

# mail sender is your account
mailSender=

# mail pwd is your mail password 
# please use mcpwd to encrypt your password
mailPwd=(eg. U2FsdGVkX18/rFRWPNp/dBoD3hPxmPyft+0NJF2lUWg=)

#mail server SMTP
mailServer=smtps://smtp.mxhichina.com (enterprise mail)
mailServer=smtps://smtp.aliyun.com (person mail)

#mail Server port
mailPort=465
```



### mccomm 
record command to file

### mcenv 
env variable 

### mcmail 
for mail command log  
eg. 
```shell
# send mc.conf config file
mcmail file: subject recipient
# send special file
mcmail file:YOURFILE subject recipient
# send additional 
mcmail file:YOURFILE subject recipient accessnory
# send text
mcmail YOURMSG  subject recipient
# send file & additional
mcmail YOURFILE subject recipient accessnory
```
### mcpwd 
for mc.conf within mailPwd encrypt password  
eg.  
```shell
1. mcpwd -e YOURMAILPASSWORD
```


### mcuser
record user , ip , and ip relative addr

### mccert
generate certification file for CA , SSL , -G3

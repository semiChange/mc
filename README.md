# mc
monitor Linux  command or ssh operate  and mail report

### inst.sh
execute install mc  
NOTE: restart ssh  login after install mc

### config file
/etc/mc/mc.conf

### mccomm 
record command to file

### mcenv 
env variable 

### mcmail 
for mail command log  
eg. 
```shell
1. mcmail file:YOURFILE subject recipient
2. mcmail file:YOURFILE subject recipient accessnory
3. mcmail YOURMSG  subject recipient
4. mcmail YOURFILE subject recipient accessnory
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

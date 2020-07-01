bash  shell 解析 yml 格式配置文件

例如：/home/application.yml 内容如下
```
spring:
    datasource:
        password: 123456
        username: root
```
读取方式为spring.datasource.password
```
password=`getYmlValue /home/application.yml  spring.datasource.password`
echo $password
```


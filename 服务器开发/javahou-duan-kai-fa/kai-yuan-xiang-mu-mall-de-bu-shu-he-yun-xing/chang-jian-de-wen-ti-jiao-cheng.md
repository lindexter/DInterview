# 常见的问题教程

#### docker中elasticsearch启动不了
需要修改内存
```
find /var/lib/docker/ -name jvm.options
vim  /var/lib/docker/overlay2/5d20b562131d29a4a9860dd6c000a7f7914601f67e20f80320df8c5a88c318e7/diff/usr/share/elasticsearch/config/jvm.options

```
将##-Xms4g改成-Xms512m

elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v7.12.0/elasticsearch-analysis-ik-7.12.0.zip

#### Jenkins中添加远程服务器ssh凭证，记得使用密钥配置验证

#### 由于远程服务器需要开发2375端口，存在一定的安全隐患
http://www.macrozheng.com/#/reference/docker_protect_socket?id=%e5%ae%a2%e6%88%b7%e7%ab%af%e8%ae%bf%e9%97%ae



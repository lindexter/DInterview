# FastAdmin常用的命令

#### 一键生成后端Api的接口文档
```
php think api --force=true
```
>//一键生成API文档
php think api --force=true
//指定https://www.fastadmin.com为API接口请求域名,默认为空
php think api -u https://www.fastadmin.com --force=true
//输出自定义文件为myapi.html,默认为api.html
php think api -o myapi.html --force=true
//修改API模板为mytemplate.html，默认为index.html
php think api -e mytemplate.html --force=true
//修改标题为FastAdmin,作者为作者
php think api -t FastAdmin -a Karson --force=true
//查看API接口命令行帮助
php think api -h
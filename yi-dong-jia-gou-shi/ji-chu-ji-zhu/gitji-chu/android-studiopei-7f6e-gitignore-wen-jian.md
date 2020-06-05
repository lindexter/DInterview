# Android Studio配置.gitignore文件

## 语法

以斜杠“/”开头表示目录；

以星号“*”通配多个字符；

以问号“?”通配单个字符

以方括号“[]”包含单个字符的匹配列表；

以叹号“!”表示不忽略(跟踪)匹配到的文件或目录；

此外，git 对于 .ignore 配置文件是按行**从上到下**进行规则匹配的，意味着如果前面的规则匹配的范围更大，则后面的规则将不会生效

## 通用的配置文件
```xml
*.iml
.gradle
/local.properties
/.idea/workspace.xml
/.idea/libraries
.DS_Store
/build
/captures
```


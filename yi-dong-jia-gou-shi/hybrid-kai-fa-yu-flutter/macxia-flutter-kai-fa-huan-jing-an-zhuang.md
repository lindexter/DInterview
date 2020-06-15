# macOS下Flutter安装开发环境

## 配置Flutter国内镜像


打开.bash\_profile  
添加Flutter的国内镜像环境变量配置

```xml
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
```

![](/assets/移动架构师-Flutter-开发环境配置-1.png)

## 打开官网，下载Flutter的SDK

mac SDK下载地址：[https://flutter.dev/docs/get-started/install/macos](https://flutter.dev/docs/get-started/install/macos)

![](/assets/移动架构师-Flutter-开发环境配置-2.png)

## 配置SDK的环境变量

.bash\_profile中添加Flutter SDK环境变量
```xml
export FLUTTER_HOME=/Users/Dexter/Documents/codingTools/flutter/bin
export PATH=${PATH}:${FLUTTER_HOME}
```
![](/assets/移动架构师-Flutter-开发环境配置-4.png)

![](/assets/移动架构师-Flutter-开发环境配置-3.png)

>flutter doctor : 检测Flutter的本机环境依赖


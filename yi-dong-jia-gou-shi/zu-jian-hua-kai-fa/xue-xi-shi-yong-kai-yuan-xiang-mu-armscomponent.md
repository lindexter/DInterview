# 学习使用开源项目ArmsComponent

> [https://github.com/JessYanCoding/ArmsComponent](https://github.com/JessYanCoding/ArmsComponent)

### ArmsComponent组件化关于butterknife的不兼容解决
repositories中添加maven仓库
```groovy
//修复butterknife不兼容高版本gradle的依赖
maven { url "https://oss.sonatype.org/content/repositories/snapshots" }
```

```groovy
dependencies {
        classpath 'com.android.tools.build:gradle:3.4.2'
        classpath ('com.jakewharton:butterknife-gradle-plugin:10.1.1-SNAPSHOT') {
            exclude group: 'com.android.tools.build'
        }
//        classpath 'com.jakewharton:butterknife-gradle-plugin:10.1.0'
        //如果 ButterKnife 插件和其他插件发生冲突而报错请试试 v8.4.0 版本的 ButterKnife 插件, 注意 v8.4.0 最高只能支持 com.android.tools.build:gradle:3.0.1
//        classpath 'com.jakewharton:butterknife-gradle-plugin:8.4.0'
    }
```




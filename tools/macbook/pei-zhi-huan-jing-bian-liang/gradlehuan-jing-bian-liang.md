# gradle配置

> #### 什么是gradle

gradle 实际上是一个通用的构建工具。它不限于构建 Android 应用程序。

在 Gradle 的 GitHub 仓库中，它被描述为：构建工具，着重于构建自动化和支持多语言开发。如果您在任何平台上构建、测试、发布和部署软件，Gradle 提供了一个灵活的模型，可以支持从编译和打包代码到发布的整个开发生命周期。

> #### 环境变量配置

![](/assets/macbook-环境变量-gradle-4.png)

![](/assets/gradle-环境变量-gradle-5.png)

如果是zsh的shell工具，则需要在.zshrc中添加执行.bash\_profile，才能保证每次打开终端都初始化环境变量

![](/assets/macbook-环境变量-gradle-6.png)

> #### Android Studio的gradle配置

经常出现类似：

* 换个新电脑安装完Android Sutdio第一次打开一个工程巨慢
* 手动配置Gradle Home为什么总是无效?
* 明明已经下载了Gradle，配置了gradle home,为什么打开工程还是去自动下载Gradle?

一个android项目中，编译所用的gradle工具文件配置

distributionUrl 决定了这个项目使用的gradle版本![](/assets/macbook-环境变量-gradle-1.png)![](/assets/macbook-环境变量-gradle-2.png)


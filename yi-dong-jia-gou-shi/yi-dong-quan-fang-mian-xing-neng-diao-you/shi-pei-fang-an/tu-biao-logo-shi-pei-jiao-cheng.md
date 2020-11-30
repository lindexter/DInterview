# 图标logo适配教程

## 解决Android修改APP图标无效的问题

### 解释原因

从Android 8.0开始，应用图标分为了前景层和背景层。因此我们要将前景和背景分离，前景用来显示Logo，背景用来衬托。

![](/assets/import.png)

### 设置适配的logo图标
拖动Resize，调整至合适大小
点击Next，可能会提示会覆盖文件，继续Finish即可
![](/assets/移动架构师-移动全方面性能调优-适配方案-图标logo适配教程-2.png)
mipmap中的图标文件已被替换，并且做好了适配。
logo图标官方建议放在mipmap中

>教程来源：https://blog.csdn.net/y_universe/article/details/103273618

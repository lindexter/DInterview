# Xcode 添加复制行快捷键
> https://www.jianshu.com/p/d6b829b49bcd

# 修改权限
修改 Xcode 快捷键配置文件 IDETextKeyBindingSet.plist 权限
```
sudo chmod 666 /Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Resources/IDETextKeyBindingSet.plist
sudo chmod 777 /Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Resources/
```

# 增加快捷方式

打开 Xcode 快捷键配置文件 IDETextKeyBindingSet.plist
```
open /Applications/Xcode.app/Contents/Frameworks/IDEKit.framework/Resources/IDETextKeyBindingSet.plist
```

在 Insertions and Indentations 下添加键值对：key：
```
Duplicate Current Line
```
value：
```
selectLine:, copy:, moveToEndOfLine:, moveToBeginningOfLine:, paste:, moveBackward:
IDETextKeyBindingSet.plist
```

# 设置快捷键
重启 Xcode 让 IDETextKeyBindingSet.plist 配置生效
打开 Xcode -> Preferences -> Key Bindings ，搜索找到 Duplicate Current Line
设置自己喜欢的快捷键：Command + D（若有冲突可以删除冲突快捷键即可）
Key Bindings
复制行：Command + D
删除行：Command + Delete
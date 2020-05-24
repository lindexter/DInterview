# 注解与反射

## 注解的保留级别和作用域
|保留级别| 标签|使用技术|  说明  |
| :-- | :-- | :-- |:----: |
|源码 |SOURCE|APT技术 |编译期获取成员信息，生成额外的辅助类|
|字节码| CLASS|字节码增强 |修改编译后生成的class的代码逻辑，热修复技术等|
|运行时| RUNNINGTIME| 反射|IOC，反射技术|
示例：
```java
@Retention(CLASS)
@Target({METHOD, PARAMETER, FIELD, LOCAL_VARIABLE})
public @interface DrawableRes {
}
```




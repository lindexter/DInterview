# 注解与反射

## 注解的保留级别和作用域
|保留级别|   |   |
| :--: | :--: | :------: |
|源码 |SOURCE| |
|字节码| CLASS| |
|运行时| RUNNINGTIME| |
示例：
```java
@Retention(CLASS)
@Target({METHOD, PARAMETER, FIELD, LOCAL_VARIABLE})
public @interface DrawableRes {
}
```




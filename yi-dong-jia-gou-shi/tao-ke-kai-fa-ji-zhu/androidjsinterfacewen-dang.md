# AndroidJSInterface接口文档

### 1、显示Toast的消息

##### URL

window.NativeView.showMessage\(String message\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| message | ture | string | 显示的toast消息 |

### 2、复制文本到剪贴板

##### URL

window.NativeView.copyShareDocument\(String text\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| text | ture | string | 需要复制的文本 |

### 3、保存图片

##### URL

window.NativeView.savePicture\(String\[\] picUrls\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| picUrls | ture | string数组 | 保存图片的url |

### 4、微信好友分享网页地址

##### URL

window.NativeView.weChatShare\(String webUrl\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| webUrl | ture | string | 需要分享的网页url |

### 5、微信朋友圈分享网页地址

##### URL

window.NativeView.weChatFriendShare\(String webUrl\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| webUrl | ture | string | 需要分享的网页url |

### 6、微信登录

##### URL

window.NativeView.loginByWechat\(\)

### 7、webview页面加载成功回调

##### URL

window.NativeView.onPageLoading\(boolean isSuccess\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| isSuccess | ture | boolean | 是否加载成功 |

### 8、webview获取Apk的版本号

##### URL

window.NativeView.appVersion\(\)

#### 回调接口

```
javascript:appVersionCallback(versionCode)
```

### 9、清除webview的缓存\(有提示信息\)

##### URL

window.NativeView.clearCache\(\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| isSuccess | ture | boolean | 是否清除成功 |

### 10、清除webview的缓存

##### URL

window.NativeView.clearCache\(boolean isHideToast\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| isHideToast | ture | boolean | 是否隐藏提示信息 |

### 11、校验是否有新版本的APP

##### URL

window.NativeView.checkAppUpdate\(\)

### 12、判断是否是网页的首页

##### URL

window.NativeView.setIsHomeTab\(boolean isHomeTab\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| isHomeTab | ture | boolean | 设置该参数可控制判断是否可以android手机返回键返回网页 |

### 13、获取手机的通用信息

##### URL

window.NativeView.getSystemInfo\(\)

##### 回调

```
"javascript:systemInfoResult('" + PhoneInfoBean.getPhoneInfoString() + "')"
```
##### 回调JSON参数
| 参数 | 类型 | 说明 |
| :--- | :--- | --- |
| model | String | 手机型号 |
| version | String | 系统版本 |
| linuxCore | String | Linux内核 |
| androidId  | String | ANDROID_ID |
| deviceId  | String | 设备Id |
| serial | String | 序列号(Android10以上无权限获取) |
| imei  | String | IMEI(Android10以上无权限获取) |
| imsi  | String | IMSI(Android10以上无权限获取) |
| meid | String | MEID(Android10以上无权限获取) |
| isPhone  | boolean | 是否是手机 |
| isSimCardReady | boolean | 判断sim卡是否准备好 |
| simOperatorName | String | 获取sim卡运营商名称 |
| simOperatorByMnc | String | 获取sim卡运营商名称 |

>https://developer.android.com/training/articles/user-data-ids

### 14、隐藏手机软键盘

##### URL

window.NativeView.hideKeyboard\(\)

### 15、显示手机软键盘

##### URL

window.NativeView.showKeyboard\(\)

### 16、保存数据到轻缓存中\(只能存string\)

##### URL

window.NativeView.saveSP\(String key,String value\)

#### 请求参数

| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| key | ture | String | 键 |
| value | ture | String | 值 |

### 17、从轻缓存中获取数据\(只能取string\)
##### URL
window.NativeView.getSP\(String key\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| key | ture | String | 键 |
#### 回调接口
```java
javascript:getSharedPreferences('" + key + "," + value) + "')"
```

### 18、根据URL保存成图片二维码
##### URL
window.NativeView.saveQRcode\(String qrUrl\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| qrUrl | ture | String | 需要保存的url |

### 19、获取渠道标识字符串\(只能取string\)
##### URL
window.NativeView.getChannel\(\)
#### 回调接口
```java
javascript:getChannelResult('" + channel + "')"
```

### 20、获取手机的型号和系统版本
##### URL
window.NativeView.appMessage\(\)
#### 回调接口
```java
javascript:appMessageCallback('" + model + " " + version + "')"
```

### 21、DMS行为上报接口一
##### URL
window.NativeView.logAction\(String actionType\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | :--- |
| actionType | ture | String | 行为类型 |
>行为类型，分为两类，一类是在DMP上定义的标准行为类型，具体见com.qq.gdt.action.ActionType类；另一类是您自己自定义的行为类型，可以传入一个字符串类型的参数，要求：这个字符串只能包含字母、数字和下划线，必须以字母开头，长度不能超过64
详细参数见附录
https://developers.e.qq.com/docs/guide/user_actions/sdk
>public static final String START_APP = "START_APP";
    public static final String PAGE_VIEW = "PAGE_VIEW";
    public static final String REGISTER = "REGISTER";
    public static final String VIEW_CONTENT = "VIEW_CONTENT";
    public static final String CONSULT = "CONSULT";
    public static final String ADD_TO_CART = "ADD_TO_CART";
    public static final String PURCHASE = "PURCHASE";
    public static final String SEARCH = "SEARCH";
    public static final String ADD_TO_WISHLIST = "ADD_TO_WISHLIST";
    public static final String INITIATE_CHECKOUT = "INITIATE_CHECKOUT";
    public static final String COMPLETE_ORDER = "COMPLETE_ORDER";
    public static final String DOWNLOAD_APP = "DOWNLOAD_APP";
    public static final String RATE = "RATE";
    public static final String RESERVATION = "RESERVATION";
    public static final String SHARE = "SHARE";
    public static final String APPLY = "APPLY";
    public static final String CLAIM_OFFER = "CLAIM_OFFER";
    public static final String NAVIGATE = "NAVIGATE";
    public static final String PRODUCT_RECOMMEND = "PRODUCT_RECOMMEND";

### 22、DMS行为上报接口二
##### URL
window.NativeView.logAction\(String actionType, String key, String value\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | :--- |
| actionType | ture | String | 行为类型 |
| key | ture | String | 单个行为参数的key |
| key | ture | String | 单个行为参数的value |

### 22、DMS行为上报接口三
##### URL
window.NativeView.logAction\(String actionType, String actionParam\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | :--- |
| actionType | ture | String | 行为类型 |
| actionParam | ture | JsonString | 行为参数json字符串 |

### 23、DMS设置用户软ID
##### URL
window.NativeView.setUserUniqueId\(String userUniqueId\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| userUniqueId | ture | String | 用户软ID |

### 24、DMS执行预设置的action方法
##### URL
window.NativeView.doActionUtilsMethods\(String methods,Object[] params\)
#### 请求参数
| 参数 | 必选 | 类型 | 说明 |
| :--- | :--- | :--- | --- |
| methods | ture | String | 执行的方法名 |
| params | ture | 数组 | 执行的方法参数只允许传字符串和布尔值 |

>methods详细参数参考
>





















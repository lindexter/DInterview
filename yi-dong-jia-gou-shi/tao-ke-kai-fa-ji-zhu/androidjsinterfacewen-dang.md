# AndroidJSInterface接口文档
-----------

### 1、显示Toast的消息
##### URL
window.NativeView.showMessage(String message)
#### 请求参数

|参数|必选|类型|说明|
|:----- |:-------|:-----|----- |
|message |ture |string|显示的toast消息 |

### 2、复制文本到剪贴板
##### URL
window.NativeView.copyShareDocument(String text)
#### 请求参数

|参数|必选|类型|说明|
|:----- |:-------|:-----|----- |
|text |ture |string|需要复制的文本 |

### 3、保存图片
##### URL
window.NativeView.savePicture(String[] picUrls)
#### 请求参数

|参数|必选|类型|说明|
|:----- |:-------|:-----|----- |
|picUrls |ture |string数组|保存图片的url |



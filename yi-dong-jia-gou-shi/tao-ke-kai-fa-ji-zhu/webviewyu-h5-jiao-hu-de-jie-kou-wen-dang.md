# 在H5Platform平台上快速配置Module

1. 复制Module，重命名Module名字，删除iml文件

2. settings.gradle中include新的module

3. 修改包名和Application，包括androidTest和Test的包名

4. 修改manifest里的package和activity的路径

5. 修改bulid.gradle[Module]的applicationId和App名称

6. 修改String.xml中的APP名称

7. 删掉MainActivity和LaunchActivity中的R文件的import包，导入新的R文件

8. 修改基础包app中BuildConfig导入

9. 修改微信依赖包的R文件依赖


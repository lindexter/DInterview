# 在H5Platform平台上快速配置Module

1. 复制Module，重命名Module名字，删除iml文件

2. settings.gradle中include新的module

3. 修改包名和Application，包括androidTest和Test的包名\(Rename directory,去掉打勾Search in comments and strings\)

4. 修改manifest里的package和BizUtils的路径

5. 修改bulid.gradle\[Module\]的applicationId、App名称和BASE\_URL

6. 修改icon和loading页图片

7. 国际化的APP需要在manifest中添加静默下载的service

8. 重新签名




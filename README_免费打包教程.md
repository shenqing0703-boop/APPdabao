# 寰亚直播 免费无广告 APK 打包教程

这个项目用于把网站 https://671.lol/?app=1 打包成 Android APK。

## 使用方法

1. 登录 GitHub。
2. 新建一个仓库，建议选 Private。
3. 上传本项目解压后的所有文件。
4. 打开仓库页面上方 Actions。
5. 点击左侧 Build Android APK。
6. 点击 Run workflow。
7. 等待 3-8 分钟。
8. 打包完成后进入最新任务。
9. 页面底部 Artifacts 下载 huanya-live-apk。
10. 解压后得到 app-debug.apk。
11. 改名为 app.apk，上传到你的下载页。

## 修改网址

文件：app/src/main/java/com/huanya/live/MainActivity.java

修改：
private static final String HOME_URL = "https://671.lol/?app=1";

## 修改应用名称

文件：app/src/main/res/values/strings.xml

修改：
<string name="app_name">寰亚直播</string>

## 注意

这是 debug 签名 APK，适合先测试和小范围分发。
以后正式长期运营，建议改成 release 签名，方便用户覆盖升级。

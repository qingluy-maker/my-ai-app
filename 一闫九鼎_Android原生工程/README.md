# 一闫九鼎 - 安卓原生独立 APP 工程源码

这是一个已配置好的 Android Studio 原生工程，包含：
- 自定义应用图标与「一闫九鼎」应用名称
- 沉浸式全屏 WebView 容器（无浏览器顶栏）
- 自动对接安卓系统 DownloadManager，下载视频或图集直接存入相册/下载目录
- 相册读写权限与剪贴板权限预置

## 如何生成独立 APK 文件：

### 方法 1：使用 Android Studio（最简单）
1. 下载并解压本项目 ZIP
2. 打开 Android Studio，选择 **File -> Open**，选中解压出的工程根目录
3. 等待 Gradle 自动同步完成
4. 点击顶部菜单栏 **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**
5. 构建完成后，右下角弹窗点击 **locate**，即可得到生成的 **app-debug.apk** 安装包！
6. 将该 .apk 发送给手机直接安装即可使用。

### 方法 2：使用命令行快速打包
```bash
./gradlew assembleDebug
# 输出文件路径：app/build/outputs/apk/debug/app-debug.apk
```

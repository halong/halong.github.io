### Windows搭建flutter在Android Studio开发环境

- 安装Flutter：到 https://flutter.io/docs/ 下载Flutter SDK压缩包并解压

- 配置系统环境：右击计算机->属性->高级系统设置->环境变量->新建变量：PUB_HOSTED_URL=https://pub.flutter-io.cn    FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn   
  Path追加flutter的解压路径/bin  
  可以运行cmd  flutter -v检测是否配置成功

- 在Android Studio安装flutter和 Dart插件：file->Settings->Plugins->MarketPlace分别搜索flutter和Dart并安装 重启 

- 新建flutter项目：file->new -> new Flutter Project

- flutter项目运行原理： 以android/ios文件夹里的原生代码为程序入口，接入lib文件夹的dart文件作为程序主体，从而实现一套代码编译出android/ios两个平台app

- 如何编写flutter项目： 只需要编写lib文件夹里的dart文件就行了，其中main.dart为入口。另外，第三方依赖添加到pubspec.yaml文件中的dependencies下面。

### Mac搭建flutter开发环境

- 安装Flutter：到 https://flutter.dev/docs/development/tools/sdk/archive?tab=macos#macos下载Flutter SDK压缩包并解压

- 配置系统环境：在终端输入 vim ~/.bash_profile 新建或打开配置文件；按下i进入Insert编辑模式；输入 export PATH=~/flutter/bin:$PATH 将flutter文件路径追加到PATH，用：隔开；增加一行 export PUB_HOSTED_URL=https://pub.flutter-io.cn 再增加一行 export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn  按下Esc键退出编辑模式，输入:wq 命令退出并保存；输入 source ~/.bash_profile刷新当前终端窗口；输入 echo $PATH 查看PATH；

- Xcode安装flutter和 Dart插件：进入终端输入brew install --HEAD libimobiledevice
  brew install ideviceinstaller
  brew install ios-deploy
  brew install cocoapods
  pod setup

### VS Code开发Flutter

- 安装Flutter和 Dart插件：View->Command Palette->分别搜索Dart和Flutter并安装

- 新建Flutter项目：View->Command Palette->输入flutter:new Project
### flutter在Android Studio环境搭建

- 下载flutter-sdk:到https://github.com/flutter/flutter将代码克隆到本地。

- 在Android Studio安装Flutter插件：file->Settings->Plugins->MarketPlace搜索flutter

- 解决flutter-sdk下载依赖问题：打开flutter\packages\flutter_tools\gradle\flutter.gradle 在repositories里添加：

···     

      maven{
            url 'https://maven.aliyun.com/repository/jcenter'
          }
		  
	  maven{
             url 'https://maven.aliyun.com/repository/google'
          }
		  
      maven{
            url 'http://maven.aliyun.com/nexus/content/groups/public'
          }
···
    

### 在Vs Code上编译
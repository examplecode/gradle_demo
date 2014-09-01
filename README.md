# 演示Gradle 的用法

## 目录结构

1. hello-apk 传统的eclipse 项目
2. hello-apk-with-gradle 从传统的eclipse项目拷贝而来 使用gradle脚本构建的项目。



## hello-apk-with-gradle 构建脚本演示

* build.gradle 默认构建脚本
* build.gradle-simple 最简单的构建脚本
* build.gradle-proguard 使用proguard
* build.gradle-new-package 同时创建新的包名


使用构建脚本进行构建，执行命令如下：

    gradle build -b build.gradle-simple



## 其他

### realse 包需要的自签名文件

    $ keytool -genkey -v -keystore examplecode.keystore -alias examplecode -keyalg RSA -keysize 2048 -validity 100000



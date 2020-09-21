# MyCacher

### 依赖snapshot版本
1、配置Maven仓库地址，在工程根目录的build.gradle中配置：
maven {
    url "https://oss.sonatype.org/content/repositories/snapshots"
}

2、module目录下的build.gradle中添加依赖如下依赖：   
  com.tencent.iot.hub:hub-device-java:1.0.1-SNAPSHOT

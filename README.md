# MyCacher

### gradle 依赖snapshot
1、配置Maven仓库地址，在工程根目录的build.gradle中配置url("https://oss.sonatype.org/content/repositories/snapshots")
```
allprojects {
    repositories {
        google()
        jcenter()
        maven {
            url "https://oss.sonatype.org/content/repositories/snapshots"
        }
    }
}
```

2、module目录下的build.gradle中添加依赖如下依赖
```
dependencies {
    ...
    implementation 'com.tencent.iot.hub:hub-device-java:1.0.1-SNAPSHOT'
}
```

### maven 依赖snapshot
```
<dependencies>
    <dependency>
        <groupId>com.tencent.iot.hub</groupId>
        <artifactId>hub-device-java</artifactId>
        <version>1.0.1-SNAPSHOT</version>
    </dependency>
</dependencies>
<repositories>
    <repository>
        <id>snapshots</id>
        <url>https://oss.sonatype.org/content/repositories/snapshots</url>
    </repository>
</repositories>
```

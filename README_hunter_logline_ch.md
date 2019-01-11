# LogLine-Plugin

这个插件会为你每行日志添加行号，可以帮你更快定位日志，尤其有时候你在一个Java文件中不同地方，打印了一样的日志。

## 快速引入

在build.gradle中添加以下依赖

```groovy

dependencies {
    implementation 'com.quinn.hunter:hunter-linelog-library:0.8.5'
}

repositories {
    jcenter()
}

buildscript {
    repositories {
        jcenter()
        google()
    }
    dependencies {
        classpath 'com.quinn.hunter:hunter-linelog-plugin:0.9.1'
    }
}

apply plugin: 'hunter-linelog'
    
```



未使用这个插件时打印的日志

```java

I/MainActivity: onCreate

```
使用插件后的日志

```java

I/MainActivity[21]: onCreate

```  
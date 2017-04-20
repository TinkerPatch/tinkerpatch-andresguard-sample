# tinkerpatch-andresguard-sample

[ ![Download](https://api.bintray.com/packages/simsun/maven/tinkerpatch-android-sdk/images/download.svg) ](https://bintray.com/simsun/maven/tinkerpatch-android-sdk/_latestVersion)
[![Join Slack](https://slack.tinkerpatch.com/badge.svg)](https://slack.tinkerpatch.com)

集成[AndResGuard](https://github.com/shwenzhang/AndResGuard)的例子。

只需copy`andresguard.gradle`到你的工程中，并在`tinkerpatch.gradle`文件中增加如下代码:
```gradle
/**
 * 引入 AndResGuard的相关配置
 */
project.ext {
    TP_BAKPATH = bakPath
    TP_BASEINFO = baseInfo
    TP_VARIANTNAME = variantName
}
apply from: 'andresguard.gradle'
```

如果你开启资源混淆，备份文件夹中会多出`*-resource_mapping.txt`和`-andresguard.apk`文件。带有后缀`-andresguard`为资源混淆过的安装包。

[更多集成文档](http://tinkerpatch.com/Docs/intro)

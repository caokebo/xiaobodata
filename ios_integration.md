# iOS

SDK适用于 iOS7.0 及以上的系统    

> **导入SDK**

请按照以下步骤将SDK导入到您的项目中：

 1. 解压 iOS SDK 压缩文件。

 2. 添加 ```MobAnalyticsSDK-WaveletData.a``` 和 ```MobAnalytics.h```到您的iOS工程中。

 提醒: 勾选 ```Copy items if needed```


> **配置AndroidManifest.xml**

| **库名称** | **说明** |
| -- | -- |
| Foundation.framework	 | 基础依赖库|
| Security.framework	 | 用于APP连接圈选页面SSL连接|
| CoreTelephony.framework| 用于读取运营商名称|
| SystemConfiguration.framework| 用于检测网络状况|
| SystemConfiguration.framework| 用于判断网络状态|

提醒: 添加项目依赖库的位置在 项目设置```target``` -> 选项卡```General``` -> ```Linked Frameworks and Libraries```
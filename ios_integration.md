# iOS

SDK适用于 iOS7.0 及以上的系统    

> **导入SDK**

请按照以下步骤将SDK导入到您的项目中：

 1. 解压 iOS SDK 压缩文件。

 2. 添加 ```MobAnalyticsSDK-WaveletData.a``` 和 ```MobAnalytics.h```到您的iOS工程中。

 提醒:勾选 ```Copy items if needed```


> **配置AndroidManifest.xml**

| 权限 | 权限描述 |

| -- | -- |

| ACCESS_NETWORK_STATE| 允许应用检测网络连接状态，当网络关闭或者异常时，不发送数据。 |

| READ_PHONE_STATE| 允许应用读取手机信息，用户获取deviceID，作为用户的唯一标识。 |

| ACCESS_WIFI_STATE| 当获取不到deviceID(设备为wifi版)时获取MCA地址，作为用户的唯一标识。 |

| INTERNET| 允许应用访问互联网，用于用户数据的上传。 |

| ACCESS_FINE_LOCATION| 可通过GPS获取设备的位置信息，用来修正用户的地域分布数据，使报表数据更准确。。 |


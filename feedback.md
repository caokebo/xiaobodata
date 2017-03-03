# 摇一摇反馈

> 功能说明


摇一摇反馈是提供给使用者反馈问题的一个功能，能帮助开发人员快速定位应用中出现的问题并解决，提高应用稳定性和用户体验。摇一摇反馈我们提供了大量的可定制化方法，让反馈界面完美融入应用中。


{% method -%}
{% sample lang="Android" -%}

摇一摇反馈功能默认开启。但是要在`AndroidManifest.xml`配置XBFeedbackActivity，才能使用该功能。



```
<manifest……>
   <application ……>
   ……
     <!--可选-->
     <activity android:name="com.xiaobodata.mobileanalytics.activity.XBFeedbackActivity"/>
   </application>
</manifest>
```
下图是默认摇一摇反馈图

![](/assets/feedback_dialog_hint.png)             ![](/assets/feedback_activity.png)

> **功能设置**

* 应用里有显示摇一摇反馈的开关按钮:

  设置摇一摇反馈功能是否激活(在有激活开关的activity中使用，使当前activity也可以摇一摇反馈)
```
VmaAgent.setFeedbackEnabled(boolean isFeedbackEnabled, Activity activity)
```

  设置摇一摇反馈功能关闭监听(在有激活开关的activity中使用，监听摇一摇反馈关闭状态，用于设置激活开关为关闭)
```
VmaAgent.setOnCloseFeedbackListener(OnCloseFeedbackListener onCloseFeedbackListener)
```
  获取摇一摇反馈是否激活(在有激活开关的activity中使用,设置激活开关状态）
```
VmaAgent.getFeedbackEnabled()
```
  设置摇一摇dialog风格(在有激活开关时使用)，是否有关闭按钮， 默认为flase
```
VmaAgent.setFeedbackDialogHasClose(boolean hasClose)
```
下图为有关闭按钮的提示框

 ![](/assets/feedback_dialog_hint1.png)
  
 注意事项：
   1. 建议有激活摇一摇反馈开关按钮的时候使用上面方法。
   2. 提示框style使用android.app.AlertDialog,会随着android版本不同而不同。

   

* 定制化反馈界面:

 设置反馈界面状态栏沉浸式,默认为true
```
VmaAgent.setFeedbackBarImmersive(boolean isImmersive)
```
设置状态栏沉浸式颜色,默认为默认标题的背景色(默认色值为#2E2D2D)
```
VmaAgent.setFeedbackBarBackgroundColor(String Color)
```
设置反馈界面标题背景色(默认色值为#2E2D2D)
```
VmaAgent.setFeedbackTitleBackgroundColor(String Color)
```
设置反馈界面标题颜色(默认色值为#FFFFFF)
```
VmaAgent.setFeedbackTitleColor(String Color)
```
设置反馈界面标题左右文字颜色(默认色值为#FFFFFF)
```
VmaAgent.setFeedbackTitleRLColor(String Color)
```
设置反馈界面标题左右文字按下颜色(默认色值为#383737)
```
VmaAgent.setFeedbackTitlePressedColor(String Color)
```
设置反馈界面底部tab背景颜色(默认色值为#2E2D2D)
```
VmaAgent.setFeedbackTabBottomBackgroundColor(String Color)
```
设置反馈界面底部tab按钮按下颜色(默认色值为#383737)
```
VmaAgent.setFeedbackTabBottomPressedColor(String Color)
```
设置反馈界面底部颜色选择器背景颜色(默认色值为#272828)
```
VmaAgent.setFeedbackPickViewBackgroundColor(String Color)
```
* 通用功能:
 
 设置摇一摇反馈功能是否激活
```
VmaAgent.setFeedbackEnabled(boolean isFeedbackEnabled)
```
设置摇一摇反馈灵敏度(默认为1100，900-2000之间)
```
VmaAgent.setFeedbackShakingThreshold(int shakingThreshold)
```


{% sample lang="iOS" -%}
```java
iOS描述

```
{% endmethod %}





\# 摇一摇反馈

> 功能说明


摇一摇反馈是提供给使用者反馈问题的一个功能，能帮助开发人员快速定位应用中出现的问题并解决，提高应用稳定性和用户体验。摇一摇反馈我们提供了大量的可定制化方法，让反馈界面完美融入应用中。


{% method -%}
{% sample lang="Android" -%}
```java
//设置摇一摇反馈功能是否激活
VmaAgent.setFeedbackEnabled(boolean isFeedbackEnabled)   
//设置摇一摇反馈功能是否激活(在有激活开关的activity中使用)
VmaAgent.setFeedbackEnabled(boolean isFeedbackEnabled, Activity activity) 
//设置摇一摇反馈功能关闭监听
VmaAgent.setOnCloseFeedbackListener(OnCloseFeedbackListener onCloseFeedbackListener)
//设置状态栏沉浸式,默认为true
VmaAgent.setFeedbackBarImmersive(boolean isImmersive)
//设置状态栏沉浸式颜色,默认为默认title的背景色
VmaAgent.setFeedbackBarBackgroundColor(String Color)
//设置反馈界面标题背景色
VmaAgent.setFeedbackTitleBackgroundColor(String Color)
//设置反馈界面标题颜色
VmaAgent.setFeedbackTitleColor(String Color)
//设置反馈界面标题左右文字颜色
VmaAgent.setFeedbackTitleRLColor(String Color)
//设置反馈界面标题左右文字按下颜色
VmaAgent.setFeedbackTitlePressedColor(String Color)
//设置反馈界面底部tab背景颜色
VmaAgent.setFeedbackTabBottomBackgroundColor(String Color)
//设置反馈界面底部tab按钮按下颜色
VmaAgent.setFeedbackTabBottomPressedColor(String Color)
//设置反馈界面底部颜色选择器背景颜色
VmaAgent.setFeedbackPickViewBackgroundColor(String Color)
//获取摇一摇反馈是否激活
VmaAgent.getFeedbackEnabled()
//设置摇一摇反馈灵敏度(默认为1100，900-2000之间)
VmaAgent.setFeedbackShakingThreshold(int shakingThreshold)
//设置摇一摇dialog是否有关闭按钮 默认为flase
VmaAgent.setFeedbackDialogHasClose(boolean hasClose)

```

{% sample lang="iOS" -%}
```java
iOS描述

```
{% endmethod %}





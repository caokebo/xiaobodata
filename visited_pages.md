# 访问页面


> **功能说明**


此功能可帮助开发者统计应用中各个页面的访问次数、平均停留时长和页面跳出率，为产品优化提供依据。


> **功能集成**

{% method -%}

{% sample lang="Android" -%}
* 进入页面的时候调用(在要统计的页面 onResume()里):

```java
VmaAgent.onResume(Context context,String pageName)
```
* 退出页面的时候调用(在要统计的页面 onPause()里):

```java
VmaAgent.onPause(Context context)
```
注意事项：

1. onResume和onPause要成对出现；
2. pageName不能相同;
3. 如果页面是fragment，那么不要再依赖的activity添加以上代码(避免重复统计)，直接在要统计的fragment的`onResume()`里调用`VmaAgent.onPageStart(String pageName)`,`onPause()`里调用`VmaAgent.onPageEnd(String pageName)`。


{% sample lang="iOS" -%}
Here is how to print a message to `stdout` using iOS.

```
fmt.Println("My first method")
```
{% endmethod %}
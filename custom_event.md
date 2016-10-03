# 自定义事件


> **功能说明**

自定义事件用于统计任何您期望去跟踪的数据，如：用户点击某功能按钮、填写某个输入框、触发了某个广告等。

自定义事件有2种集成方式：

1. 有痕埋点;
2. 无痕埋点。


* **有痕埋点**

有痕埋点是指在App中以触发代码方式来记录自定义数据追踪点的实现方式。

EventId无需提前在数据平台中定义，可自行定义名称，直接加入到应用中需要跟踪的位置即可生效。

有痕埋点除了记录行为，还支持添加一些描述行为的参数，使用多对Key-Value的方式对事件发生时的状况做详尽记录。参数非必须使用，使用时每个有痕埋点下没有事件参数限制。

* **无痕埋点**

无痕埋点支持App界面中的按钮、输入框、单选和多选控件、图片按钮等的点击动作自动计数。您不需要书写额外的触发代码，在报表平台中通过动态添加，SDK会自动部署追踪码。


{% method -%}

{% sample lang="Android" -%}

* 在你需要添加事件的地方加上如下代码：

```java
VmaAgent.onEvent(Context context, String event_id);
```

例：用户点击登陆按钮(登录事件id为后台添加的事件id)

```@Override
public void onClick(View v) {
VmaAgent.onEvent(LoginActivity.this, "登录事件id");
}```

* 如果你需要事件的其他信息，你可以这样添加代码：

```
VmaAgent.onEvent(Context context, String event_id,HashMap<String, String> map);
```

例：用户点击欧洲杯投注按钮(投注事件id为后台添加的事件id)

```@Override
public void onClick(View v) {
HashMap<String,String> map = new HashMap<String,String>();      
map.put("team","英国 VS 法国");
VmaAgent.onEvent(this, "投注事件id",map);
}```

{% sample lang="iOS" -%}

```go
fmt.Println("My first method")
```
{% endmethod %}




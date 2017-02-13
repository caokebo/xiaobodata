# HTML5

> **适用范围**

网站统计监控利器，支持PC、移动端数据收集。

> **跟踪原理介绍**

使用小波数据网站统计跟踪网站的流量，您需要在网站的每一个网页中加入小波数据的JavaScript代码。统计代码在创建站点时获取，一个站点对应一个代码跟踪ID。

当用户浏览您网站的某一个页面时，这段JavaScript代码会被执行，将所收集到的访问参数发送到小波数据的服务器，小波数据根据跟踪ID对数据进行归类处理，然后展示到相应ID的站点统计报告里。正确安装统计代码后，一般60分钟左右后，即可以查看到统计数据。因此要想统计到完整的访问流量，必须在网站的每一个页面中都安装正确ID的统计代码。


> **代码类型**

异步分析代码：此代码以异步加载形式进行加载，可以真正做到对网站打开速度完全没有影响，使用该代码能够大幅提升网站的打开速度，也可提升统计数据的准确性。不管是PC站点还是移动站点，小波数据都支持。

```

 <script type="text/javascript">
 var _xbd = _xbd || [];
 _xbd.push(['trackPageView']);

 (function() {
     var g = document.createElement("script");
     g.src = "http://xiaobodata.com/xb.js?XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX";
     g.type='text/javascript'; g.async=true; g.defer=true;
     var s = document.getElementsByTagName('script')[0];
     s.parentNode.insertBefore(g,s);
 })(); 
</script>


```


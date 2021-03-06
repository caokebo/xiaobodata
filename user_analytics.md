# 用户分析

> **新增用户**

首次联网启动应用的设备视为一个新增用户，以IMEI/OpenUDID标识用户的唯一性。

统计指标定义：

* 新增用户：新增加的应用使用者（按设备），重安装应用不会重复计量。

* 新增用户占比：某段时间内新增用户占所选时间段总新增用户的比例。

![](/assets/new_user.png)

在新增用户明细列表中，点击【详情】按钮，可以查看其对应的新增用户明细，包括：账号、设备标识、系统、机型、运营商、省市以及日期等信息。
![](/assets/用户分析4.png)

![](/assets/new_user_detail.png)


> **活跃用户**

所选时间段内，启动过应用的用户(去重)，启动过一次的用户即被视为活跃用户，包括新用户和老用户。

针对活跃用户的分析包括活跃用户趋势和活跃用户明细两个部分。

统计指标定义：

* 活跃用户：启动过应用的用户（去重），启动过一次的用户即视为活跃用户，包括新用户与老用户。

* 活跃用户占比：某段时间内活跃用户占所选时间段总活跃用户的比例。

![](/assets/active_user.png)

在活跃用户明细列表中，点击【详情】按钮，可以查看其对应的活跃用户明细，包括：账号、设备标识、系统、机型、运营商、省市以及日期等信息。

![](/assets/active_user_detail.png)


> **启动次数**

针对启动次数的分析，包括启动次数趋势和启动次数明细两个部分。

统计指标定义：

* 启动次数：Android启动定义：打开应用即为启动。应用完全退出或者在后台运行超过30s（默认30s）后再被打开，算为一次新启动。iOS启动定义：打开应用即为启动。应用完全退出或者在后台运行后再被打开，算为一次新启动。

* 启动次数占比：某段时间内启动次数占所选时间段总启动次数的比例。

![](/assets/launch.png)


> **版本分布**

针对版本分布的分析，包括TOP10版本趋势和版本分布明细两部分。

TOP10版本趋势，分别从新增用户、活跃用户、启动次数三个维度，展示了累计用户排名前10的各版本变化趋势，可以帮助您了解每个版本的用户新增，最新版本的升级情况，目前最活跃的是哪些版本等。

统计指标定义：

* 新增用户：新增加的应用使用者（按设备），重安装应用不会重复计量。

* 活跃用户：启动过应用的用户（去重），启动过一次的用户即视为活跃用户，包括新用户与老用户。

* 启动次数：打开应用即视为启动，完全退出或退至后台即视为启动结束。

![](/assets/version_user.png)

页面中按照应用版本倒序展示版本分布情况，包括：应用版本、截至今日版本累计用户（%）、新增用户、升级用户、新增+升级、活跃用户、启动次数及操作。

![](/assets/version_user_detail.png)

统计指标定义：

* 版本累计用户（%）：截至到现在，该版本的累计用户（占累计用户全体的比例）。

* 新增用户：新增加的应用使用者（按设备），重安装应用不会重复计量。

* 升级用户：从其他版本升级到该版本的用户（以设备为判断标准）。

* 活跃用户：启动过应用的用户（去重），启动过一次的用户即视为活跃用户，包括新用户与老用户。

* 启动次数：打开应用即视为启动，完全退出或退至后台即视为启动结束。























# 篮球API接口


## 1、篮球比赛
### 1.1、基础接口
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球赛事列表|	GET| /api/sports/basketball/matchevent/list	| GK数据|	2018-07-05 17:38:47|
|篮球球队列表|	GET| /api/sports/basketball/team/list|	 GK数据|	2019-02-26 16:51:10|
|篮球删除比赛|	GET| /api/sports/basketball/match/deleted_ids|	 GK数据|	2019-03-14 10:15:42|

### 1.2、即时数据
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球实时统计|	GET| /api/sports/basketball/match/detail_live|	 GK数据|	2019-04-18 19:28:41|
|篮球赛程赛果|	GET| /api/sports/basketball/match/list|	 GK数据|	2019-04-19 11:57:25|
|篮球即时比分|	GET| /api/sports/basketball/match/live|	 GK数据|	2019-04-11 18:33:56|

### 1.3、赛事分析
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球比赛详情|	GET| /api/sports/basketball/match/detail|	 GK数据|	2019-04-19 15:24:28|
|篮球分析数据|	GET| /api/sports/basketball/match/analysis|	 GK数据|	2019-04-19 16:33:30|

### 1.4、即时指数
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球实时指数|	GET| /api/sports/basketball/odds/live_history|	 GK数据	|2019-01-24 10:45:46|
|单场指数历史|	GET| /api/sports/basketball/odds/history|	 GK数据	|2019-04-10 11:51:48|


### 1.5、情报分析
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球比赛情报|	GET| /api/sports/basketball/match/intelligence|	 GK数据|	2018-09-11 11:01:22|
### 1.6、动画直播
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球动画直播	|GET| mlive|	 GK数据|	2018-06-07 10:29:38|


### 1.7、资料库
| 接口名称 [7] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|赛季列表|	GET| /api/v2/sports/basketball/season/list|	 GK数据|	2019-02-21 17:33:47|
|赛季赛程|	GET| /api/v2/sports/basketball/season/matches|	 GK数据|	2019-04-19 15:25:50|
|赛季球队统计|	GET| /api/v2/sports/basketball/season/teams_stats|	 GK数据|	2019-04-19 15:26:17|
|赛季积分榜|	GET| /api/v2/sports/basketball/season/tables|	 GK数据|	2019-04-19 15:27:17|
|球员详情|	GET| /api/v2/sports/basketball/player/detail|	 GK数据|	2019-04-19 15:33:16|
|球队阵容|	GET| /api/v2/sports/basketball/team/lineup|	 GK数据|	2019-04-19 15:29:20|
|赛季球员统计|	GET| /api/v2/sports/basketball/season/players_stats|	 GK数据|	2019-04-19 15:31:56|



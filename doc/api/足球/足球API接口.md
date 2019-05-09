# 足球API接口

## 1、足球比赛
### 1.1、基础接口
| 接口名称 [4] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|  [赛事球队变动](赛事球队变动.md)	|GET| api/sports/football/update/profile|	 GK数据	|2019-04-19 14:43:50|
| 足球赛事资料	|GET |api/sports/football/matchevent/list|	 GK数据	|2019-04-19 14:50:30|
| 足球球队资料	|GET |api/sports/football/team/list|	 GK数据	|2019-04-19 14:49:07|
| 足球删除比赛	|GET| api/sports/football/match/deleted_ids|	 GK数据	|2019-03-14 10:15:32	|




### 1.2、即时数据
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|足球实时统计|	GET| /api/sports/football/match/detail_live|	 GK数据|	2019-04-18 19:29:06|
|足球即时比分|	GET| /api/sports/football/match/live|	 GK数据|	2019-04-16 14:36:30|
|足球赛程赛果|	GET| /api/sports/football/match/list|	 GK数据|	2019-04-19 14:51:15|

### 1.3、赛事分析
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|足球比赛详情|	GET| /api/sports/football/match/detail|	 GK数据|	2019-04-19 14:52:22|
|足球比赛阵容|	GET| /api/sports/football/match/lineup|	 GK数据|	2019-04-19 14:52:46|
|足球分析数据|	GET| /api/sports/football/match/analysis|	 GK数据|	2019-04-19 16:33:07|


### 1.4、即时指数
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|足球实时指数|	GET| /api/sports/football/odds/live_history|	 GK数据|	2019-03-04 17:35:18|
|单场指数历史|	GET| /api/sports/football/odds/history|	 GK数据|	2019-04-10 11:50:33|

### 1.5、百欧指数
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|实时百欧指数|	GET| /api/sports/football/odds/europe/live|	 GK数据|	2019-04-04 16:36:17|
|单场百欧历史|	GET| /api/sports/football/odds/europe/history|	 GK数据|	2019-04-04 16:36:32|
|百欧公司列表|	GET| /api/sports/odds/company/list|	 GK数据|	2019-04-04 16:11:35|
### 1.6、情报分析
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|情报分析接口|	GET| /api/sports/football/match/intelligence|	 GK数据|	2019-04-03 12:17:39|

### 1.7、动画直播
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|足球动画直播|	GET| mlive|	 GK数据|	2018-09-12 13:44:29|

### 1.8、资料库
| 接口名称 [11] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|足球赛制说明|	GET| /api/sports/football/competition/rule/list|	 GK数据|	2019-03-29 17:14:50|
|足球赛季列表|	GET| /api/sports/football/season/list|	 GK数据|	2019-04-19 14:56:07|
|足球转会列表|	GET| /api/sports/football/transfer/list|	 GK数据|	2019-04-28 15:40:37|
|足球球员详情|	GET| /api/sports/football/player/detail|	 GK数据|	2019-05-06 12:00:00|
|球队球员数据统计|	GET| /api/sports/football/season/stats|	 GK数据|	2019-04-19 14:58:34|
|足球赛季详情|	GET| /api/sports/football/season/detail|	 GK数据|	2019-04-19 15:05:54|
|足球球员荣誉列表|	GET| /api/sports/football/player/honor/list|	 GK数据|	2019-05-09 10:37:55|
|国家队FIFA排名|	GET| /api/sports/football/ranking/fifa|	 GK数据|	2019-04-19 15:06:50|
|足球球员列表|	GET| /api/sports/football/player/list|	 GK数据|	2019-04-12 16:32:44|
|足球球队详情|	GET| /api/sports/football/team/detail|	 GK数据|	2019-04-28 15:41:38|
|俱乐部积分排名|	GET| /api/sports/football/ranking/club|	 GK数据|	2019-04-19 15:08:05|


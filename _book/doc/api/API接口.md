# API接口

## 1、足球比赛
### 1.1、基础接口
| 接口名称 [4] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
| [赛事球队变动](/doc/api/足球/赛事球队变动.html)	|GET| api/sports/football/update/profile|	 GK数据	|2019-04-19 14:43:50|
| 足球赛事资料	|GET |api/sports/football/matchevent/list|	 GK数据	|2019-04-19 14:50:30|
| 足球球队资料	|GET |api/sports/football/team/list|	 GK数据	|2019-04-19 14:49:07|
| 足球删除比赛	|GET| api/sports/football/match/deleted_ids|	 GK数据	|2019-03-14 10:15:32	|



#### 1.1.1、 赛事球队变动
启用
HTTP
/api/sports/football/update/profile
GET
##### 1.1.1.1、请求参数
| 序号 | 参数名 |说明 | 必填 | 类型|示例 |详情|
| :---- | :----| :------------ |:---- |:-----|:-----|:-----|
						
|1	|user|	用户名，请联系商务|	是|	[string]|		
|2	|secret	|用户密钥，请联系商务|	是|	[string]|		
##### 1.1.1.2、返回参数
| 序号 | 参数名 |说明 | 必含 | 类型|详情|
| :---- | :----| :------------ |:---- |:-----:-----|
|1|	update|	更新、增加|	是|	[json]	|查看|
|2|	delete|	删除|	是|	[json]|	查看|

##### 1.1.1.3、详细说明


返回近2小时内有变动（增、删、改）的球队、赛事信息
**update 更新字段说明**
```
{
  "teams": [
    {
      "id": 43872,//球队id
      "competition_id": 2115,//赛事id
      "name_zh": "堤格雷斯女足",//中文名
      "name_zht": "堤格雷斯女足",//粤语名
      "name_en": "Tigres Women",//英文名
      "logo": "5731d0f14705060246ac2ac1a02b104f.png",//球队logo，前缀：http://cdn.sportnanoapi.com/football/team/
      "found": 0,//成立年份
      "website": ""//官网
      "national": 0,//是否国家队
      "country_logo": "",//国家队logo
    }
  ],
  "competitons": [
    {
      "id": 542,//赛事id
      "type": 1,//赛事类型
      "area_id ": 4,//区域id
      "country_id": 69,//国家id
      "name_zh": "中国超级联赛",//中文名
      "short_name_zh": "中超",//简称
      "name_zht": "中國超級聯賽",//粤语名
      "short_name_zht": "中超",//粤语简称
      "name_en": "Chinese Super League",//英文名
      "short_name_en": "CHA CSL",//英文简称
      "logo": "74ef1042c6c061f558f409876602732d.png"//赛事logo，前缀：http://cdn.sportnanoapi.com/football/competition/
    }
  ]
}
```
**delete 删除字段说明**
```
{
  "teams": [
   1,//球队id
   2,//球队id
   3
  ],
  "competitons": [
    1,//赛事id
    2
  ]
}
``` 
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


## 2、篮球比赛
### 2.1、基础接口
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球赛事列表|	GET| /api/sports/basketball/matchevent/list	| GK数据|	2018-07-05 17:38:47|
|篮球球队列表|	GET| /api/sports/basketball/team/list|	 GK数据|	2019-02-26 16:51:10|
|篮球删除比赛|	GET| /api/sports/basketball/match/deleted_ids|	 GK数据|	2019-03-14 10:15:42|

### 2.2、即时数据
| 接口名称 [3] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球实时统计|	GET| /api/sports/basketball/match/detail_live|	 GK数据|	2019-04-18 19:28:41|
|篮球赛程赛果|	GET| /api/sports/basketball/match/list|	 GK数据|	2019-04-19 11:57:25|
|篮球即时比分|	GET| /api/sports/basketball/match/live|	 GK数据|	2019-04-11 18:33:56|

### 2.3、赛事分析
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球比赛详情|	GET| /api/sports/basketball/match/detail|	 GK数据|	2019-04-19 15:24:28|
|篮球分析数据|	GET| /api/sports/basketball/match/analysis|	 GK数据|	2019-04-19 16:33:30|

### 2.4、即时指数
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球实时指数|	GET| /api/sports/basketball/odds/live_history|	 GK数据	|2019-01-24 10:45:46|
|单场指数历史|	GET| /api/sports/basketball/odds/history|	 GK数据	|2019-04-10 11:51:48|


### 2.5、情报分析
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球比赛情报|	GET| /api/sports/basketball/match/intelligence|	 GK数据|	2018-09-11 11:01:22|
### 2.6、动画直播
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|篮球动画直播	|GET| mlive|	 GK数据|	2018-06-07 10:29:38|


### 2.7、资料库
| 接口名称 [7] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|赛季列表|	GET| /api/v2/sports/basketball/season/list|	 GK数据|	2019-02-21 17:33:47|
|赛季赛程|	GET| /api/v2/sports/basketball/season/matches|	 GK数据|	2019-04-19 15:25:50|
|赛季球队统计|	GET| /api/v2/sports/basketball/season/teams_stats|	 GK数据|	2019-04-19 15:26:17|
|赛季积分榜|	GET| /api/v2/sports/basketball/season/tables|	 GK数据|	2019-04-19 15:27:17|
|球员详情|	GET| /api/v2/sports/basketball/player/detail|	 GK数据|	2019-04-19 15:33:16|
|球队阵容|	GET| /api/v2/sports/basketball/team/lineup|	 GK数据|	2019-04-19 15:29:20|
|赛季球员统计|	GET| /api/v2/sports/basketball/season/players_stats|	 GK数据|	2019-04-19 15:31:56|



## 3、体彩指数

### 3.1、体彩关联
| 接口名称 [1] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|体彩比赛关联|	GET| /api/sports/lottery/match/list|	 GK数据|	2019-04-26 16:49:10|

### 3.2、传统足彩接口
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|传统足彩赛程|	GET| /api/v2/sports/zc/matches|	 GK数据|	2019-03-13 16:48:02|
|传统足彩开奖结果|	GET| /api/v2/sports/zc/result|	 GK数据|	2019-04-28 11:55:26|

### 3.3、北单接口
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|北京单场指数|	GET| /api/v2/sports/bd/odds|	 GK数据|	2019-03-13 16:48:54|
|北京单场开奖结果|	GET| /api/v2/sports/bd/result|	 GK数据|	2019-04-28 11:51:21|

### 3.4、竞彩接口
| 接口名称 [2] | 方法 |接口URI | 最近更新者 | 更新日期|
| :---------- | :----| :--------------------------- |:--------- |:----------------|
|竞彩比赛指数|	GET| /api/sports/jc/odds|	 GK数据|	2019-03-13 16:49:13|
|竞彩开奖结果|	GET| /api/v2/sports/jc/result|	 GK数据|	2019-04-28 11:53:18|
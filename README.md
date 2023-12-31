# LocalArknights

此仓库为LocalArknights 1.9.3 Beta 3.jar的资源文件仓库

原仓库已于2021年停止更新并进行删库，倒卖风波已过，因此公开该代码以方便各位搭建、游玩和学习此仓库仅供内容保留，仓库所有者仅进行源代码修复，不会进行任何游戏内容的更新

[资源文件仓库](https://github.com/jiellll1219/LocalArns-res) [源代码仓库](https://github.com/jiellll1219/LocalArns)

## 如何使用

- 启动MySQL
- 克隆此仓库至本地
- 把预编译或自行编译的jar放到克隆的文件夹内
- 使用 ```java -jar "hypergryph-1.9.4 Beta 3.jar" ```启动

### 前置条件

1. MySQL 不低于8.0.10
	* [MySql](https://dev.mysql.com/downloads/mysql/)
2. Java 不低于1.8.0
	* [Java 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
	* [Java SE 8](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html)

## 已实现功能

好友系统

助战系统

公开招募

干员寻访

干员一系列养成

商店源石、皮肤的购买

战斗（可以推图，有掉落） 目前可推进度6-1

基建：制造站、贸易站、加工站、专精训练

邮件收发

Mod加载

## 客户端下载

[百度网盘](https://pan.baidu.com/s/1P_GFqVulkx7LRWe6yr1-0A?pwd=1145)

[微云](https://share.weiyun.com/OS49Gfbk)

[谷歌云盘](https://drive.google.com/drive/folders/1NmT4rF1Fm4QRut2Hdr9rbS7OtU1cH3-0?usp=share_link)

[OneDrive](https://1drv.ms/u/s!AvymlfMQY0dAdWwryYgMp1GzvLk?e=lnn5JY)

[MEGA](https://mega.nz/folder/laA00QRZ#D0-Qf8rvRs9G4Jik53XZgg)


# 指南

以下为各类数据编辑帮助，仅供参考，请按照实际情况调整

## 各类常用数据文件位置

账户数据: 数据库-account表-user项  
角色id表： data/excel/charcter_table.json  
物品id表： data/excel/item_table.json  
皮肤id表： data/excel/skin_table.json  
合约id表： data/excel/crisis_table.json

## 数据编辑
1. 定位账户主要数据
				账户数据搜索 `status`

	#### 格式
	```
	"status"{
	"ap": 0,
        "exp": 0,
        "uid": 0,
        "gold": 0,
		"flangs":{...
		},
		        "level": 0,
        "maxAp": 0,
        "avatar": {
            "id": "avatar_def_06",
            "type": "ICON"
        },
        "resume": "简介内容",
        "avatarId": "0",
        "hggShard": 0,
        "lggShard": 0,
        "nickName": "账户名称",
        "progress": 0,
        "secretary": "看板角色id",
        "gachaCount": 0,
        "iosDiamond": 0,
        "nickNumber": "0",
        "registerTs": 0,
        "serverName": "服务器名称",
        "gachaTicket": 0,
        "socialPoint": 0,
        "diamondShard": 0,
        "lastOnlineTs": 0,
        "apLimitUpFlag": 0,
        "lastApAddTime": 0,
        "lastRefreshTs": 0,
        "androidDiamond": 0,
        "friendNumLimit": 0,
        "globalVoiceLan": "JP",
        "practiceTicket": 0,
        "recruitLicense": 0,
        "tenGachaTicket": 0,
        "secretarySkinId": "看板角色皮肤id",
        "buyApRemainTimes": 0,
        "mainStageProgress": "main_01-01",//主线进度
        "instantFinishTicket": 0,
        "tipMonthlyCardExpireTs": 0,
        "monthlySubscriptionEndTime": 0,
        "monthlySubscriptionStartTime": 0
	},
	```

2. 定位账户基建数据

	账户数据搜索 `building`

    #### 格式
    ```
    "building"{
        "chars": {
            "1": {
                "ap": 0,
                "index": -1,
                "bubble": {
                    "assist": {
                        "ts": 0,
                        "add": -1
                    },
                    "normal": {
                        "ts": 0,
                        "add": -1
                    }
                },
                "charId": "角色id",
                "workTime": 0,
                "roomSlotId": "",
                "changeScale": 0,
                "lastApAddTime": 0
            },
            "2": {...
            },
            "3": {...
            }
    },
    ```
    
3. 定位干员数据	

	账户数据搜索搜索 `chars`

    #### 格式
    ```
    "chars": {
    "1": {
                "exp": 0,
                "skin": "char_002_amiya@test#1",
                "equip": {},
                "level": 1,
                "charId": "char_002_amiya",
                "instId": 1,
                "skills": [{
                    "state": 0,
                    "unlock": 1,
                    "skillId": "skcom_magic_rage[3]",
                    "specializeLevel": 3,
                    "completeUpgradeTime": -1
                }, {
                    "state": 0,
                    "unlock": 1,
                    "skillId": "skchr_amiya_2",
                    "specializeLevel": 3,
                    "completeUpgradeTime": -1
                }, {
                    "state": 0,
                    "unlock": 1,
                    "skillId": "skchr_amiya_3",
                    "specializeLevel": 3,
                    "completeUpgradeTime": -1
                }],
                "gainTime": 0,
                "voiceLan": "JP",
                "favorPoint": 0,
                "evolvePhase": 0,
                "currentEquip": null,
                "mainSkillLvl": 0,
                "potentialRank": 1,
                "defaultSkillIndex": 0
            },
            "2": {...
            },
            "3": {...
            }
    },
    ```

## 卡池编辑

#### 卡池更换  
config中修改timestamp参数为卡池openTime后或endtimp前  

```
"timestamp":{
		"monday":1645437600,
		"tuesday":1644919200,
		"wednesday":1645005600,
		"thursday":1645092000,
		"friday":1645178400,
		"saturday":1645264800,
		"sunday":1645351200
	},
```
详情请查看卡池信息文件，该文件位于  
* "server_location"/excel/gacha_table.json

卡池模板位置  
* "server_location"/data/gahca

`perAvailList`为卡池可获得的角色

`rarityRank`为干员稀有度，合法范围为0-5

在`rarityRank`下方的`charIdList`为干员id表

`totalPercent`为获得概率，单位为小数，合法范围在0-1  
* 请注意，全部列表相加的获得概率不要超过1，否则可能引发故障

`upCharInfo`为获得概率提升列表，规则与上述相同

#### 如要添加新的自定义卡池请按规律命名json文件并在`gacha_table.json`中添加该卡池id与时间

## 可能导致存档损坏的事件列举

1. 干员信物数量过多（16/32/64）
2. 任意物品数量为负
3. 拥有有时间限期的物品
4. 基建中干员调整

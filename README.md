# LocalArknights

�˲ֿ�ΪLocalArknights 1.9.3 Beta 3.jar����Դ�ļ��ֿ�

ԭ�ֿ�����2021��ֹͣ���²�����ɾ�⣬�����粨�ѹ�����˹����ô����Է����λ��������ѧϰ�˲ֿ�������ݱ������ֿ������߽�����Դ�����޸�����������κ���Ϸ���ݵĸ���

[��Դ�ļ��ֿ�](https://github.com/jiellll1219/LocalArns-res) [Դ����ֿ�](https://github.com/jiellll1219/LocalArns)

## ���ʹ��

- ����MySQL
- ��¡�˲ֿ�������
- ��Ԥ��������б����jar�ŵ���¡���ļ�����
- ʹ�� ```java -jar "hypergryph-1.9.4 Beta 3.jar" ```����

### ǰ������

1. MySQL ������8.0.10
	* [MySql](https://dev.mysql.com/downloads/mysql/)
2. Java ������1.8.0
	* [Java 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
	* [Java SE 8](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html)

## ��ʵ�ֹ���

����ϵͳ

��սϵͳ

������ļ

��ԱѰ��

��Աһϵ������

�̵�Դʯ��Ƥ���Ĺ���

ս����������ͼ���е��䣩 Ŀǰ���ƽ���6-1

����������վ��ó��վ���ӹ�վ��ר��ѵ��

�ʼ��շ�

Mod����

## �ͻ�������

[�ٶ�����](https://pan.baidu.com/s/1P_GFqVulkx7LRWe6yr1-0A?pwd=1145)

[΢��](https://share.weiyun.com/OS49Gfbk)

[�ȸ�����](https://drive.google.com/drive/folders/1NmT4rF1Fm4QRut2Hdr9rbS7OtU1cH3-0?usp=share_link)

[OneDrive](https://1drv.ms/u/s!AvymlfMQY0dAdWwryYgMp1GzvLk?e=lnn5JY)

[MEGA](https://mega.nz/folder/laA00QRZ#D0-Qf8rvRs9G4Jik53XZgg)


# ָ��

����Ϊ�������ݱ༭�����������ο����밴��ʵ���������

## ���ೣ�������ļ�λ��

�˻�����: ���ݿ�-account��-user��  
��ɫid�� data/excel/charcter_table.json  
��Ʒid�� data/excel/item_table.json  
Ƥ��id�� data/excel/skin_table.json  
��Լid�� data/excel/crisis_table.json

## ���ݱ༭
1. ��λ�˻���Ҫ����
				�˻��������� `status`

	#### ��ʽ
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
        "resume": "�������",
        "avatarId": "0",
        "hggShard": 0,
        "lggShard": 0,
        "nickName": "�˻�����",
        "progress": 0,
        "secretary": "�����ɫid",
        "gachaCount": 0,
        "iosDiamond": 0,
        "nickNumber": "0",
        "registerTs": 0,
        "serverName": "����������",
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
        "secretarySkinId": "�����ɫƤ��id",
        "buyApRemainTimes": 0,
        "mainStageProgress": "main_01-01",//���߽���
        "instantFinishTicket": 0,
        "tipMonthlyCardExpireTs": 0,
        "monthlySubscriptionEndTime": 0,
        "monthlySubscriptionStartTime": 0
	},
	```

2. ��λ�˻���������

	�˻��������� `building`

    #### ��ʽ
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
                "charId": "��ɫid",
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
    
3. ��λ��Ա����	

	�˻������������� `chars`

    #### ��ʽ
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

## ���ر༭

#### ���ظ���  
config���޸�timestamp����Ϊ����openTime���endtimpǰ  

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
������鿴������Ϣ�ļ������ļ�λ��  
* "server_location"/excel/gacha_table.json

����ģ��λ��  
* "server_location"/data/gahca

`perAvailList`Ϊ���ؿɻ�õĽ�ɫ

`rarityRank`Ϊ��Աϡ�жȣ��Ϸ���ΧΪ0-5

��`rarityRank`�·���`charIdList`Ϊ��Աid��

`totalPercent`Ϊ��ø��ʣ���λΪС�����Ϸ���Χ��0-1  
* ��ע�⣬ȫ���б���ӵĻ�ø��ʲ�Ҫ����1�����������������

`upCharInfo`Ϊ��ø��������б�������������ͬ

#### ��Ҫ����µ��Զ��忨���밴��������json�ļ�����`gacha_table.json`����Ӹÿ���id��ʱ��

## ���ܵ��´浵�𻵵��¼��о�

1. ��Ա�����������ࣨ16/32/64��
2. ������Ʒ����Ϊ��
3. ӵ����ʱ�����ڵ���Ʒ
4. �����и�Ա����

# 删除备份-DeleteUDBBackup

删除UDB实例备份

# Request Parameters
|Parameter name|Type|Description|Required|
|---|---|---|---|
|Region|string|地域。 参见 [地域和可用区列表](../summary/regionlist.html)|**Yes**|
|Zone|string|可用区。参见 [可用区列表](../summary/regionlist.html)|**Yes**|
|ProjectId|string|项目ID。不填写为默认项目，子帐号必须填写。 请参考[GetProjectList接口](../summary/get_project_list.html)|No|
|BackupId|int|备份id，可通过DescribeUDBBackup获得|**Yes**|

# Response Elements
|Parameter name|Type|Description|Required|
|---|---|---|---|
|RetCode|int|返回码|**Yes**|
|Action|string|操作名称|**Yes**|

# Request Example
```
https://api.ucloud.cn/?Action=DeleteUDBBackup
&Region=cn-bj2
&Zone=cn-bj2-04
&BackupId=5160
```

# Response Example
```
{
    "Action": "DeleteUDBBackupResponse", 
    "RetCode": 0
}
```

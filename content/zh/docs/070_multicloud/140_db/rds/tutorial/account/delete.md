---
title: "删除"
date: 2021-06-23T08:22:33+08:00
weight: 10
description: >
   删除RDS实例账号
---


{{< tabs >}}
{{% tab name="控制台" %}}

 ![删除RDS实例账号](../../../images/rds_account_delete.png)


{{% /tab %}}


{{% tab name="命令行" %}}
```bash
# 删除RDS实例账号
$ climc dbinstance-account-delete 02c5634d-40bf-40f2-8212-4773c4dc9f0e
+----------------------+--------------------------------------------------------------------------------------------------------------------------+
|        Field         |                                                          Value                                                           |
+----------------------+--------------------------------------------------------------------------------------------------------------------------+
| account              | qj-jd                                                                                                                    |
| account_id           | 96f46c61-38c4-4fd7-857a-effb4f69eabf                                                                                     |
| brand                | JDcloud                                                                                                                  |
| can_delete           | true                                                                                                                     |
| can_update           | true                                                                                                                     |
| cloud_env            | public                                                                                                                   |
| cloudregion          | JDcloud 华北-北京                                                                                                        |
| cloudregion_id       | 5323c848-cbe8-4d1d-8319-e42641fed2f2                                                                                     |
| created_at           | 2021-06-22T07:05:37.000000Z                                                                                              |
| dbinstance           | testrds                                                                                                                  |
| dbinstance_id        | c466cc2b-5377-4bf3-8cf8-f9d8c89fb955                                                                                     |
| dbinstanceprivileges | [{"account":"hello","database":"test","dbinstancedatabase_id":"034f9dea-f23f-4d0f-84be-697a62101d16","privileges":"rw"}] |
| deleted              | false                                                                                                                    |
| host                 | %                                                                                                                        |
| id                   | 02c5634d-40bf-40f2-8212-4773c4dc9f0e                                                                                     |
| is_emulated          | false                                                                                                                    |
| manager              | qj-jd                                                                                                                    |
| manager_domain       | Default                                                                                                                  |
| manager_domain_id    | default                                                                                                                  |
| manager_id           | 8e47bb75-5105-4ef9-84b8-8aa5927b06dd                                                                                     |
| manager_project      | system                                                                                                                   |
| manager_project_id   | a9a365125abf43c580ba98e5640b5c51                                                                                         |
| name                 | hello                                                                                                                    |
| project              | system                                                                                                                   |
| project_domain       | Default                                                                                                                  |
| project_id           | a9a365125abf43c580ba98e5640b5c51                                                                                         |
| provider             | JDcloud                                                                                                                  |
| region               | JDcloud 华北-北京                                                                                                        |
| region_ext_id        | cn-north-1                                                                                                               |
| region_external_id   | JDcloud/cn-north-1                                                                                                       |
| region_id            | 5323c848-cbe8-4d1d-8319-e42641fed2f2                                                                                     |
| status               | deleting                                                                                                                 |
| tenant               | system                                                                                                                   |
| tenant_id            | a9a365125abf43c580ba98e5640b5c51                                                                                         |
| update_version       | 1                                                                                                                        |
| updated_at           | 2021-06-24T06:33:31.000000Z                                                                                              |
| vpc                  | newvpc                                                                                                                   |
| vpc_ext_id           | vpc-cyeqenbik9                                                                                                           |
| vpc_id               | d532c177-e8e3-42d3-82c4-af6bef949566                                                                                     |
+----------------------+--------------------------------------------------------------------------------------------------------------------------+
```
{{% /tab %}}
{{< /tabs >}}

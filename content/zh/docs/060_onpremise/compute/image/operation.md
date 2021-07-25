---
title: "其他操作"
date: 2019-07-19T17:29:09+08:00
weight: 100
---

## 导入镜像

云平台的 glance 镜像服务支持从外部 url 导入镜像，对应 climc 的子命令为 `image-import`　。

```bash
# 导入 https://iso.yunion.cn/yumrepo-3.2/images/cirros-0.4.0-x86_64-disk.qcow2 镜像
$ climc image-import --format qcow2 --os-type Linux cirros-test.qcow2 https://iso.yunion.cn/yumrepo-3.2/images/cirros-0.4.0-x86_64-disk.qcow2
```

使用 `image-list` 或 `image-show` 查询导入镜像的状态，变为 active 时表明可以使用。

## 下载镜像

如果需要将云平台的镜像导出到本地，就需要用 `climc image-download` 把 glance 存的镜像下载下来。

参考 [查询镜像](../query/) 查询你想要下载的镜像，获取镜像 id 或 name。

下载镜像:

```bash
# OUTPUT 指定镜像的保存路径和文件名称，如/root/test.qcow2
$ climc image-download [--output OUTPUT] <image_id>
```

## 删除镜像

镜像默认启用了删除保护，当镜像确定不用了，需要先通过`climc image-update`禁用删除保护，再通过 `climc image-delete` 删除镜像。

```bash

# 禁用镜像删除保护
$ climc image-update --unprotected <image_id>
# 删除镜像
$ climc image-delete <image_id>
```

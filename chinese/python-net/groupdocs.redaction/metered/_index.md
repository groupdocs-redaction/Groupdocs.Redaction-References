---
title: "Metered 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "管理计量（按使用付费）许可证。"
type: docs
url: /zh/python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

管理计量（按使用付费）许可证。

Metered 许可证根据实际消耗计费（通常是页面或
处理的文档）。在应用启动时设置一次公私钥对
应用启动时；包装器会将使用情况报告回 GroupDocs
后台的许可证服务器。

Metered 类型公开以下成员：

### 方法
| 方法 | 描述 |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | 返回当前密钥的剩余计量信用。 |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | 返回迄今为止已消耗的总计量数量。 |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | 使用给定的公钥/私钥对激活计量计费。 |

### 另请参阅
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)

---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化 LoadOptions 类的新实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

初始化 LoadOptions 类的新实例。

```python
def __init__(self):
    ...
```

## __init__ {#password}

使用指定的密码初始化 LoadOptions 的新实例。

```python
def __init__(self, password):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| password | `str` | 受保护文件的密码。 |

### 示例

```python
    from groupdocs.redaction.options import LoadOptions

    # 加载受密码保护的文档
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

使用指定的预光栅化标志初始化新的 LoadOptions 实例。

```python
def __init__(self, pre_rasterize):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| pre_rasterize | `bool` | 如果为 True，则在加载时强制光栅化。 |

## __init__ {#password-pre_rasterize}

使用指定的密码初始化新的 LoadOptions 实例。

如果 `pre_rasterize` 为 True，则在加载文档时强制进行光栅化。

```python
def __init__(self, password, pre_rasterize):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| password | `str` | 受保护文件的密码。 |
| pre_rasterize | `bool` | 如果为 True，则在加载时强制光栅化。 |

### 示例

```python
from groupdocs.redaction.options import LoadOptions

# 加载受密码保护的文档
load_opt = LoadOptions("mypassword")
```

### 另请参阅
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)

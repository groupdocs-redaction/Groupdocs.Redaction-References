---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "編集完了ステータスを表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

編集完了ステータスを表します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Applied](#Applied) | リダクションは完全にかつ成功裏に適用されました。 |
|
|  | [PartiallyApplied](#PartiallyApplied) | リダクションは一致の一部にのみ適用されました。 |
|
|  | [Skipped](#Skipped) | レダクションはスキップされました（適用されません）。 |
|
|  | [Failed](#Failed) | 例外によりレダクションが失敗しました。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


リダクションは完全にかつ成功裏に適用されました。


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


リダクションは一致の一部にのみ適用されました。


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


レダクションはスキップされました（適用されません）。


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


例外によりレダクションが失敗しました。


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)

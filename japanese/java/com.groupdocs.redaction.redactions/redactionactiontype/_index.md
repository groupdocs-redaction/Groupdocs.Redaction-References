---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "削除を実行するために取れるアクションを表します。"
type: docs
weight: 37
url: /ja/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

削除を実行するために取れるアクションを表します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [Replacement](#Replacement) | 編集されたテキストは別のテキストに置き換えられるか、ブロックで覆われました。 |
|
|  | [Cleanup](#Cleanup) | データは削除されましたが、空のオブジェクトがドキュメントに残ります。 |
|
|  | [Deletion](#Deletion) | データと関連する構造がドキュメントから削除されました。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


編集されたテキストは別のテキストに置き換えられるか、ブロックで覆われました。


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


データは削除されましたが、空のオブジェクトがドキュメントに残ります。


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


データと関連する構造がドキュメントから削除されました。


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)

---
title: "ReplacementType"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "一致したテキストの置換タイプを表します。"
type: docs
weight: 38
url: /ja/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

一致したテキストの置換タイプを表します。

## フィールド

| フィールド | 説明 |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | 一致したテキストを別の文字列に置き換えます（例:）。 |
|
|  | [DrawBox](#DrawBox) | 削除されたテキストの代わりに、特定の色（デフォルトは黒）の矩形を描画します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


一致したテキストを別の文字列に置き換えます（例: 免除コード）。


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


削除されたテキストの代わりに、特定の色（デフォルトは黒）の矩形を描画します。


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
| 名前 | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)

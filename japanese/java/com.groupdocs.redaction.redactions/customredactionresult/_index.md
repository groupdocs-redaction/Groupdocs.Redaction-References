---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "返される結果を表します。"
type: docs
weight: 14
url: /ja/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

返される結果を表します [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler)。

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getApply()](#getApply--) | 置換を適用すべきかどうかを示す値を取得します。 |
|
|  | [setApply(boolean value)](#setApply-boolean-) | 置換を適用すべきかどうかを示す値を設定します。 |
|
|  | [getText()](#getText--) | #getApply().getApply() が true のときに使用される置換テキストを取得します |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | #getApply().getApply() が true のときに使用される置換テキストを設定します |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


置換を適用すべきかどうかを示す値を取得します。


**Returns:**
boolean -  true  は一致したテキストを #getText().getText() で置き換えるためです。false の場合は置き換えません。

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


置換を適用すべきかどうかを示す値を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | boolean | true  は置換を適用することを意味し、false の場合は適用しません。 |
|

### getText() {#getText--}
```
public final String getText()
```


#getApply().getApply() が true のときに使用される置換テキストを取得します
true
.


**Returns:**
java.lang.String - 置換テキストです。

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


#getApply().getApply() が true のときに使用される置換テキストを設定します
true
.


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | 置換テキストです。 |
|


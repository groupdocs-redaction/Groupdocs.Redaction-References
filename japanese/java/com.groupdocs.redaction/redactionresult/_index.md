---
title: "RedactionResult"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "編集操作の結果を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

編集操作の結果を表します。

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 実行ステータスを取得します。 |
|
|  | [getErrorMessage()](#getErrorMessage--) | 診断用エラーメッセージを取得します。 |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | スキップされたステータスで RedactionResult クラスの新しいインスタンスを初期化します。 |
|
|  | [partial(String description)](#partial-java.lang.String-) | 部分的に適用されたステータスで RedactionResult クラスの新しいインスタンスを初期化します。 |
|
|  | [failed(String description)](#failed-java.lang.String-) | 失敗ステータスで RedactionResult クラスの新しいインスタンスを初期化します。 |
|
|  | [successful()](#successful--) | 適用（成功）ステータスで RedactionResult クラスの新しいインスタンスを初期化します。 |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


実行ステータスを取得します。


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


診断用エラーメッセージを取得します。


**Returns:**
java.lang.String - 診断用エラーメッセージ。

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


スキップされたステータスで RedactionResult クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 説明 | java.lang.String | 操作がスキップされた理由 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


部分的に適用されたステータスで RedactionResult クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 説明 | java.lang.String | 操作が完全に適用されなかった理由 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


失敗ステータスで RedactionResult クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | 説明 | java.lang.String | 失敗または例外の詳細 |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


適用（成功）ステータスで RedactionResult クラスの新しいインスタンスを初期化します。


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result


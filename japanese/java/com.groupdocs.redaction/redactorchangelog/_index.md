---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "Redactor クラスの Apply メソッドに渡された赤字リストの結果を表します。"
type: docs
weight: 17
url: /ja/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Apply() メソッドに渡された赤字リストの結果を表します。
Redactor
クラス。

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | RedactorChangeLog クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getStatus()](#getStatus--) | 適用されたすべての赤字の最終ステータスを取得します。 |
|
|  | [getRedactionLog()](#getRedactionLog--) | リストを取得します |
RedactorLogEntry
インスタンス。
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


RedactorChangeLog クラスの新しいインスタンスを初期化します。


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


適用されたすべての赤字の最終ステータスを取得します。


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


リストを取得します
RedactorLogEntry
インスタンス。


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - RedactorLogEntry インスタンスのリストです。


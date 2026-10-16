---
title: "RedactorSettings"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "編集プロセスをカスタマイズできるようにする、編集設定を表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.redaction.options/redactorsettings/
---
**Inheritance:**
java.lang.Object
```
public class RedactorSettings
```

赤字設定を表し、赤字プロセスをカスタマイズできるようにします。

*** ** * ** ***


**Learn more**

* More details about implementing ILogger interface: [Use advanced logging](../https://docs.groupdocs.com/redaction/java/use-advanced-logging/)
* More details about implementing IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [RedactorSettings()](#RedactorSettings--) | RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactorSettings(ILogger logger)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-) | 指定された ILogger インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactorSettings(IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-) | 指定された IRedactionCallback インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactorSettings(IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-) | 指定された IOcrConnector インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-) | 指定された ILogger と IRedactionCallback のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
|  | [RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)](#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-) | 指定された ILogger、IRedactionCallback、IOcrConnector のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getLogger()](#getLogger--) | 実装しているクラスのインスタンスを取得します |
ILogger
、イベントとエラーの記録に使用されます。
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.redaction.options.ILogger-) | 実装しているクラスのインスタンスを設定します |
ILogger
、イベントとエラーの記録に使用されます。
|
|  | [getRedactionCallback()](#getRedactionCallback--) | 実装しているクラスのインスタンスを取得します |
IRedactionCallback
.
|
|  | [setRedactionCallback(IRedactionCallback value)](#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-) | 実装しているクラスのインスタンスを設定します |
IRedactionCallback
.
|
|  | [getOcrConnector()](#getOcrConnector--) | 実装しているクラスのインスタンスを取得します |
IOcrConnector
インターフェイス。
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | 実装しているクラスのインスタンスを設定します |
IOcrConnector
インターフェイス。
|
### RedactorSettings() {#RedactorSettings--}
```
public RedactorSettings()
```


RedactorSettings クラスの新しいインスタンスを初期化します。


### RedactorSettings(ILogger logger) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-}
```
public RedactorSettings(ILogger logger)
```


指定された ILogger インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger インターフェイスを実装しているクラスのインスタンス |
|

### RedactorSettings(IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(IRedactionCallback callback)
```


指定された IRedactionCallback インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck インターフェイスを実装しているクラスのインスタンス |
|

### RedactorSettings(IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(IOcrConnector ocrConnector)
```


指定された IOcrConnector インスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector インターフェイスの有効な実装 |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback)
```


指定された ILogger と IRedactionCallback のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger インターフェイスを実装しているクラスのインスタンス |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck インターフェイスを実装しているクラスのインスタンス |
|

### RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector) {#RedactorSettings-com.groupdocs.redaction.options.ILogger-com.groupdocs.redaction.redactions.IRedactionCallback-com.groupdocs.redaction.integration.IOcrConnector-}
```
public RedactorSettings(ILogger logger, IRedactionCallback callback, IOcrConnector ocrConnector)
```


指定された ILogger、IRedactionCallback、IOcrConnector のインスタンスを使用して RedactorSettings クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.redaction.options/ilogger) | ILogger インターフェイスを実装しているクラスのインスタンス |
|
|  | callback | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallbck インターフェイスを実装しているクラスのインスタンス |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector インターフェイス実装のインスタンスです。null にすることができます。 |
|

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


実装しているクラスのインスタンスを取得します
ILogger
、イベントとエラーの記録に使用されます。


**Returns:**
[ILogger](../../com.groupdocs.redaction.options/ilogger) - An instance of a class, implementing  ILogger , that is used for logging events and errors.

### setLogger(ILogger value) {#setLogger-com.groupdocs.redaction.options.ILogger-}
```
public final void setLogger(ILogger value)
```


実装しているクラスのインスタンスを設定します
ILogger
、イベントとエラーの記録に使用されます。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.redaction.options/ilogger) | イベントとエラーのログ記録に使用される **ILogger** を実装したクラスのインスタンスです。 |
|

### getRedactionCallback() {#getRedactionCallback--}
```
public final IRedactionCallback getRedactionCallback()
```


実装しているクラスのインスタンスを取得します
IRedactionCallback
.


**Returns:**
[IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) - An instance of a class, implementing  IRedactionCallback .

### setRedactionCallback(IRedactionCallback value) {#setRedactionCallback-com.groupdocs.redaction.redactions.IRedactionCallback-}
```
public final void setRedactionCallback(IRedactionCallback value)
```


実装しているクラスのインスタンスを設定します
IRedactionCallback
.


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [IRedactionCallback](../../com.groupdocs.redaction.redactions/iredactioncallback) | IRedactionCallback を実装したクラスのインスタンスです。 |
|

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


実装しているクラスのインスタンスを取得します
IOcrConnector
インターフェイス。


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - An instance of a class, implementing  IOcrConnector  interface.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


実装しているクラスのインスタンスを設定します
IOcrConnector
インターフェイス。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector インターフェイスを実装したクラスのインスタンスです。 |
|


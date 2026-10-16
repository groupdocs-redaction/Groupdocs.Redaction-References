---
title: "従量課金"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "従量課金ライセンスを適用するためのメソッドを提供します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```

適用するためのメソッドを提供します
[Metered](../https://purchase.groupdocs.com/faqs/licensing/metered)
ライセンス。

<br />

*** ** * ** ***

**Learn more**

* More about Metered licensing: [Metered Licensing FAQ](../https://purchase.groupdocs.com/faqs/licensing/metered)
* More about GroupDocs.Signature licensing: [Evaluation Limitations and Licensing](../https://docs.groupdocs.com/display/signaturejava/Evaluation+Limitations+and+Licensing+of+GroupDocs.Signature)

<br />


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Metered()](#Metered--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | 従量課金キーで製品を有効化します。 |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 処理された MB の量を取得します。 |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 消費されたクレジット数を取得します。 |
|
### Metered() {#Metered--}
```
public Metered()
```


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


従量課金キーで製品を有効化します。

<br />

*** ** * ** ***

> ```
>  Following example demonstrates how to activate product with Metered keys.
>   string publicKey = "Public Key";
>  string privateKey = "Private Key";
>  Metered metered = new Metered();
>  metered.SetMeteredKey(publicKey, privateKey);
>  
>  
> ```

<br />



**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 公開鍵です。 |
|
|  | privateKey | java.lang.String | 秘密鍵です。 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


処理された MB の量を取得します。

<br />

*** ** * ** ***

> ```
>   Following example demonstrates how to retrieve amount of MBs processed.
>     string publicKey = "Public Key";
>   string privateKey = "Private Key";
>
>   Metered metered = new Metered();
>   metered.SetMeteredKey(publicKey, privateKey);
>   decimal mbProcessed = Metered.GetConsumptionQuantity();
>   
>   
> ```

<br />



**Returns:**
java.math.BigDecimal
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


消費されたクレジット数を取得します。

<br />

*** ** * ** ***

> ```
>   Following example demonstrates how to retrieve count of credits consumed.
>     string publicKey = "Public Key";
>   string privateKey = "Private Key";
>
>   Metered metered = new Metered();
>   metered.SetMeteredKey(publicKey, privateKey);
>   decimal creditsConsumed = Metered.GetConsumptionCredit();
>   
>   
> ```

<br />



**Returns:**
java.math.BigDecimal

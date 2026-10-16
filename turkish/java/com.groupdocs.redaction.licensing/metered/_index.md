---
title: "Ölçülen"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Ölçülen lisansı uygulamak için yöntemler sağlar."
type: docs
weight: 11
url: /tr/java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```

Uygulamak için yöntemler sağlar
[Metered](../https://purchase.groupdocs.com/faqs/licensing/metered)
lisans.

<br />

*** ** * ** ***

**Learn more**

* More about Metered licensing: [Metered Licensing FAQ](../https://purchase.groupdocs.com/faqs/licensing/metered)
* More about GroupDocs.Signature licensing: [Evaluation Limitations and Licensing](../https://docs.groupdocs.com/display/signaturejava/Evaluation+Limitations+and+Licensing+of+GroupDocs.Signature)

<br />


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Metered()](#Metered--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ölçülen anahtarlarla ürünü etkinleştirir. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | İşlenen MB miktarını alır. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Kullanılan kredi sayısını alır. |
|
### Metered() {#Metered--}
```
public Metered()
```


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Ölçülen anahtarlarla ürünü etkinleştirir.

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | publicKey | java.lang.String | Açık anahtar. |
|
|  | privateKey | java.lang.String | Özel anahtar. |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


İşlenen MB miktarını alır.

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


Kullanılan kredi sayısını alır.

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

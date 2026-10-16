---
title: "Metered"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt methoden voor het toepassen van een Metered-licentie."
type: docs
weight: 11
url: /nl/java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```

Biedt methoden voor het toepassen
[Metered](../https://purchase.groupdocs.com/faqs/licensing/metered)
licentie.

<br />

*** ** * ** ***

**Learn more**

* More about Metered licensing: [Metered Licensing FAQ](../https://purchase.groupdocs.com/faqs/licensing/metered)
* More about GroupDocs.Signature licensing: [Evaluation Limitations and Licensing](../https://docs.groupdocs.com/display/signaturejava/Evaluation+Limitations+and+Licensing+of+GroupDocs.Signature)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Metered()](#Metered--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Activeert het product met Metered-sleutels. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Haalt de hoeveelheid verwerkte MB's op. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Haalt het aantal verbruikte credits op. |
|
### Metered() {#Metered--}
```
public Metered()
```


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Activeert het product met Metered-sleutels.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | publicKey | java.lang.String | De openbare sleutel. |
|
|  | privateKey | java.lang.String | De privésleutel. |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Haalt de hoeveelheid verwerkte MB's op.

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


Haalt het aantal verbruikte credits op.

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

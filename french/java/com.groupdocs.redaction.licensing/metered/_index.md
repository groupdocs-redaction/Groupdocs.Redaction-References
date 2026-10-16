---
title: "Mesuré"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit des méthodes pour appliquer une licence Mesurée."
type: docs
weight: 11
url: /fr/java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```

Fournit des méthodes pour appliquer
[Metered](../https://purchase.groupdocs.com/faqs/licensing/metered)
licence.

<br />

*** ** * ** ***

**Learn more**

* More about Metered licensing: [Metered Licensing FAQ](../https://purchase.groupdocs.com/faqs/licensing/metered)
* More about GroupDocs.Signature licensing: [Evaluation Limitations and Licensing](../https://docs.groupdocs.com/display/signaturejava/Evaluation+Limitations+and+Licensing+of+GroupDocs.Signature)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Metered()](#Metered--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Active le produit avec des clés Mesurées. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Récupère la quantité de Mo traités. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Récupère le nombre de crédits consommés. |
|
### Metered() {#Metered--}
```
public Metered()
```


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Active le produit avec des clés Mesurées.

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
| Paramètre | Type | Description |
| --- | --- | --- |
|  | publicKey | java.lang.String | La clé publique. |
|
|  | privateKey | java.lang.String | La clé privée. |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Récupère la quantité de Mo traités.

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


Récupère le nombre de crédits consommés.

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

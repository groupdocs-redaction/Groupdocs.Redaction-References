---
title: "मेटर्ड"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "मेटर्ड लाइसेंस लागू करने के लिए विधियाँ प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```

लागू करने के लिए विधियाँ प्रदान करता है
[Metered](../https://purchase.groupdocs.com/faqs/licensing/metered)
लाइसेंस।

<br />

*** ** * ** ***

**Learn more**

* More about Metered licensing: [Metered Licensing FAQ](../https://purchase.groupdocs.com/faqs/licensing/metered)
* More about GroupDocs.Signature licensing: [Evaluation Limitations and Licensing](../https://docs.groupdocs.com/display/signaturejava/Evaluation+Limitations+and+Licensing+of+GroupDocs.Signature)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
| [Metered()](#Metered--) |  |
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | मेटर्ड कुंजियों के साथ उत्पाद को सक्रिय करता है। |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | प्रसंस्कृत MB की मात्रा प्राप्त करता है। |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | उपयोग किए गए क्रेडिट की गणना प्राप्त करता है। |
|
### Metered() {#Metered--}
```
public Metered()
```


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


मेटर्ड कुंजियों के साथ उत्पाद को सक्रिय करता है।

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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | publicKey | java.lang.String | सार्वजनिक कुंजी। |
|
|  | privateKey | java.lang.String | निजी कुंजी। |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


प्रसंस्कृत MB की मात्रा प्राप्त करता है।

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


उपयोग किए गए क्रेडिट की गणना प्राप्त करता है।

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

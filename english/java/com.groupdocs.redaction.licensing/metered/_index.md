---
title: Metered
second_title: GroupDocs.Redaction for Java API Reference
description: Provides methods which allow to activate product with Metered license and retrieve amount of MBs processed.
type: docs
weight: 17
url: /java/com.groupdocs.redaction.licensing/metered/
---
**Inheritance:**
java.lang.Object, com.groupdocs.redaction.licensing.MeteredCore
```
public class Metered extends MeteredCore
```

Provides methods which allow to activate product with Metered license and retrieve amount of MBs processed. Learn more about Metered licenses [here][].


[here]: https://purchase.groupdocs.com/faqs/licensing/metered
## Constructors

| Constructor | Description |
| --- | --- |
| [Metered()](#Metered--) | Initializes a new instance of Metered class. |
## Methods

| Method | Description |
| --- | --- |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Activates the product with Metered keys. |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Retrieves the amount of MBs processed. |
| [getConsumptionCredit()](#getConsumptionCredit--) | Gets the consumption credit. |
| [reportUsageInBytes(long bytesLength)](#reportUsageInBytes-long-) |  |
| [reportCreditsUsage(long usedCredits)](#reportCreditsUsage-long-) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initializes a new instance of Metered class.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Activates the product with Metered keys.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | The public key. |
| privateKey | java.lang.String | The private key. |

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Retrieves the amount of MBs processed.

**Returns:**
double - consumption quantity
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Gets the consumption credit.

**Returns:**
double - consumption quantity
### reportUsageInBytes(long bytesLength) {#reportUsageInBytes-long-}
```
public static void reportUsageInBytes(long bytesLength)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| bytesLength | long |  |

### reportCreditsUsage(long usedCredits) {#reportCreditsUsage-long-}
```
public static void reportCreditsUsage(long usedCredits)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| usedCredits | long |  |


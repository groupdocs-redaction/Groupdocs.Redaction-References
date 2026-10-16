---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar alternativ för ersättning av matchad text."
type: docs
weight: 31
url: /sv/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Representerar alternativ för ersättning av matchad text.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Initierar en ny instans av klassen ReplacementOptions med ersättningstext som ett alternativ. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Initierar en ny instans av klassen ReplacementOptions med färgad rektangel som ett alternativ. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getActionType()](#getActionType--) | Hämtar ersättningsåtgärden: rita ruta eller ersätta text. |
|
|  | [getReplacement()](#getReplacement--) | Hämtar det textuella ersättningsvärdet. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Ställer in det textuella ersättningsvärdet. |
|
|  | [getBoxColor()](#getBoxColor--) | Hämtar färgen för en |
ReplacementType.DrawBox
alternativ (ignoreras annars).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Ställer in färgen för en |
ReplacementType.DrawBox
alternativ (ignoreras annars).
|
|  | [getFilters()](#getFilters--) | Hämtar en array av filter som ska tillämpas med denna redigering. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Ställer in en array av filter som ska tillämpas med denna redigering. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Hämtar en anpassad redigeringshanterare. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Ställer in en anpassad redigeringshanterare. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Initierar en ny instans av klassen ReplacementOptions med ersättningstext som ett alternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ersättning | java.lang.String | Textuell ersättning |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Initierar en ny instans av klassen ReplacementOptions med färgad rektangel som ett alternativ.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | färg | java.awt.Color | Rektangelns färg |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Hämtar ersättningsåtgärden: rita ruta eller ersätta text.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Hämtar det textuella ersättningsvärdet.


**Returns:**
java.lang.String - Det textuella ersättningsvärdet.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Ställer in det textuella ersättningsvärdet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Det textuella ersättningsvärdet. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Hämtar färgen för en
ReplacementType.DrawBox
alternativ (ignoreras annars).


**Returns:**
java.awt.Color - Färgen för ett  ReplacementType.DrawBox  alternativ (ignoreras annars).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Ställer in färgen för en
ReplacementType.DrawBox
alternativ (ignoreras annars).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.awt.Color | Färgen för ett  ReplacementType.DrawBox  alternativ (ignoreras annars). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Hämtar en array av filter som ska tillämpas med denna redigering.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - En array av filter som ska tillämpas med denna redigering.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Ställer in en array av filter som ska tillämpas med denna redigering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | En array av filter som ska tillämpas med denna redigering. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Hämtar en anpassad redigeringshanterare. Stöds endast för PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Ställer in en anpassad redigeringshanterare. Stöds endast för PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | En instans av [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)

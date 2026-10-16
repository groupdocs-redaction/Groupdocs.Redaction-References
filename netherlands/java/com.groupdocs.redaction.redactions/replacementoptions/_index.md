---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt opties voor het vervangen van gematchte tekst."
type: docs
weight: 31
url: /nl/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Vertegenwoordigt opties voor het vervangen van gematchte tekst.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Initialiseert een nieuwe instantie van de ReplacementOptions‑klasse met vervangende tekst als optie. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Initialiseert een nieuwe instantie van de ReplacementOptions‑klasse met gekleurde rechthoek als optie. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getActionType()](#getActionType--) | Haalt de vervangingsactie op: vak tekenen of tekst vervangen. |
|
|  | [getReplacement()](#getReplacement--) | Haalt de tekstuele vervangingswaarde op. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Stelt de tekstuele vervangingswaarde in. |
|
|  | [getBoxColor()](#getBoxColor--) | Haalt de kleur op voor een |
ReplacementType.DrawBox
optie (genegeerd anders).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Stelt de kleur in voor een |
ReplacementType.DrawBox
optie (genegeerd anders).
|
|  | [getFilters()](#getFilters--) | Haalt een array van filters op die met deze redactie moeten worden toegepast. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Stelt een array van filters in om toe te passen met deze redactie. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Haalt een aangepaste redactiehandler op. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Stelt een aangepaste redactiehandler in. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Initialiseert een nieuwe instantie van de ReplacementOptions‑klasse met vervangende tekst als optie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | vervanging | java.lang.String | Tekstuele vervanging |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Initialiseert een nieuwe instantie van de ReplacementOptions‑klasse met gekleurde rechthoek als optie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | kleur | java.awt.Color | Rechthoekkleur |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Haalt de vervangingsactie op: vak tekenen of tekst vervangen.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Haalt de tekstuele vervangingswaarde op.


**Returns:**
java.lang.String - De tekstuele vervangingswaarde.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Stelt de tekstuele vervangingswaarde in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De tekstuele vervangingswaarde. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Haalt de kleur op voor een
ReplacementType.DrawBox
optie (genegeerd anders).


**Returns:**
java.awt.Color - De kleur voor een  ReplacementType.DrawBox  optie (genegeerd anders).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Stelt de kleur in voor een
ReplacementType.DrawBox
optie (genegeerd anders).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.awt.Color | De kleur voor een  ReplacementType.DrawBox  optie (genegeerd anders). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Haalt een array van filters op die met deze redactie moeten worden toegepast.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Een array van filters om toe te passen met deze redactie.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Stelt een array van filters in om toe te passen met deze redactie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Een array van filters om toe te passen met deze redactie. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Haalt een aangepaste redactiehandler op. Alleen ondersteund voor PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Stelt een aangepaste redactiehandler in. Alleen ondersteund voor PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Een instantie van [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)

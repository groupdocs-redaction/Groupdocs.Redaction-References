---
title: "ReplacementOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les options pour le remplacement du texte correspondant."
type: docs
weight: 31
url: /fr/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Représente les options pour le remplacement du texte correspondant.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Initialise une nouvelle instance de la classe ReplacementOptions avec le texte de remplacement comme option. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Initialise une nouvelle instance de la classe ReplacementOptions avec un rectangle coloré comme option. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getActionType()](#getActionType--) | Obtient l'action de remplacement : dessiner une boîte ou remplacer le texte. |
|
|  | [getReplacement()](#getReplacement--) | Obtient la valeur de remplacement textuel. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Définit la valeur de remplacement textuel. |
|
|  | [getBoxColor()](#getBoxColor--) | Obtient la couleur pour un |
ReplacementType.DrawBox
option (ignorée autrement).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Définit la couleur pour un |
ReplacementType.DrawBox
option (ignorée autrement).
|
|  | [getFilters()](#getFilters--) | Obtient un tableau de filtres à appliquer avec cette censure. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Définit un tableau de filtres à appliquer avec cette censure. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Obtient un gestionnaire de censure personnalisé. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Définit un gestionnaire de censure personnalisé. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Initialise une nouvelle instance de la classe ReplacementOptions avec le texte de remplacement comme option.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | remplacement | java.lang.String | Remplacement textuel |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Initialise une nouvelle instance de la classe ReplacementOptions avec un rectangle coloré comme option.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | couleur | java.awt.Color | Couleur du rectangle |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Obtient l'action de remplacement : dessiner une boîte ou remplacer le texte.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Obtient la valeur de remplacement textuel.


**Returns:**
java.lang.String - La valeur du remplacement textuel.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Définit la valeur de remplacement textuel.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | La valeur du remplacement textuel. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Obtient la couleur pour un
ReplacementType.DrawBox
option (ignorée autrement).


**Returns:**
java.awt.Color - La couleur pour un  ReplacementType.DrawBox  option (ignorée autrement).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Définit la couleur pour un
ReplacementType.DrawBox
option (ignorée autrement).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.awt.Color | La couleur pour un  ReplacementType.DrawBox  option (ignorée autrement). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Obtient un tableau de filtres à appliquer avec cette censure.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Un tableau de filtres à appliquer avec cette censure.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Définit un tableau de filtres à appliquer avec cette censure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Un tableau de filtres à appliquer avec cette censure. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Obtient un gestionnaire de censure personnalisé. Pris en charge uniquement pour PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Définit un gestionnaire de censure personnalisé. Pris en charge uniquement pour PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Une instance de [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)

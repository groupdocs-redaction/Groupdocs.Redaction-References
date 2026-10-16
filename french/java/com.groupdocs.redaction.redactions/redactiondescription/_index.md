---
title: "RedactionDescription"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les informations d'une action de modification unique effectuée pendant le processus de rédaction."
type: docs
weight: 25
url: /fr/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Représente les informations d'une action de modification unique effectuée pendant le processus de rédaction.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement d'image. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Obtient le type de données du document - texte, métadonnées ou annotations. |
|
|  | [getActionType()](#getActionType--) | Obtient l'opération de rédaction : remplacement, nettoyage ou suppression. |
|
|  | [getOriginalText()](#getOriginalText--) | Obtient le texte correspondant, si une expression est fournie. |
|
|  | [getReplacement()](#getReplacement--) | Obtient les informations de remplacement, peut être nul. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Obtient les informations de remplacement pour les rédactions de zones d'image, renvoie nul pour les rédactions textuelles. |
|
|  | [getDetails()](#getDetails--) | Obtient des informations détaillées optionnelles pour l'élément en cours de rédaction. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Définit des informations détaillées optionnelles pour l'élément en cours de rédaction. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Initialise une nouvelle instance de la classe RedactionDescription sans informations de remplacement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redactionType | int | Type de données en cours de rédaction |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action à effectuer sur ces données |
|
|  | originalText | java.lang.String | Texte correspondant, commentaire ou corps d'annotation |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redactionType | int | Type de données en cours de rédaction |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action à effectuer sur ces données |
|
|  | originalText | java.lang.String | Texte correspondant, commentaire ou corps d'annotation |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Texte de remplacement, texte correspondant et sa position dans la chaîne originale |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Initialise une nouvelle instance de la classe RedactionDescription avec des informations de remplacement d'image.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redactionType | int | Type de données en cours de rédaction |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Action à effectuer sur ces données |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Informations de remplacement de zone d'image |
|
|  | imageDetails | java.lang.String | Description textuelle de l'image, par défaut c'est String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Obtient le type de données du document - texte, métadonnées ou annotations.


**Returns:**
int - Le type de données du document - texte, métadonnées ou annotations.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Obtient l'opération de rédaction : remplacement, nettoyage ou suppression.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Obtient le texte correspondant, si une expression est fournie.


**Returns:**
java.lang.String - Le texte correspondant, si une expression est fournie.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Obtient les informations de remplacement, peut être nul.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Obtient les informations de remplacement pour les rédactions de zones d'image, renvoie nul pour les rédactions textuelles.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Obtient des informations détaillées optionnelles pour l'élément en cours de rédaction.


**Returns:**
java.lang.String - Des informations détaillées optionnelles pour l'élément en cours de rédaction.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Définit des informations détaillées optionnelles pour l'élément en cours de rédaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Des informations détaillées optionnelles pour l'élément en cours de rédaction. |
|


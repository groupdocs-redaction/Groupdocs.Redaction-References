---
title: "CustomRedactionContext"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit les données d'entrée pour ."
type: docs
weight: 13
url: /fr/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Fournit les données d'entrée pour [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Obtient le numéro de page du fragment correspondant, lorsqu'il est disponible. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Définit le numéro de page du fragment correspondant. |
|
|  | [getText()](#getText--) | Obtient le texte correspondant pour la rédaction. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Définit le texte correspondant pour la rédaction. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Obtient le numéro de page du fragment correspondant, lorsqu'il est disponible.


**Returns:**
int - Le numéro de page, ou une valeur spécifique au format si la page n'est pas connue.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Définit le numéro de page du fragment correspondant.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le numéro de page. |
|

### getText() {#getText--}
```
public final String getText()
```


Obtient le texte correspondant pour la rédaction.


**Returns:**
java.lang.String - Le texte correspondant.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Définit le texte correspondant pour la rédaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le texte correspondant. |
|


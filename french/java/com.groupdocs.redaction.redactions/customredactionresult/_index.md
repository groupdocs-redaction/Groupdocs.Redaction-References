---
title: "CustomRedactionResult"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un résultat retourné par ."
type: docs
weight: 14
url: /fr/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Représente un résultat retourné par [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getApply()](#getApply--) | Obtient une valeur indiquant si le remplacement doit être appliqué. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Définit une valeur indiquant si le remplacement doit être appliqué. |
|
|  | [getText()](#getText--) | Obtient le texte de remplacement utilisé lorsque #getApply().getApply() est |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Définit le texte de remplacement utilisé lorsque #getApply().getApply() est |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Obtient une valeur indiquant si le remplacement doit être appliqué.


**Returns:**
boolean -  true  pour remplacer le texte correspondant par #getText().getText(); sinon,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Définit une valeur indiquant si le remplacement doit être appliqué.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | true  pour appliquer le remplacement ; sinon,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Obtient le texte de remplacement utilisé lorsque #getApply().getApply() est
true
.


**Returns:**
java.lang.String - Le texte de remplacement.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Définit le texte de remplacement utilisé lorsque #getApply().getApply() est
true
.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le texte de remplacement. |
|


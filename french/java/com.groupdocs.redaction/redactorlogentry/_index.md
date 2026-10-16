---
title: "RedactorLogEntry"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente les résultats de l'application de la rédaction."
type: docs
weight: 18
url: /fr/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Représente les résultats de l'application de la rédaction.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Initialise une nouvelle instance de la classe RedactorLogEntry pour la rédaction. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getResult()](#getResult--) | Obtient le résultat, renvoyé par |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Obtient la référence à la rédaction et ses options. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Initialise une nouvelle instance de la classe RedactorLogEntry pour la rédaction.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Référence à la rédaction |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Résultat de la rédaction, signalé par le gestionnaire de format |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Obtient le résultat, renvoyé par
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Obtient la référence à la rédaction et ses options.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.


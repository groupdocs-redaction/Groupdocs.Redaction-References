---
title: "RedactionPolicy"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une politique de désinfection contenant un ensemble de rédactions spécifiques à appliquer."
type: docs
weight: 14
url: /fr/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Représente une politique de désinfection, contenant un ensemble de rédactions spécifiques à appliquer.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Crée une nouvelle instance de la politique de rédaction. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Crée une nouvelle instance de la politique de rédaction avec une liste spécifique de rédactions. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Obtient un tableau entièrement configuré |
Rédaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Charge une instance de |
RedactionPolicy
à partir d'un chemin de fichier.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Charge une instance de |
RedactionPolicy
à partir d'un flux.
|
|  | [save(String filePath)](#save-java.lang.String-) | Enregistre la politique de rédaction dans un fichier. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre la politique de rédaction dans un flux. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Crée une nouvelle instance de la politique de rédaction.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Crée une nouvelle instance de la politique de rédaction avec une liste spécifique de rédactions.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Un tableau de rédactions pour la politique |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Obtient un tableau entièrement configuré
Rédaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Un tableau de classes dérivées de Redaction entièrement configurées.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Charge une instance de
RedactionPolicy
à partir d'un chemin de fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin du fichier XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Charge une instance de
RedactionPolicy
à partir d'un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | entrée | java.io.InputStream | Flux contenant la configuration XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Enregistre la politique de rédaction dans un fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin du fichier. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Enregistre la politique de rédaction dans un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | Flux cible pour enregistrer la politique |
|


---
title: "SaveOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit des options pour changer le nom du fichier de sortie et/ou convertir le document en rasterisation PDF basée sur l'image."
type: docs
weight: 14
url: /fr/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur des images (rasterisation).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Initialise une nouvelle instance avec les valeurs par défaut : rasteriser en PDF - false, ajouter le suffixe - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Initialise une nouvelle instance avec les paramètres fournis. |
|
## Champs

| Champ | Description |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Représente la valeur de suffixe par défaut, qui est \"Redacted\". |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Obtient une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Définit une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Obtient un suffixe personnalisé pour le nom de fichier de sortie. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Définit un suffixe personnalisé pour le nom de fichier de sortie. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Obtient une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
|
|  | [getRasterization()](#getRasterization--) | Obtient les paramètres de rasterisation. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Options d'enregistrement du traitement de texte. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Initialise une nouvelle instance avec les valeurs par défaut : rasteriser en PDF - false, ajouter le suffixe - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Initialise une nouvelle instance avec les paramètres fournis.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | Vrai, si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF |
|
|  | suffix | java.lang.String | Ce texte sera ajouté à la fin du nom de fichier, s'il n'est pas vide il définit également AddSuffix sur true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Représente la valeur de suffixe par défaut, qui est \"Redacted\".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Obtient une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. False par défaut.


**Returns:**
boolean - Une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. False par défaut.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Définit une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. False par défaut.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. False par défaut. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Obtient un suffixe personnalisé pour le nom de fichier de sortie. S'il n'est pas spécifié, le
SaveSuffix
constante sera utilisée.


**Returns:**
java.lang.String - Un suffixe personnalisé pour le nom de fichier de sortie. S'il n'est pas spécifié, la constante SaveSuffix sera utilisée.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Définit un suffixe personnalisé pour le nom de fichier de sortie. S'il n'est pas spécifié, le
SaveSuffix
constante sera utilisée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Un suffixe personnalisé pour le nom du fichier de sortie. S'il n'est pas spécifié, la constante SaveSuffix sera utilisée. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Obtient une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF.


**Returns:**
booléen - Une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Obtient les paramètres de rasterisation.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Options d'enregistrement du traitement de texte.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)

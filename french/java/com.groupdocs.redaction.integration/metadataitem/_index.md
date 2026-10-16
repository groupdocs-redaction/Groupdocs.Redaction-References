---
title: "MetadataItem"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un élément de métadonnées commun à tous les formats pris en charge et utilisé dans les rédactions de métadonnées."
type: docs
weight: 12
url: /fr/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Représente un élément de métadonnées, commun à tous les formats pris en charge et utilisé dans les suppressions de métadonnées.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Initialise une nouvelle instance. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Obtient le nom original de l'élément de métadonnées, tel qu'il apparaît dans le document. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Définit le nom original de l'élément de métadonnées, tel qu'il apparaît dans le document. |
|
|  | [getCategory()](#getCategory--) | Obtient la catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource incorporée. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Définit une catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource intégrée. |
|
|  | [getFilter()](#getFilter--) | Obtient une valeur de |
MetadataFilters
, attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments.
|
|  | [setFilter(int value)](#setFilter-int-) | Définit une valeur de |
MetadataFilters
, attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments.
|
|  | [getValues()](#getValues--) | Obtient la valeur de l'élément de métadonnées. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Définit la valeur de l'élément de métadonnées. |
|
|  | [isCustom()](#isCustom--) | Obtient une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Définit une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Obtient une clé de dictionnaire pour , en utilisant son OriginalName et d'autres données. |
|
|  | [createClone()](#createClone--) | Crée une copie profonde de l'instance actuelle. |
|
|  | [getActualValue()](#getActualValue--) | Obtient la représentation sous forme de chaîne de la valeur de l'élément de métadonnées. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Initialise une nouvelle instance.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Obtient le nom original de l'élément de métadonnées, tel qu'il apparaît dans le document.


**Returns:**
java.lang.String - Un nom original de l'élément de métadonnées, tel qu'il apparaît dans le document.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Définit le nom original de l'élément de métadonnées, tel qu'il apparaît dans le document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Un nom original de l'élément de métadonnées, tel qu'il apparaît dans le document. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Obtient la catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource incorporée.


**Returns:**
java.lang.String - Une catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource intégrée.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Définit une catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource intégrée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Une catégorie de l'élément de métadonnées, par exemple l'ID de ressource pour un élément de métadonnées de ressource intégrée. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Obtient une valeur de
MetadataFilters
, attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments.


**Returns:**
int - Une valeur de  MetadataFilters , attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Définit une valeur de
MetadataFilters
, attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Une valeur de  MetadataFilters , attribuée à cet élément de métadonnées qui est utilisé dans le filtrage des éléments. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Obtient la valeur de l'élément de métadonnées.


**Returns:**
java.util.List<java.lang.String> - La valeur de l'élément de métadonnées.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Définit la valeur de l'élément de métadonnées.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.util.List<java.lang.String> | La valeur de l'élément de métadonnées. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Obtient une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document).


**Returns:**
boolean - Une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Définit une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document).


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si cet élément est personnalisé (ajouté par les auteurs du document). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Obtient une clé de dictionnaire pour , en utilisant son OriginalName et d'autres données.


**Returns:**
java.lang.String - Une clé de dictionnaire pour , en utilisant son OriginalName et d'autres données.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Crée une copie profonde de l'instance actuelle.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Obtient la représentation sous forme de chaîne de la valeur de l'élément de métadonnées.


**Returns:**
java.lang.String - La représentation sous forme de chaîne de la valeur de l'élément de métadonnées.


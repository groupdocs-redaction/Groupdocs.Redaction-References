---
title: "MetadataItem"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een metadata-item voor dat algemeen is voor alle ondersteunde formaten en wordt gebruikt bij metadata-redacties."
type: docs
weight: 12
url: /nl/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Stelt een metadata-item voor, gemeenschappelijk voor alle ondersteunde formaten en gebruikt bij metadata-redacties.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Initialiseert een nieuw exemplaar. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Haalt de oorspronkelijke naam van het metadata-item op, zoals deze in het document voorkomt. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Stelt de oorspronkelijke naam van het metadata-item in, zoals deze in het document voorkomt. |
|
|  | [getCategory()](#getCategory--) | Haalt een categorie van het metadata-item op, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Stelt een categorie van het metadata-item in, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item. |
|
|  | [getFilter()](#getFilter--) | Haalt een waarde op van |
MetadataFilters
, toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie.
|
|  | [setFilter(int value)](#setFilter-int-) | Stelt een waarde in van |
MetadataFilters
, toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie.
|
|  | [getValues()](#getValues--) | Haalt de waarde van het metadata-item op. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Stelt de waarde van het metadata-item in. |
|
|  | [isCustom()](#isCustom--) | Haalt een waarde op die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Stelt een waarde in die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Haalt een woordenboek‑sleutel op voor , met gebruik van de OriginalName en andere gegevens. |
|
|  | [createClone()](#createClone--) | Maakt een diepe kloon van de huidige instantie. |
|
|  | [getActualValue()](#getActualValue--) | Haalt de tekenreeksrepresentatie van de waarde van het metadata-item op. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Initialiseert een nieuw exemplaar.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Haalt de oorspronkelijke naam van het metadata-item op, zoals deze in het document voorkomt.


**Returns:**
java.lang.String - Een originele naam van het metadata-item, zoals het in het document voorkomt.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Stelt de oorspronkelijke naam van het metadata-item in, zoals deze in het document voorkomt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Een originele naam van het metadata-item, zoals het in het document voorkomt. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Haalt een categorie van het metadata-item op, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item.


**Returns:**
java.lang.String - Een categorie van het metadata-item, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Stelt een categorie van het metadata-item in, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Een categorie van het metadata-item, bijvoorbeeld resource-ID voor een ingebed resource-metadata-item. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Haalt een waarde op van
MetadataFilters
, toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie.


**Returns:**
int - Een waarde van  MetadataFilters , toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Stelt een waarde in van
MetadataFilters
, toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Een waarde van  MetadataFilters , toegewezen aan dit metadata-item die wordt gebruikt bij itemfiltratie. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Haalt de waarde van het metadata-item op.


**Returns:**
java.util.List<java.lang.String> - De waarde van het metadata-item.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Stelt de waarde van het metadata-item in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.util.List<java.lang.String> | De waarde van het metadata-item. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Haalt een waarde op die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document).


**Returns:**
boolean - Een waarde die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Stelt een waarde in die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of dit item aangepast is (toegevoegd door de auteurs van het document). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Haalt een woordenboek‑sleutel op voor , met gebruik van de OriginalName en andere gegevens.


**Returns:**
java.lang.String - Een woordenboek‑sleutel voor , met gebruik van de OriginalName en andere gegevens.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Maakt een diepe kloon van de huidige instantie.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Haalt de tekenreeksrepresentatie van de waarde van het metadata-item op.


**Returns:**
java.lang.String - De tekenreeksrepresentatie van de waarde van het metadata-item.


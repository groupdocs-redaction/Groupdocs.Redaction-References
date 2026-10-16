---
title: "MetadataItem"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar ett metadataobjekt som är gemensamt för alla stödda format och används i metadata-redigeringar."
type: docs
weight: 12
url: /sv/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Representerar ett metadataobjekt, gemensamt för alla stödda format och som används i metadata‑redigeringar.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Initierar en ny instans. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Hämtar det ursprungliga namnet på metadataobjektet, så som det visas i dokumentet. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Ställer in det ursprungliga namnet på metadataobjektet, så som det visas i dokumentet. |
|
|  | [getCategory()](#getCategory--) | Hämtar en kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Ställer in en kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt. |
|
|  | [getFilter()](#getFilter--) | Hämtar ett värde av |
MetadataFilters
, tilldelad detta metadataobjekt som används i objektfiltrering.
|
|  | [setFilter(int value)](#setFilter-int-) | Ställer in ett värde av |
MetadataFilters
, tilldelad detta metadataobjekt som används i objektfiltrering.
|
|  | [getValues()](#getValues--) | Hämtar metadataobjektets värde. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Ställer in metadataobjektets värde. |
|
|  | [isCustom()](#isCustom--) | Hämtar ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Ställer in ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Hämtar en ordboksnyckel för , med dess OriginalName och annan data. |
|
|  | [createClone()](#createClone--) | Skapar en djup klon av den aktuella instansen. |
|
|  | [getActualValue()](#getActualValue--) | Hämtar strängrepresentationen av metadataobjektets värde. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Initierar en ny instans.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Hämtar det ursprungliga namnet på metadataobjektet, så som det visas i dokumentet.


**Returns:**
java.lang.String - Ett originalnamn för metadataobjektet, så som det visas i dokumentet.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Ställer in det ursprungliga namnet på metadataobjektet, så som det visas i dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Ett originalnamn för metadataobjektet, så som det visas i dokumentet. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Hämtar en kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt.


**Returns:**
java.lang.String - En kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Ställer in en kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | En kategori för metadataobjektet, till exempel resurs-ID för ett inbäddat resursmetadataobjekt. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Hämtar ett värde av
MetadataFilters
, tilldelad detta metadataobjekt som används i objektfiltrering.


**Returns:**
int - Ett värde av  MetadataFilters , tilldelat detta metadataobjekt som används i objektfiltrering.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Ställer in ett värde av
MetadataFilters
, tilldelad detta metadataobjekt som används i objektfiltrering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Ett värde av  MetadataFilters , tilldelat detta metadataobjekt som används i objektfiltrering. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Hämtar metadataobjektets värde.


**Returns:**
java.util.List<java.lang.String> - Metadataobjektets värde.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Ställer in metadataobjektets värde.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.util.List<java.lang.String> | Metadataobjektets värde. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Hämtar ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare).


**Returns:**
boolean - Ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Ställer in ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om detta objekt är anpassat (tillagt av dokumentets författare). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Hämtar en ordboksnyckel för , med dess OriginalName och annan data.


**Returns:**
java.lang.String - En ordboksnyckel för , med dess OriginalName och annan data.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Skapar en djup klon av den aktuella instansen.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Hämtar strängrepresentationen av metadataobjektets värde.


**Returns:**
java.lang.String - Strängrepresentationen av metadataobjektets värde.


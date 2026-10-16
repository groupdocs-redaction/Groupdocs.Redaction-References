---
title: "MetadataItem"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет элемент метаданных, общий для всех поддерживаемых форматов и используемый в редактировании метаданных."
type: docs
weight: 12
url: /ru/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Представляет элемент метаданных, общий для всех поддерживаемых форматов и используемый при редактировании метаданных.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Инициализирует новый экземпляр. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Получает оригинальное имя элемента метаданных, как оно указано в документе. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Устанавливает оригинальное имя элемента метаданных, как оно указано в документе. |
|
|  | [getCategory()](#getCategory--) | Получает категорию элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Устанавливает категорию элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса. |
|
|  | [getFilter()](#getFilter--) | Получает значение |
MetadataFilters
, назначенное этому элементу метаданных, которое используется при фильтрации элементов.
|
|  | [setFilter(int value)](#setFilter-int-) | Устанавливает значение |
MetadataFilters
, назначенное этому элементу метаданных, которое используется при фильтрации элементов.
|
|  | [getValues()](#getValues--) | Получает значение элемента метаданных. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Устанавливает значение элемента метаданных. |
|
|  | [isCustom()](#isCustom--) | Получает значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Устанавливает значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Получает ключ словаря для , используя его OriginalName и другие данные. |
|
|  | [createClone()](#createClone--) | Создаёт глубокую копию текущего экземпляра. |
|
|  | [getActualValue()](#getActualValue--) | Получает строковое представление значения элемента метаданных. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Инициализирует новый экземпляр.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Получает оригинальное имя элемента метаданных, как оно указано в документе.


**Returns:**
java.lang.String — Исходное имя элемента метаданных, как оно отображается в документе.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Устанавливает оригинальное имя элемента метаданных, как оно указано в документе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Исходное имя элемента метаданных, как оно отображается в документе. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Получает категорию элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса.


**Returns:**
java.lang.String — Категория элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Устанавливает категорию элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Категория элемента метаданных, например идентификатор ресурса для встроенного элемента метаданных ресурса. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Получает значение
MetadataFilters
, назначенное этому элементу метаданных, которое используется при фильтрации элементов.


**Returns:**
int — Значение  MetadataFilters , назначенное этому элементу метаданных, которое используется при фильтрации элементов.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Устанавливает значение
MetadataFilters
, назначенное этому элементу метаданных, которое используется при фильтрации элементов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Значение  MetadataFilters , назначенное этому элементу метаданных, которое используется при фильтрации элементов. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Получает значение элемента метаданных.


**Returns:**
java.util.List<java.lang.String> — Значение элемента метаданных.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Устанавливает значение элемента метаданных.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.util.List<java.lang.String> | Значение элемента метаданных. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Получает значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа).


**Returns:**
boolean — Значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Устанавливает значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, является ли этот элемент пользовательским (добавленным авторами документа). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Получает ключ словаря для , используя его OriginalName и другие данные.


**Returns:**
java.lang.String — Ключ словаря для , используя его OriginalName и другие данные.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Создаёт глубокую копию текущего экземпляра.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Получает строковое представление значения элемента метаданных.


**Returns:**
java.lang.String — Строковое представление значения элемента метаданных.


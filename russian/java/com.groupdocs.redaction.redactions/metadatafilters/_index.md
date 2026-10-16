---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет список наиболее распространённых типов метаданных документа."
type: docs
weight: 19
url: /ru/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Представляет список наиболее распространённых типов метаданных документа.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Поля

| Поле | Описание |
| --- | --- |
|  | [None](#None) | Пустая настройка фильтра, не соответствует ни одному элементу метаданных. |
|
|  | [Author](#Author) | Автор документа. |
|
|  | [Category](#Category) | Категория документа. |
|
|  | [Comments](#Comments) | Комментарий к документу. |
|
|  | [Company](#Company) | Компания автора. |
|
|  | [ContentStatus](#ContentStatus) | Состояние содержимого. |
|
|  | [CreatedTime](#CreatedTime) | Время создания. |
|
|  | [HyperlinkBase](#HyperlinkBase) | База гиперссылки. |
|
|  | [LastPrinted](#LastPrinted) | Дата и время последней печати. |
|
|  | [LastSavedBy](#LastSavedBy) | Последнее сохранение пользователем. |
|
|  | [LastSavedTime](#LastSavedTime) | Дата и время последнего сохранения. |
|
|  | [NameOfApplication](#NameOfApplication) | Название приложения, в котором был создан документ. |
|
|  | [Manager](#Manager) | Имя руководителя автора. |
|
|  | [RevisionNumber](#RevisionNumber) | Номер ревизии. |
|
|  | [Subject](#Subject) | Тема документа. |
|
|  | [Template](#Template) | Название шаблона документа. |
|
|  | [Title](#Title) | Заголовок документа. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Общее время редактирования. |
|
|  | [Version](#Version) | Версия документа. |
|
|  | [Description](#Description) | Описание документа. |
|
|  | [Keywords](#Keywords) | Ключевые слова документа. |
|
|  | [ContentType](#ContentType) | Тип содержимого. |
|
|  | [All](#All) | Все типы элементов метаданных. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getNames()](#getNames--) | Получает набор со всеми объявленными типами фильтров. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Получает значение MetadataFiler по его имени. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Разбирает строку со значениями MetadataFilers, разделёнными запятыми, в целое число. |
|
|  | [toString(int value)](#toString-int-) | Сохраняет целое число как строку со значениями MetadataFilers, разделёнными запятыми. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Пустая настройка фильтра, не соответствует ни одному элементу метаданных.


### Author {#Author}
```
public static final int Author
```


Автор документа.


### Category {#Category}
```
public static final int Category
```


Категория документа.


### Comments {#Comments}
```
public static final int Comments
```


Комментарий к документу.


### Company {#Company}
```
public static final int Company
```


Компания автора.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Состояние содержимого.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Время создания.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


База гиперссылки.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Дата и время последней печати.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Последнее сохранение пользователем.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Дата и время последнего сохранения.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Название приложения, в котором был создан документ.


### Manager {#Manager}
```
public static final int Manager
```


Имя руководителя автора.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Номер ревизии.


### Subject {#Subject}
```
public static final int Subject
```


Тема документа.


### Template {#Template}
```
public static final int Template
```


Название шаблона документа.


### Title {#Title}
```
public static final int Title
```


Заголовок документа.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Общее время редактирования.


### Version {#Version}
```
public static final int Version
```


Версия документа.


### Description {#Description}
```
public static final int Description
```


Описание документа.


### Keywords {#Keywords}
```
public static final int Keywords
```


Ключевые слова документа.


### ContentType {#ContentType}
```
public static final int ContentType
```


Тип содержимого.


### All {#All}
```
public static final int All
```


Все типы элементов метаданных.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Получает набор со всеми объявленными типами фильтров.


**Returns:**
java.util.Set<java.lang.String> - Набор со всеми объявленными типами фильтров.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Получает значение MetadataFiler по его имени.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | valueName | java.lang.String | Имя MetadataFilter. |
|

**Returns:**
int - Значение MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Разбирает строку со значениями MetadataFilers, разделёнными запятыми, в целое число.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | values | java.lang.String | Строка со значениями MetadataFilers, разделёнными запятыми. |
|

**Returns:**
int - Значение MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Сохраняет целое число как строку со значениями MetadataFilers, разделёнными запятыми.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Значение MetadataFiler. |
|

**Returns:**
java.lang.String - Строка со значениями MetadataFiler, разделёнными запятыми.


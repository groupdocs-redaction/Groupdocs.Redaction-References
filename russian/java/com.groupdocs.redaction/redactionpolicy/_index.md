---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет политику санитизации, содержащую набор конкретных редактирований для применения."
type: docs
weight: 14
url: /ru/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Представляет политику очистки, содержащую набор конкретных редактирований для применения.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Создает новый экземпляр политики Redaction. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Создает новый экземпляр политики Redaction со специфическим списком редактирований. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Получает массив полностью настроенных |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Загружает экземпляр |
RedactionPolicy
из пути к файлу.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Загружает экземпляр |
RedactionPolicy
из потока.
|
|  | [save(String filePath)](#save-java.lang.String-) | Сохраняет политику редактирования в файл. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет политику редактирования в поток. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Создает новый экземпляр политики Redaction.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Создает новый экземпляр политики Redaction со специфическим списком редактирований.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Массив редактирований для политики |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Получает массив полностью настроенных
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Массив полностью настроенных классов, производных от Redaction.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Загружает экземпляр
RedactionPolicy
из пути к файлу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к XML‑файлу |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Загружает экземпляр
RedactionPolicy
из потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | input | java.io.InputStream | Поток, содержащий XML‑конфигурацию |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Сохраняет политику редактирования в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Сохраняет политику редактирования в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | Целевой поток для сохранения политики |
|


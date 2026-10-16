---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет результаты списка редактирований, переданных методу Apply класса Redactor."
type: docs
weight: 17
url: /ru/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Представляет результаты списка редактирований, переданных методу Apply() класса
Redactor
класс.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Инициализирует новый экземпляр класса RedactorChangeLog. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getStatus()](#getStatus--) | Получает окончательный статус всех применённых редактирований. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Получает список |
RedactorLogEntry
экземпляры.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Инициализирует новый экземпляр класса RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Получает окончательный статус всех применённых редактирований.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Получает список
RedactorLogEntry
экземпляры.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - Список экземпляров RedactorLogEntry.


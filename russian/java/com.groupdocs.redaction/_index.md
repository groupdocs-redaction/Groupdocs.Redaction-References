---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Пакет предоставляет классы для редактирования конфиденциальной информации в документах форматов PDF, растровых изображений и офисных документов."
type: docs
weight: 10
url: /ru/java/com.groupdocs.redaction/
---

Пакет предоставляет классы для замазывания конфиденциальной информации из документов в форматах PDF, растровых изображений и офисных документов.

Основные классы в этом пакете:

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## Классы

| Класс | Описание |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Представляет информацию о документе. |
| [FileType](../com.groupdocs.redaction/filetype) | Представляет тип файла. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Представляет краткую информацию о странице. |
| [Redaction](../com.groupdocs.redaction/redaction) | Представляет базовый абстрактный класс для всех типов редактирования. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Представляет политику очистки, содержащую набор конкретных редактирований для применения. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Представляет результат операции редактирования. |
| [Redactor](../com.groupdocs.redaction/redactor) | Представляет основной класс, который контролирует процесс редактирования документа, позволяя открывать, редактировать и сохранять документы. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Представляет результаты списка редактирований, передаваемых методу Apply() класса Redactor. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Представляет результаты применения редактирования. |

## Интерфейсы

| Интерфейс | Описание |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Определяет методы, необходимые для получения базовой информации о документе. |

## Перечисления

| Перечисление | Описание |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Представляет статус завершения редактирования. |

---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Paketet tillhandahåller klasser för att redigera känslig information från dokument i PDF‑rasterbilds- och kontorsdokumentformat."
type: docs
weight: 10
url: /sv/java/com.groupdocs.redaction/
---

Paketet tillhandahåller klasser för att rensa känslig information från dokument i PDF-, rasterbild- och kontorsdokumentformat.

De viktigaste klasserna i detta paket är:

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## Klasser

| Klass | Beskrivning |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Representerar information om ett dokument. |
| [FileType](../com.groupdocs.redaction/filetype) | Representerar en filtyp. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Representerar en kort sidinformation. |
| [Redaction](../com.groupdocs.redaction/redaction) | Representerar en grundläggande abstrakt klass för alla raderingsklasser. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Representerar en saneringspolicy som innehåller en uppsättning specifika raderingar att tillämpa. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Representerar ett resultat av raderingsoperationen. |
| [Redactor](../com.groupdocs.redaction/redactor) | Representerar en huvudklass som kontrollerar dokumentraderingsprocessen och möjliggör att öppna, radera och spara dokument. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Representerar resultat för en lista med raderingar som skickas till Apply()-metoden i Redactor-klassen. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Representerar resultat av att tillämpa radering. |

## Gränssnitt

| Gränssnitt | Beskrivning |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Definierar metoder som krävs för att hämta grundläggande dokumentinformation. |

## Enumerationer

| Enum | Beskrivning |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Representerar en raderingsslutförandestatus. |

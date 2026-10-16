---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Il pacchetto fornisce classi per redigere informazioni sensibili da documenti in formati PDF, immagine raster e documenti Office."
type: docs
weight: 10
url: /it/java/com.groupdocs.redaction/
---

Il pacchetto fornisce classi per la redazione di informazioni sensibili dai documenti in formati PDF, immagine raster e documenti Office.

Le classi principali in questo pacchetto sono:

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## Classi

| Classe | Descrizione |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Rappresenta un'informazione sul documento. |
| [FileType](../com.groupdocs.redaction/filetype) | Rappresenta un tipo di file. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Rappresenta una breve informazione di pagina. |
| [Redaction](../com.groupdocs.redaction/redaction) | Rappresenta una classe astratta di base per tutti i tipi di redazione. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Rappresenta una politica di sanificazione, contenente un insieme di redazioni specifiche da applicare. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Rappresenta un risultato dell'operazione di redazione. |
| [Redactor](../com.groupdocs.redaction/redactor) | Rappresenta la classe principale che controlla il processo di redazione dei documenti, consentendo di aprire, redigere e salvare i documenti. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Rappresenta i risultati per un elenco di redazioni, passati al metodo Apply() della classe Redactor. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Rappresenta i risultati dell'applicazione della redazione. |

## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Definisce i metodi necessari per ottenere le informazioni di base del documento. |

## Enumerazioni

| Enum | Descrizione |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Rappresenta lo stato di completamento della redazione. |

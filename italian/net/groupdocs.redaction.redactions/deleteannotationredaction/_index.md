---
title: "DeleteAnnotationRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione del testo che elimina le annotazioni se il testo corrisponde a una determinata espressione regolare, opzionalmente elimina tutte le annotazioni."
type: docs
weight: 580
url: /it/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Rappresenta una redazione di testo che elimina le annotazioni se il testo corrisponde a una determinata espressione regolare (opzionalmente elimina tutte le annotazioni).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, con impostazioni per eliminare tutte le annotazioni (corrispondenti a tutto). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Inizializza una nuova istanza della classe DeleteAnnotationRedaction, eliminando le annotazioni che corrispondono all'espressione fornita. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Ottiene l'espressione regolare da corrispondere. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Esempi

Il seguente esempio dimostra come rimuovere tutte le annotazioni contenenti le parole "use", "show" o "describe" dal documento (e lasciare le altre).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->

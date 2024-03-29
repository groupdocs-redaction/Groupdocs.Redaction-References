---
title: AnnotationRedaction
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Rappresenta una redazione che sostituisce il testo dellannotazione commenti ecc. corrispondente a una determinata espressione regolare.
type: docs
weight: 440
url: /it/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Rappresenta una redazione che sostituisce il testo dell'annotazione (commenti, ecc.) corrispondente a una determinata espressione regolare.

```csharp
public class AnnotationRedaction : Redaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Inizializza una nuova istanza della classe AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Inizializza una nuova istanza della classe AnnotationRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Ottiene l'espressione regolare per la corrispondenza. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Ottiene una sostituzione testuale per il testo corrispondente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una data istanza di formato. |

### Osservazioni

**Saperne di più**

* Maggiori dettagli sull'applicazione delle redazioni: [Nozioni di base sulla redazione](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Maggiori dettagli sulla redazione delle annotazioni del documento: [Redazioni di annotazioni](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Esempi

L'esempio seguente mostra come sostituire il nome "John" con "[redatto]" in tutte le annotazioni.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Guarda anche

* class [Redaction](../../groupdocs.redaction/redaction)
* spazio dei nomi [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

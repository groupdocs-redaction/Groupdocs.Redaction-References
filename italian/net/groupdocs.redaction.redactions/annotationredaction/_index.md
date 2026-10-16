---
title: "AnnotationRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione che sostituisce testo, commenti, ecc. delle annotazioni che corrispondono a una determinata espressione regolare."
type: docs
weight: 530
url: /it/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Rappresenta una redazione che sostituisce il testo delle annotazioni (commenti, ecc.) che corrisponde a una determinata espressione regolare.

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
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Ottiene l'espressione regolare da corrispondere. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Ottiene una sostituzione testuale per il testo corrispondente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Esempi

Il seguente esempio dimostra come sostituire il nome "John" con "[redacted]" in tutte le annotazioni.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->

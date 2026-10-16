---
title: "RemovePageRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione che rimuove una pagina, diapositiva, foglio di lavoro, ecc. da un documento."
type: docs
weight: 770
url: /it/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Rappresenta una redazione che rimuove una pagina (diapositiva, foglio di lavoro, ecc.) da un documento.

```csharp
public class RemovePageRedaction : Redaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Inizializza una nuova istanza della classe RemovePageRedaction. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Restituisce il conteggio delle pagine da rimuovere. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Restituisce l'indice della posizione di inizio (basato su zero). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Restituisce la posizione di riferimento per la ricerca, l'inizio o la fine di un documento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Esempi

Il seguente esempio dimostra come rimuovere l'ultima pagina del documento.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->

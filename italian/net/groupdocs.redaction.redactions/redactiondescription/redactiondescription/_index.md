---
title: "RedactionDescription"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| redactionType | RedactionType | Tipo di dati da redigere |
| actionType | RedactionActionType | Azione da eseguire su questi dati |
| originalText | String | Testo corrispondente, commento o corpo dell'annotazione |

### Vedi anche

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| redactionType | RedactionType | Tipo di dati da redigere |
| actionType | RedactionActionType | Azione da eseguire su questi dati |
| originalText | String | Testo corrispondente, commento o corpo dell'annotazione |
| sostituzione | TextReplacement | Testo di sostituzione, testo corrispondente e la sua posizione all'interno della stringa originale |

### Vedi anche

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione dell'area immagine.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| redactionType | RedactionType | Tipo di dati da redigere |
| actionType | RedactionActionType | Azione da eseguire su questi dati |
| imageAreaReplacement | RegionReplacementOptions | Informazioni sulla sostituzione dell'area immagine |
| imageDetails | String | Descrizione testuale dell'immagine, per impostazione predefinita è String.Empty |

### Vedi anche

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->

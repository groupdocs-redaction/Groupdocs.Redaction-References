---
title: "PreviewOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Inizializza una nuova istanza della classe PreviewOptions facendo chiudere lo stream di output."
type: docs
weight: 10
url: /it/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

Inizializza una nuova istanza della classe PreviewOptions, facendo chiudere lo stream di output.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crea un flusso per l'anteprima di una pagina specifica |

### Vedi anche

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Inizializza una nuova istanza della classe PreviewOptions, facendo restituire lo stream di output al client per un uso successivo.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crea un flusso per l'anteprima di una pagina specifica |
| releasePageStream | ReleasePageStream | Notifica che la generazione dell'anteprima della pagina è completata e ottiene il flusso di output |

### Vedi anche

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->

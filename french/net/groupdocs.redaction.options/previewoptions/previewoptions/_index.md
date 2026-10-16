---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Initialise une nouvelle instance de la classe PreviewOptions provoquant la fermeture du flux de sortie."
type: docs
weight: 10
url: /fr/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

Initialise une nouvelle instance de la classe PreviewOptions, entraînant la fermeture du flux de sortie.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crée un flux pour un aperçu de page spécifique |

### Voir aussi

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Initialise une nouvelle instance de la classe PreviewOptions, entraînant le renvoi du flux de sortie au client pour une utilisation ultérieure.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| createPageStream | CreatePageStream | Crée un flux pour un aperçu de page spécifique |
| releasePageStream | ReleasePageStream | Signale que la génération de l'aperçu de la page est terminée et récupère le flux de sortie |

### Voir aussi

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->

---
title: "Enregistrer"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Enregistre le document dans un fichier avec les options suivantes AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /fr/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Enregistre le document dans un fichier avec les options suivantes : AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Valeur de retour

Chemin du document censuré

### Voir aussi

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Enregistre le document dans un fichier.

```csharp
public string Save(SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveOptions | SaveOptions | Options pour ajouter un suffixe ou rasteriser |

### Valeur de retour

Chemin du document censuré

### Exemples

L'exemple suivant montre comment enregistrer un document en utilisant SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // La rédaction du document se trouve ici
       // ...
    
       // Enregistrez le document avec les options par défaut (convertir les pages en images, enregistrer en PDF)
       redactor.Save();
    
       // Enregistrez le document dans son format d'origine en écrasant le fichier original
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Enregistrez le document sous le fichier "*_Redacted.*" dans son format d'origine
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Enregistrez le document sous "*_AnyText.*" (par ex. horodatage au lieu de "AnyText") dans son nom de fichier sans rasterisation
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Voir aussi

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Enregistre le document dans le flux spécifié.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| document | Stream | Le flux cible. |
| saveOptions | SaveOptions | Les options d'enregistrement qui contrôlent la rasterisation, le suffixe du nom de fichier de sortie et les paramètres d'enregistrement spécifiques au document. |

### Voir aussi

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->

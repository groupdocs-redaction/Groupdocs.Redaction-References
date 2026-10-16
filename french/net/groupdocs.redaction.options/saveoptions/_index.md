---
title: "SaveOptions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en rasterisation PDF basée sur l'image."
type: docs
weight: 450
url: /fr/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur des images (rasterisation).

```csharp
public class SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Initialise une nouvelle instance avec les valeurs par défaut : rasteriser en PDF - false, ajouter le suffixe - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Initialise une nouvelle instance avec les paramètres fournis. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Obtient ou définit une valeur indiquant si le nom de fichier doit être modifié avant l'enregistrement. False par défaut. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Obtient les paramètres de rasterisation. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Obtient ou définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Obtient ou définit un suffixe personnalisé pour le nom du fichier de sortie. S'il n'est pas spécifié, la constante [`SaveSuffix`](./savesuffix) sera utilisée. |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Obtient les options d'enregistrement spécifiques aux documents de traitement de texte. |

## Champs

| Nom | Description |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Représente la valeur de suffixe par défaut, qui est "Redacted". |

### Remarques

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->

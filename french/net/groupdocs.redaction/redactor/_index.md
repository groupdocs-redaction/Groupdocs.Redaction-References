---
title: "Redactor"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente la classe principale qui contrôle le processus de rédaction de documents, permettant d’ouvrir, de rédiger et d’enregistrer des documents."
type: docs
weight: 820
url: /fr/net/groupdocs.redaction/redactor/
---
## Redactor class

Représente la classe principale qui contrôle le processus de rédaction de documents, permettant d'ouvrir, de rédiger et d'enregistrer des documents.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) en utilisant un flux. |
| [Redactor](redactor#constructor_3)(string) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) en utilisant un chemin de fichier. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) pour un document protégé par mot de passe en utilisant un flux. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) pour un document protégé par mot de passe en utilisant son chemin. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) pour un document protégé par mot de passe en utilisant un flux et des paramètres. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialise une nouvelle instance de la classe [`Redactor`](../redactor) pour un document protégé par mot de passe en utilisant son chemin et des paramètres. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Applique une censure au document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Applique une politique de censure au document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Applique un ensemble de censures au document. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Libère les ressources. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Génère des images d'aperçu de pages spécifiques dans un format d'image donné. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Obtient les informations générales sur le document – taille, nombre de pages, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Enregistre le document dans un fichier avec les options suivantes : AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Enregistre le document dans un fichier. |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | Enregistre le document dans le flux spécifié. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Exemples

L'exemple suivant montre l'application d'une seule censure au document.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

L'exemple suivant montre l'application d'une liste de censures au document.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... autres censures
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false, si au moins une censure a échoué
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

L'exemple suivant montre comment appliquer une politique de rédaction à tous les fichiers d'un dossier d'entrée donné, et enregistrer dans l'un des dossiers de sortie – pour les fichiers mis à jour avec succès et pour ceux qui ont échoué.

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

L'exemple suivant montre comment ouvrir des documents protégés par mot de passe en utilisant LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici nous pouvons utiliser l'instance du document pour effectuer des censures
}
```

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

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->

---
title: Redactor
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une classe principale qui contrôle le processus de rédaction de documents permettant douvrir de rédiger et denregistrer des documents.
type: docs
weight: 660
url: /fr/net/groupdocs.redaction/redactor/
---
## Redactor class

Représente une classe principale qui contrôle le processus de rédaction de documents, permettant d'ouvrir, de rédiger et d'enregistrer des documents.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initialise une nouvelle instance de[`Redactor`](../redactor) classe utilisant stream. |
| [Redactor](redactor#constructor_3)(string) | Initialise une nouvelle instance de[`Redactor`](../redactor) classe utilisant le chemin du fichier. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initialise une nouvelle instance de[`Redactor`](../redactor) classe pour un document protégé par mot de passe utilisant stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initialise une nouvelle instance de[`Redactor`](../redactor) classe pour un document protégé par mot de passe en utilisant son chemin. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initialise une nouvelle instance de[`Redactor`](../redactor)classe pour un document protégé par mot de passe à l'aide du flux et des paramètres. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initialise une nouvelle instance de[`Redactor`](../redactor) classe pour un document protégé par mot de passe en utilisant son chemin et ses paramètres. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Applique une caviardage au document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Applique une politique de rédaction au document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Applique un ensemble de caviardages au document. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Libère des ressources. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Génère des images d'aperçu de pages spécifiques dans un format d'image donné. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Obtient les informations générales sur le document - taille, nombre de pages, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Enregistre le document dans un fichier avec les options suivantes : AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Enregistre le document dans un fichier. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Enregistre le document dans un flux, y compris l'emplacement personnalisé. |

### Remarques

**Apprendre encore plus**

* Plus de détails sur l'application des caviardages : [Les bases de la rédaction](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Sujets de rédaction plus avancés : [Utilisation avancée](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Exemples

L'exemple suivant illustre l'application d'une seule rédaction au document.

L'exemple suivant illustre l'application d'une liste de caviardages au document.

L'exemple suivant montre comment appliquer une stratégie de masquage à tous les fichiers d'un dossier entrant donné et enregistrer dans l'un des dossiers sortants - pour les fichiers mis à jour avec succès et pour ceux qui ont échoué.

L'exemple suivant montre comment ouvrir un document protégé par mot de passe à l'aide de LoadOptions.

L'exemple suivant montre comment enregistrer un document à l'aide de SaveOptions.

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

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... autres caviardages
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, si au moins une rédaction a échoué
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

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

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Ici, nous pouvons utiliser une instance de document pour effectuer des suppressions
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // La rédaction du document va ici
       // ...
    
       // Enregistrer le document avec les options par défaut (convertir les pages en images, enregistrer au format PDF)
       redactor.Save();
    
       // Enregistrer le document au format d'origine en écrasant le fichier d'origine
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Enregistrer le document dans le fichier "*_Redacted.*" au format d'origine
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Enregistre le document dans "*_AnyText.*" (par exemple, horodatage au lieu de "AnyText") dans son nom de fichier sans pixellisation
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Voir également

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* espace de noms [GroupDocs.Redaction](../../groupdocs.redaction)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

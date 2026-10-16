---
title: "RedactionPolicy"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une politique de désinfection contenant un ensemble de rédactions spécifiques à appliquer."
type: docs
weight: 500
url: /fr/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

Représente une politique de désinfection, contenant un ensemble de rédactions spécifiques à appliquer.

```csharp
public class RedactionPolicy
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Crée une nouvelle instance de la politique de rédaction. |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | Crée une nouvelle instance de la politique de rédaction avec une liste spécifique de rédactions. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | Obtient un tableau de classes dérivées de [`Redaction`](../redaction) entièrement configurées. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | Charge une instance de [`RedactionPolicy`](../redactionpolicy) à partir d'un flux. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | Charge une instance de [`RedactionPolicy`](../redactionpolicy) à partir d'un chemin de fichier. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | Enregistre la politique de rédaction dans un flux. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | Enregistre la politique de rédaction dans un fichier. |

### Remarques

**Learn more**

* More details about policies: [Use of redaction policies](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Exemples

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

L'exemple suivant contient un fichier de politique XML d'exemple avec des configurations d'exemple pour tous les types de rédactions.

```csharp
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Voir aussi

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->

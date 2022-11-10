---
title: Load
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Charge une instance deRedactionPolicygroupdocs.redaction/redactionpolicy à partir dun chemin de fichier.
type: docs
weight: 20
url: /fr/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Charge une instance de[`RedactionPolicy`](../../redactionpolicy) à partir d'un chemin de fichier.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| filePath | String | Chemin d'accès au fichier XML |

### Return_Value

Politique de rédaction

### Exemples

L'exemple suivant montre comment appliquer une stratégie de masquage à tous les fichiers d'un dossier entrant donné et enregistrer dans l'un des dossiers sortants - pour les fichiers mis à jour avec succès et pour ceux qui ont échoué.

L'exemple suivant contient un exemple de fichier de stratégie XML avec des exemples de configuration pour tous les types de biffures.

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

### Voir également

* class [RedactionPolicy](../../redactionpolicy)
* espace de noms [GroupDocs.Redaction](../../redactionpolicy)
* Assemblée [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Charge une instance de[`RedactionPolicy`](../../redactionpolicy) à partir d'un flux.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| input | Stream | Flux contenant la configuration XML |

### Return_Value

Politique de rédaction

### Exemples

L'exemple suivant montre comment appliquer une stratégie de masquage à tous les fichiers d'un dossier entrant donné et enregistrer dans l'un des dossiers sortants - pour les fichiers mis à jour avec succès et pour ceux qui ont échoué.

L'exemple suivant contient un exemple de fichier de stratégie XML avec des exemples de configuration pour tous les types de biffures.

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

### Voir également

* class [RedactionPolicy](../../redactionpolicy)
* espace de noms [GroupDocs.Redaction](../../redactionpolicy)
* Assemblée [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

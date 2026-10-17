---
title: "Utilisez les politiques de rédaction"
linkTitle: "Use redaction policies"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Apprenez à gérer. Si vous avez une politique de suppression de données sensibles d’entreprise sous forme de liste de règles de rédaction, vous n’avez pas besoin de les spécifier dans votre code. Vous pouvez spécifier un document XML contenant une liste de rédactions pré‑configurées."
type: docs
url: /fr/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Si vous avez une politique de suppression de données sensibles d’entreprise sous forme de liste de règles de rédaction, vous n’avez pas besoin de les spécifier dans votre code. Vous pouvez spécifier un document XML contenant une liste de rédactions pré‑configurées.

Ci‑dessous se trouve un exemple de fichier XML de politique de rédaction (le mappage des propriétés du code est évident) :

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
Vous pouvez utiliser la méthode RedactionPolicy.save() pour créer des documents XML de cette structure, en configurant les rédactions à l'exécution.

L'exemple suivant montre comment enregistrer un [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) dans un fichier XML.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # Définissez la couleur de la rédaction
    color = Color.from_argb(255, 220, 20, 60)

    # Configurez les rédactions
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Créez la politique
    policy = RedactionPolicy(redactions)

    # Enregistrez la politique de rédaction dans un fichier XML
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

Vous pouvez disposer d'autant de politiques que nécessaire, en les chargeant pour rédiger vos documents.

L'exemple ci‑dessous charge une politique de rédaction à partir d'un fichier XML et applique chaque règle qu'elle contient à un document en un seul appel `apply` :

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Chargez la politique de rédaction à partir d'un fichier XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Chargez le document et appliquez la politique complète en un seul appel
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Conservez le format original et ajoutez un suffixe au nom de sortie
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` est le fichier de politique utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) pour le télécharger.

`sample.docx` est le document censuré dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

---
title: "Använd redigeringspolicyer"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Lär dig hur du hanterar. Om du har en företagspolicy för borttagning av känslig data som en lista med redigeringsregler, behöver du inte ange dem i din kod. Du kan ange ett XML-dokument med en lista över förkonfigurerade redigeringar."
type: docs
url: /sv/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Om du har en företagspolicy för borttagning av känslig data som en lista med redigeringsregler, behöver du inte ange dem i din kod. Du kan ange ett XML-dokument med en lista över förkonfigurerade redigeringar.

Nedan är ett exempel på en XML-fil för redigeringspolicy (kodegenskapsmappning är uppenbar):

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
Du kan använda metoden RedactionPolicy.save() för att skapa XML-dokument med denna struktur, och konfigurera redigeringar vid körning.

Följande exempel visar hur man sparar en [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) till en XML-fil.
 

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
    # Definiera färgen för redigering
    color = Color.from_argb(255, 220, 20, 60)

    # Konfigurera redigeringarna
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Skapa policyn
    policy = RedactionPolicy(redactions)

    # Spara redigeringspolicyn till en XML-fil
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

Du kan ha så många policyer du behöver, och ladda dem för att redigera dina dokument.

Exemplet nedan laddar en redigeringspolicy från en XML-fil och tillämpar varje regel den innehåller på ett dokument i ett enda `apply`-anrop:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Ladda redigeringspolicyn från en XML-fil
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Ladda dokumentet och tillämpa hela policyn i ett anrop
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Behåll originalformatet och lägg till ett suffix till utdatafilens namn
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` är policyfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) för att ladda ner den.

`sample.docx` är dokumentet som redigerats i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) för att ladda ner det.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

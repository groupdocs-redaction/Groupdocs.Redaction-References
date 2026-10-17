---
title: "Gebruik redactie‑beleid"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Leer hoe u dit aanpakt. Als u een bedrijfsbeleid voor het verwijderen van gevoelige gegevens heeft als een lijst met redactieregels, hoeft u deze niet in uw code te specificeren. U kunt een XML‑document opgeven met een lijst van vooraf geconfigureerde redacties."
type: docs
url: /nl/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Leer hoe u dit aanpakt. Als u een bedrijfsbeleid voor het verwijderen van gevoelige gegevens heeft als een lijst met redactieregels, hoeft u deze niet in uw code te specificeren. U kunt een XML‑document opgeven met een lijst van vooraf geconfigureerde redacties.

Hieronder staat een voorbeeld van een XML‑bestand voor redactie‑beleid (de mapping van code‑eigenschappen is duidelijk):

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
U kunt de methode RedactionPolicy.save() gebruiken om XML‑documenten van deze structuur te maken, waarbij redacties tijdens runtime worden geconfigureerd.

Het volgende voorbeeld laat zien hoe u een [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) opslaat naar een XML‑bestand.
 

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
    # Definieer de kleur van de redactie
    color = Color.from_argb(255, 220, 20, 60)

    # Configureer de redacties
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Maak het beleid
    policy = RedactionPolicy(redactions)

    # Sla het redactie‑beleid op in een XML‑bestand
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

U kunt zoveel beleid hebben als u nodig heeft, en deze laden om uw documenten te redigeren.

Het voorbeeld hieronder laadt een redactiebeleid vanuit een XML‑bestand en past elke regel die het bevat toe op een document in één `apply`‑aanroep:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Laad het redactiebeleid vanuit een XML‑bestand
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Laad het document en pas het volledige beleid toe in één aanroep
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Behoud het oorspronkelijke formaat en voeg een achtervoegsel toe aan de uitvoernaam
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` is het beleidsbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) om het te downloaden.

`sample.docx` is het document dat in dit voorbeeld is geredigeerd. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) om het te downloaden.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

---
title: "Verwenden Sie Redaktionsrichtlinien"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Erfahren Sie, wie Sie vorgehen. Wenn Sie eine unternehmensinterne Richtlinie zur Entfernung sensibler Daten als Liste von Redaktionsregeln haben, müssen Sie diese nicht im Code angeben. Sie können ein XML‑Dokument mit einer Liste vordefinierter Redaktionen angeben."
type: docs
url: /de/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Wenn Sie eine unternehmensinterne Richtlinie zur Entfernung sensibler Daten als Liste von Redaktionsregeln haben, müssen Sie diese nicht im Code angeben. Sie können ein XML‑Dokument mit einer Liste vordefinierter Redaktionen angeben.

Unten finden Sie ein Beispiel für eine Redaktionsrichtlinien‑XML‑Datei (die Zuordnung der Code‑Eigenschaften ist offensichtlich):

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
Sie können die Methode RedactionPolicy.save() verwenden, um XML‑Dokumente dieser Struktur zu erstellen und Redaktionen zur Laufzeit zu konfigurieren.

Das folgende Beispiel zeigt, wie man ein [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) in einer XML‑Datei speichert.
 

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
    # Definieren Sie die Farbe der Redaktion
    color = Color.from_argb(255, 220, 20, 60)

    # Konfigurieren Sie die Redaktionen
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Erstellen Sie die Richtlinie
    policy = RedactionPolicy(redactions)

    # Speichern Sie die Redaktionsrichtlinie in einer XML‑Datei
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

Sie können beliebig viele Richtlinien verwenden, die Sie laden, um Ihre Dokumente zu schwärzen.

Das nachstehende Beispiel lädt eine Redaktionsrichtlinie aus einer XML-Datei und wendet jede darin enthaltene Regel mit einem einzigen `apply`-Aufruf auf ein Dokument an:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Laden Sie die Redaktionsrichtlinie aus einer XML-Datei
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Laden Sie das Dokument und wenden Sie die gesamte Richtlinie in einem Aufruf an
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Behalten Sie das ursprüngliche Format bei und fügen Sie dem Ausgabename ein Suffix hinzu
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` ist die in diesem Beispiel verwendete Richtliniendatei. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml), um sie herunterzuladen.

`sample.docx` ist das in diesem Beispiel geschwärzte Dokument. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx), um es herunterzuladen.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

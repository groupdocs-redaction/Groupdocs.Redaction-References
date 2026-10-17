---
title: "Usa le politiche di redazione"
linkTitle: "Use redaction policies"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Impara a gestire. Se hai una politica di rimozione dati sensibili aziendali come un elenco di regole di redazione, non è necessario specificarle nel tuo codice. Puoi specificare un documento XML con un elenco di redazioni pre-configurate."
type: docs
url: /it/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Se hai una politica di rimozione dati sensibili aziendali come un elenco di regole di redazione, non è necessario specificarle nel tuo codice. Puoi specificare un documento XML con un elenco di redazioni pre-configurate.

Di seguito è un esempio di file XML di politica di redazione (la mappatura delle proprietà del codice è ovvia):

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
Puoi usare il metodo RedactionPolicy.save() per creare documenti XML di questa struttura, configurando le redazioni a runtime.

Il seguente esempio dimostra come salvare un [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) in un file XML.
 

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
    # Definisci il colore della redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Configura le redazioni
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Crea la politica
    policy = RedactionPolicy(redactions)

    # Salva la politica di redazione in un file XML
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

Puoi avere quante politiche desideri, caricandole per redigere i tuoi documenti.

L'esempio seguente carica una policy di redazione da un file XML e applica ogni regola contenuta a un documento in una singola chiamata `apply`:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Carica la policy di redazione da un file XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Carica il documento e applica l'intera policy in una sola chiamata
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Mantieni il formato originale e aggiungi un suffisso al nome di output
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` è il file di policy utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) per scaricarlo.

`sample.docx` è il documento redatto in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) per scaricarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

---
title: "Utilice políticas de redacción"
linkTitle: "Use redaction policies"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Aprenda cómo proceder. Si tiene una política corporativa de eliminación de datos sensibles como una lista de reglas de redacción, no necesita especificarlas en su código. Puede especificar un documento XML con una lista de redacciones preconfiguradas."
type: docs
url: /es/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Aprenda cómo proceder. Si tiene una política corporativa de eliminación de datos sensibles como una lista de reglas de redacción, no necesita especificarlas en su código. Puede especificar un documento XML con una lista de redacciones preconfiguradas.

A continuación se muestra un ejemplo de archivo XML de política de redacción (el mapeo de propiedades de código es evidente):

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
Puede usar el método RedactionPolicy.save() para crear documentos XML con esta estructura, configurando las redacciones en tiempo de ejecución.

El siguiente ejemplo muestra cómo guardar una [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) en un archivo XML.
 

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
    # Defina el color de la redacción
    color = Color.from_argb(255, 220, 20, 60)

    # Configure las redacciones
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Cree la política
    policy = RedactionPolicy(redactions)

    # Guarde la política de redacción en un archivo XML
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

Puede tener tantas políticas como necesite, cargándolas para redactar sus documentos.

El ejemplo a continuación carga una política de redacción desde un archivo XML y aplica cada regla que contiene a un documento en una única llamada `apply`:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Cargar la política de redacción desde un archivo XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Cargar el documento y aplicar toda la política en una sola llamada
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Mantener el formato original y añadir un sufijo al nombre de salida
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` es el archivo de política utilizado en este ejemplo. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) para descargarlo.

`sample.docx` es el documento redactado en este ejemplo. Haga clic [aquí](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) para descargarlo.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)

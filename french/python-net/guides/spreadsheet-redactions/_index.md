---
title: "Redactions de feuilles de calcul"
linkTitle: "Spreadsheet redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment l’API de redaction Python permet de masquer des données sensibles ou privées de vos formats de documents de feuilles de calcul XLS, XLSX, ODS et autres."
type: docs
url: /fr/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction permet de masquer des données sensibles ou privées de vos formats de documents de feuilles de calcul XLS, XLSX, ODS et autres. Voir la liste complète dans l’article [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Spécifiez les options de redaction
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Chargez la feuille de calcul à masquer
    with Redactor("./sample.xlsx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(ex_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` est le fichier d’exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) pour le télécharger.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)

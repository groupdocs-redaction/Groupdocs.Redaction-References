---
title: "Pagina-redacties verwijderen"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe je pagina's met gevoelige gegevens uit je PDF-, presentatie- en spreadsheetdocumenten kunt verwijderen."
type: docs
url: /nl/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction maakt het eenvoudig om pagina's uit PDF-documenten, dia's uit presentaties en werkbladen uit spreadsheetdocumenten te verwijderen.

Met de GroupDocs.Redaction API kun je pagina's verwijderen door het paginabereik op te geven via de relatieve positie (het begin of het einde), een nulgebaseerde index en het aantal te verwijderen pagina's. Op dit moment worden de volgende formaten ondersteund: PDF, presentaties (Microsoft PowerPoint, OpenOffice Presentaties), tekstverwerkingsdocumenten (Microsoft Word, OpenOffice Teksten, Rich Text-bestanden), spreadsheets (Microsoft Excel, OpenOffice Spreadsheets, enz.) en meerframe-afbeeldingen.

## Remove page range

In het onderstaande voorbeeld verwijderen we de 2e, 3e en 4e pagina's uit het document, als het document voldoende pagina's heeft:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Laad het te redigeren document
    with Redactor("./multipage_sample.pdf") as redactor:
        # Documentinformatie ophalen
        doc_info = redactor.get_document_info()

        # Vereist minimaal 4 pagina's
        if doc_info.page_count > 3:
            # Verwijder 3 pagina's beginnend vanaf de 2e (nulgebaseerde index 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Pas de redactie toe
            result = redactor.apply(rem_opt)

            # Sla het geredigeerde document op naast het bronbestand
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) om het te downloaden.

## Remove last page

In sommige gevallen moet je mogelijk de laatste pagina of een aantal pagina's verwijderen, ongeacht hoeveel pagina's er zijn.

Het volgende voorbeeld toont hoe je de laatste pagina uit een document kunt verwijderen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Verwijder 1 pagina, geteld vanaf het einde van het document
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Laad het te redigeren document
    with Redactor("./multipage_sample.pdf") as redactor:
        # Documentinformatie ophalen
        doc_info = redactor.get_document_info()

        # Vereist minimaal 2 pagina's zodat het document niet leeg blijft
        if doc_info.page_count > 1:
            # Pas de redactie toe
            result = redactor.apply(rem_opt)

            # Sla het geredigeerde document op naast het bronbestand
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) om het te downloaden.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

In het geval van een meerframe-afbeelding moet je mogelijk een aantal frames verwijderen (gezien als "pagina's").

Het volgende voorbeeld toont hoe je 3 frames uit een geanimeerde GIF-afbeelding kunt verwijderen:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Verwijder frames beginnend vanaf de 3e (nulgebaseerde index 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Laad de meerframe-afbeelding die moet worden geredigeerd
    with Redactor("./sample.gif") as redactor:
        # Documentinformatie ophalen
        doc_info = redactor.get_document_info()

        # Vereist minimaal 7 frames
        if doc_info.page_count >= 7:
            # Pas de redactie toe
            result = redactor.apply(rem_opt)

            # Sla de geredigeerde afbeelding op naast het bronbestand
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) om het te downloaden.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)

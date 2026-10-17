---
title: "Ta bort sidredigeringar"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Den här artikeln visar hur du tar bort sidor med känslig data från dina PDF-, presentations- och kalkylbladsdokument."
type: docs
url: /sv/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction gör det enkelt att ta bort sidor från PDF-dokument, bilder från presentationer och kalkylblad från kalkylbladsdokument.

Med GroupDocs.Redaction API kan du ta bort sidor genom att ange sidintervallet med hjälp av dess relativa position (början eller slutet), nollbaserat index och antalet sidor som ska tas bort. För närvarande stöds följande format: PDF, presentationer (Microsoft PowerPoint, OpenOffice Presentationer), ordbehandlingsdokument (Microsoft Word, OpenOffice Text, Rich Text-filer), kalkylblad (Microsoft Excel, OpenOffice Kalkylblad, etc.) och flerbilds‑bilder.

## Remove page range

I exemplet nedan tar vi bort den 2:a, 3:e och 4:e sidan från dokumentet, om dokumentet har tillräckligt många sidor:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Läs in dokumentet som ska raderas
    with Redactor("./multipage_sample.pdf") as redactor:
        # Hämta dokumentinformation
        doc_info = redactor.get_document_info()

        # Kräver minst 4 sidor
        if doc_info.page_count > 3:
            # Ta bort 3 sidor med början från den 2:a (nollbaserat index 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Applicera maskeringen
            result = redactor.apply(rem_opt)

            # Spara det redigerade dokumentet bredvid källfilen
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) för att ladda ner den.

## Remove last page

I vissa fall kan du behöva ta bort den sista sidan eller ett antal sidor, oavsett hur många sidor som finns.

Följande exempel visar hur du tar bort den sista sidan från ett dokument:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Ta bort 1 sida räknat från dokumentets slut
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Läs in dokumentet som ska raderas
    with Redactor("./multipage_sample.pdf") as redactor:
        # Hämta dokumentinformation
        doc_info = redactor.get_document_info()

        # Kräver minst 2 sidor så att dokumentet inte blir tomt
        if doc_info.page_count > 1:
            # Applicera maskeringen
            result = redactor.apply(rem_opt)

            # Spara det redigerade dokumentet bredvid källfilen
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) för att ladda ner den.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Om du har en flerbildsbild kan du behöva ta bort ett antal ramar (behandlas som "sidor").

Följande exempel visar hur du tar bort 3 ramar från en animerad GIF-bild:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Ta bort ramar med början från den 3:e (nollbaserat index 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Läs in den flerbildsbild som ska maskeras
    with Redactor("./sample.gif") as redactor:
        # Hämta dokumentinformation
        doc_info = redactor.get_document_info()

        # Kräver minst 7 ramar
        if doc_info.page_count >= 7:
            # Applicera maskeringen
            result = redactor.apply(rem_opt)

            # Spara den maskerade bilden bredvid källfilen
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) för att ladda ner den.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)

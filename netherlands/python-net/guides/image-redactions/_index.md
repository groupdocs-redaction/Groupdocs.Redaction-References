---
title: "Afbeeldingsredacties"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Dit artikel laat zien hoe je gevoelige gegevens uit afbeeldingen van verschillende formaten zoals JPG, PNG, TIFF en andere kunt redigeren."
type: docs
url: /nl/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions biedt een reeks functies om gevoelige gegevens uit afbeeldingen van verschillende formaten zoals JPG, PNG, TIFF en andere te redigeren. Zie de volledige lijst in het artikel [supported document formats]().

GroupDocs.Redaction ondersteunt twee manieren om afbeeldingen te redigeren, zowel in afzonderlijke afbeeldingsbestanden als in ingesloten afbeeldingen:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction voor Python via .NET stelt je ook in staat om afbeeldingsmetadata te wijzigen (bijv. EXIF-gegevens van een afbeelding bewerken of fungeren als een \"EXIF-eraser\").

## Redact image area

Om een afbeeldingsgebied te redigeren, moet je de klasse [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) gebruiken:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Definieer de linkerbovenhoekpositie van het gebied dat moet worden geredigeerd
    sample_point = Point(385, 485)
    # Definieer de grootte van het gebied dat moet worden geredigeerd
    sample_size = Size(1793, 2069)
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Specificeer de redactie‑opties
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.jpg") as redactor:
        # Pas de redactie toe
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Standaard wordt het geredigeerde document opgeslagen in PDF-formaat
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) om het te downloaden.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Als de redactie niet kan worden toegepast op dit type bestanden, bijvoorbeeld een MS Word-document zonder ingesloten afbeeldingen, zal [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) zijn.

## Clean image metadata

Het volgende voorbeeld toont hoe je exif-gegevens (verwijderen) van een foto of een andere afbeelding kunt bewerken:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Specificeer de redactie‑opties om alle afbeeldingsmetadata te verwijderen (bijv. EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Laad de afbeelding die moet worden geredigeerd
    with Redactor("./sample.jpg") as redactor:
        # Pas de redactie toe
        result = redactor.apply(er_opt)

        # Sla de geredigeerde afbeelding op naast het bronbestand
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) om het te downloaden.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Als de redactie niet kan worden toegepast op dit type bestanden, bijvoorbeeld een BMP-afbeelding, zal [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) zijn.

## Redact embedded images

Je kunt een afbeeldingsgebied redigeren binnen alle soorten ingesloten afbeeldingen in een document.

Het volgende voorbeeld toont hoe je alle ingesloten afbeeldingen in een Microsoft Word-document kunt redigeren:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Definieer de linkerbovenhoekpositie van het gebied dat moet worden geredigeerd
    sample_point = Point(516, 311)
    # Definieer de grootte van het gebied dat moet worden geredigeerd
    sample_size = Size(170, 35)
    # Definieer de kleur van de redactiedoos
    color = Color.from_argb(255, 220, 20, 60)

    # Specificeer de redactie‑opties
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Laad het te redigeren document
    with Redactor("./sample.docx") as redactor:
        # Pas de redactie toe op alle ingesloten afbeeldingen
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Standaard wordt het geredigeerde document opgeslagen in PDF-formaat
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` is het voorbeeldbestand dat in dit voorbeeld wordt gebruikt. Klik [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) om het te downloaden.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Als de redactie niet kan worden toegepast op dit type bestanden, bijvoorbeeld een spreadsheet‑document, zal [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) zijn.

## Multi-frame images

Je kunt frames verwijderen uit een multi‑frame afbeelding met een gegeven oorsprong en frame‑aantal. Voor meer informatie zie het artikel [remove page redactions]().

Sommige afbeeldingsformaten, zoals DjVu-documenten, vereisen [pre-rasterization]() en verdere opslag in PDF-formaat.

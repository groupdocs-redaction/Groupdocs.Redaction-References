---
title: "Bildradering"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Denna artikel visar hur man raderar känslig data från bilder i olika format som JPG, PNG, TIFF och andra."
type: docs
url: /sv/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions erbjuder en uppsättning funktioner för att radera känslig data från bilder i olika format som JPG, PNG, TIFF och andra. Se hela listan i artikeln [supported document formats]() .

GroupDocs.Redaction stödjer två sätt att radera bilder, både i separata bildfiler och inbäddade bilder:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction för Python via .NET låter dig också ändra bildmetadata (t.ex. redigera EXIF-data för en bild eller fungera som en "EXIF raderare").

## Redact image area

För att radera ett bildområde måste du använda klassen [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Definiera den övre vänstra positionen för området som ska raderas
    sample_point = Point(385, 485)
    # Definiera storleken på området som behöver raderas
    sample_size = Size(1793, 2069)
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Ange redigeringsalternativen
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.jpg") as redactor:
        # Applicera maskeringen
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Som standard sparas det maskerade dokumentet i PDF-format
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) för att ladda ner den.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Om raderingen inte kan tillämpas på den här filtypen, t.ex. ett MS Word-dokument utan inbäddade bilder, kommer [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) att vara [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

Följande exempel visar hur man redigerar exif-data (raderar dem) från ett foto eller någon annan bild:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Ange raderingsalternativen för att ta bort all bildmetadata (t.ex. EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Läs in bilden som ska raderas
    with Redactor("./sample.jpg") as redactor:
        # Applicera maskeringen
        result = redactor.apply(er_opt)

        # Spara den maskerade bilden bredvid källfilen
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) för att ladda ner den.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Om raderingen inte kan tillämpas på den här filtypen, t.ex. en BMP-bild, kommer [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) att vara [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

Du kan radera bildområden i alla typer av inbäddade bilder i ett dokument.

Följande exempel visar hur man raderar alla inbäddade bilder i ett Microsoft Word-dokument:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Definiera den övre vänstra positionen för området som ska raderas
    sample_point = Point(516, 311)
    # Definiera storleken på området som behöver raderas
    sample_size = Size(170, 35)
    # Definiera färgen på redigeringsrutan
    color = Color.from_argb(255, 220, 20, 60)

    # Ange redigeringsalternativen
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Läs in dokumentet som ska raderas
    with Redactor("./sample.docx") as redactor:
        # Applicera raderingen på alla inbäddade bilder
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Som standard sparas det maskerade dokumentet i PDF-format
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` är exempelfilen som används i detta exempel. Klicka på [här](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) för att ladda ner den.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Om redigeringen inte kan tillämpas på den här typen av filer, t.ex. ett kalkylblad, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) kommer att vara [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

Du kan ta bort ramar från en flerbildsbild med ett givet ursprung och antal ramar. För ytterligare information se artikeln [remove page redactions]().

Vissa bildformat, såsom DjVu-dokument, kräver [pre-rasterization]() och vidare sparande i PDF-format.

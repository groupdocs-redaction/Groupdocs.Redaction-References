---
title: "Bildredaktionen"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Dieser Artikel zeigt, wie man sensible Daten aus Bildern verschiedener Formate wie JPG, PNG, TIFF und andere redigiert."
type: docs
url: /de/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions bietet eine Reihe von Funktionen, um sensible Daten aus Bildern verschiedener Formate wie JPG, PNG, TIFF und andere zu redigieren. Siehe die vollständige Liste im Artikel [supported document formats]().

GroupDocs.Redaction unterstützt zwei Methoden zum Redigieren von Bildern, sowohl in separaten Bilddateien als auch in eingebetteten Bildern:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction für Python via .NET ermöglicht es Ihnen außerdem, Bild-Metadaten zu ändern (z. B. EXIF-Daten eines Bildes zu bearbeiten oder als \"EXIF‑Radierer\" zu fungieren).

## Redact image area

Um einen Bildbereich zu redigieren, müssen Sie die Klasse [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) verwenden:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Definieren Sie die obere linke Position des zu redigierenden Bereichs
    sample_point = Point(385, 485)
    # Definieren Sie die Größe des zu redigierenden Bereichs
    sample_size = Size(1793, 2069)
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie die Redaktionsoptionen an
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.jpg") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Standardmäßig wird das redigierte Dokument im PDF-Format gespeichert.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) zum Herunterladen.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Wenn die Redaktion nicht auf diesen Dateityp angewendet werden kann, z. B. ein MS‑Word‑Dokument ohne eingebettete Bilder, wird [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) den Wert [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) haben.

## Clean image metadata

Das folgende Beispiel demonstriert, wie man EXIF-Daten (löscht) von einem Foto oder einem anderen Bild bearbeitet:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Geben Sie die Redaktionsoptionen an, um alle Bild-Metadaten (z. B. EXIF) zu entfernen
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Laden Sie das zu redigierende Bild
    with Redactor("./sample.jpg") as redactor:
        # Wende die Schwärzung an
        result = redactor.apply(er_opt)

        # Speichern Sie das redigierte Bild neben der Quelldatei
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) zum Herunterladen.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Wenn die Redaktion nicht auf diesen Dateityp angewendet werden kann, z. B. BMP‑Bild, wird [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) sein.

## Redact embedded images

Sie können Bildbereiche innerhalb aller Arten von eingebetteten Bildern in einem Dokument redigieren.

Das folgende Beispiel zeigt, wie man alle eingebetteten Bilder in einem Microsoft‑Word‑Dokument redigiert:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Definieren Sie die obere linke Position des zu redigierenden Bereichs
    sample_point = Point(516, 311)
    # Definieren Sie die Größe des zu redigierenden Bereichs
    sample_size = Size(170, 35)
    # Definieren Sie die Farbe der Redaktions-Box
    color = Color.from_argb(255, 220, 20, 60)

    # Geben Sie die Redaktionsoptionen an
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Laden Sie das zu redigierende Dokument
    with Redactor("./sample.docx") as redactor:
        # Wenden Sie die Redaktion auf alle eingebetteten Bilder an
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Standardmäßig wird das redigierte Dokument im PDF-Format gespeichert.
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` ist die Beispieldatei, die in diesem Beispiel verwendet wird. Klicken Sie [hier](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) zum Herunterladen.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Wenn die Redaktion nicht auf diesen Dateityp angewendet werden kann, z. B. ein Tabellenkalkulationsdokument, wird [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) sein.

## Multi-frame images

Sie können Rahmen aus einem Mehrfachrahmen‑Bild mit einem angegebenen Ursprung und einer Rahmenanzahl entfernen. Weitere Informationen finden Sie im Artikel [remove page redactions]().

Einige Bildformate, wie DjVu‑Dokumente, erfordern [pre-rasterization]() und ein anschließendes Speichern im PDF‑Format.

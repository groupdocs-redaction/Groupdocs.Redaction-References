---
title: "Redazioni di immagini"
linkTitle: "Image redactions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra come redigere dati di natura sensibile da immagini di vari formati come JPG, PNG, TIFF e altri."
type: docs
url: /it/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions offre un set di funzionalità per redigere dati di natura sensibile da immagini di vari formati come JPG, PNG, TIFF e altri. Vedi l'elenco completo nell'articolo [supported document formats]().

GroupDocs.Redaction supporta due modalità di redazione delle immagini, sia in file immagine separati che in immagini incorporate:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction per Python via .NET consente anche di modificare i metadati dell'immagine (ad esempio modificare i dati EXIF di un'immagine o agire come un "cancella EXIF").

## Redact image area

Per redigere un'area dell'immagine, è necessario utilizzare la classe [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/):

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Definisci la posizione in alto a sinistra dell'area da redigere
    sample_point = Point(385, 485)
    # Definisci le dimensioni dell'area che deve essere redatta
    sample_size = Size(1793, 2069)
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Specifica le opzioni di redazione
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.jpg") as redactor:
        # Applica la redazione
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Per impostazione predefinita, il documento redatto viene salvato in formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) per scaricarlo.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Se la redazione non può essere applicata a questo tipo di file, ad esempio un documento MS Word senza immagini incorporate, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sarà [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Clean image metadata

Il seguente esempio dimostra come modificare i dati EXIF (cancellarli) da una foto o da qualsiasi altra immagine:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Specifica le opzioni di redazione per rimuovere tutti i metadati dell'immagine (ad esempio EXIF)
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Carica l'immagine da redigere
    with Redactor("./sample.jpg") as redactor:
        # Applica la redazione
        result = redactor.apply(er_opt)

        # Salva l'immagine redatta accanto al file sorgente
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) per scaricarlo.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Se la redazione non può essere applicata a questo tipo di file, ad esempio un'immagine BMP, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sarà [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Redact embedded images

È possibile redigere l'area dell'immagine all'interno di tutti i tipi di immagini incorporate in un documento.

Il seguente esempio dimostra come redigere tutte le immagini incorporate all'interno di un documento Microsoft Word:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Definisci la posizione in alto a sinistra dell'area da redigere
    sample_point = Point(516, 311)
    # Definisci le dimensioni dell'area che deve essere redatta
    sample_size = Size(170, 35)
    # Definisci il colore della casella di redazione
    color = Color.from_argb(255, 220, 20, 60)

    # Specifica le opzioni di redazione
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Carica il documento da redigere
    with Redactor("./sample.docx") as redactor:
        # Applica la redazione a tutte le immagini incorporate
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Per impostazione predefinita, il documento redatto viene salvato in formato PDF
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` è il file di esempio utilizzato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) per scaricarlo.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Se la redazione non può essere applicata a questo tipo di file, ad esempio un documento di foglio di calcolo, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) sarà [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/).

## Multi-frame images

È possibile rimuovere i fotogrammi da un'immagine multi-fotogramma con un'origine e un numero di fotogrammi specificati. Per ulteriori informazioni, consulta l'articolo [remove page redactions]().

Alcuni formati di immagine, come i documenti DjVu, richiedono la [pre-rasterizzazione]() e il successivo salvataggio in formato PDF.

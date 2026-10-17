---
title: "Rimuovi le redazioni di pagina"
linkTitle: "Remove page redactions"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo mostra come rimuovere le pagine con dati sensibili dai tuoi documenti PDF, di presentazione e di foglio di calcolo."
type: docs
url: /it/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction consente di rimuovere facilmente le pagine dai documenti PDF, le diapositive dalle presentazioni e i fogli di lavoro dai documenti di foglio di calcolo.

Con l'API GroupDocs.Redaction è possibile rimuovere le pagine specificando l'intervallo di pagine mediante la loro posizione relativa (l'inizio o la fine), l'indice basato su zero e il numero di pagine da rimuovere. Attualmente i formati supportati sono: PDF, presentazioni (Microsoft PowerPoint, OpenOffice Presentations), documenti di elaborazione testi (Microsoft Word, OpenOffice Texts, Rich Text Files), fogli di calcolo (Microsoft Excel, OpenOffice Spreadsheets, ecc.) e immagini multi-frame.

## Remove page range

Nell'esempio seguente, rimuoviamo le pagine 2, 3 e 4 dal documento, se il documento ha un numero sufficiente di pagine:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Carica il documento da redigere
    with Redactor("./multipage_sample.pdf") as redactor:
        # Ottieni informazioni sul documento
        doc_info = redactor.get_document_info()

        # Richiede almeno 4 pagine
        if doc_info.page_count > 3:
            # Rimuovi 3 pagine a partire dalla seconda (indice zero 1)
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Applica la redazione
            result = redactor.apply(rem_opt)

            # Salva il documento redatto accanto al file sorgente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) per scaricarlo.

## Remove last page

In alcuni casi potresti dover eliminare l'ultima pagina o un numero di pagine, indipendentemente da quante pagine ci siano.

Il seguente esempio dimostra come rimuovere l'ultima pagina da un documento:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Rimuovi 1 pagina contando dalla fine del documento
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Carica il documento da redigere
    with Redactor("./multipage_sample.pdf") as redactor:
        # Ottieni informazioni sul documento
        doc_info = redactor.get_document_info()

        # Richiede almeno 2 pagine affinché il documento non rimanga vuoto
        if doc_info.page_count > 1:
            # Applica la redazione
            result = redactor.apply(rem_opt)

            # Salva il documento redatto accanto al file sorgente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) per scaricarlo.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Nel caso di un'immagine multi-frame potresti dover eliminare un numero di fotogrammi (trattati come "pagine").

Il seguente esempio dimostra come rimuovere 3 fotogrammi da un'immagine GIF animata:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # Rimuovi i fotogrammi a partire dal terzo (indice zero 2)
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Carica l'immagine multi-frame da redigere
    with Redactor("./sample.gif") as redactor:
        # Ottieni informazioni sul documento
        doc_info = redactor.get_document_info()

        # Richiede almeno 7 fotogrammi
        if doc_info.page_count >= 7:
            # Applica la redazione
            result = redactor.apply(rem_opt)

            # Salva l'immagine redatta accanto al file sorgente
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` è il file di esempio utilizzato in questo esempio. Fai clic [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) per scaricarlo.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)

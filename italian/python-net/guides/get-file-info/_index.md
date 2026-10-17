---
title: "Ottieni informazioni sul file"
linkTitle: "Get file info"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Questo articolo spiega la capacità dell'API GroupDocs.Redaction di ottenere le informazioni generali del documento, che includono FileType, PageCount e FileSize."
type: docs
url: /it/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction fornisce informazioni generali sul documento, che includono:

*   FileType
*   PageCount
*   FileSize

I seguenti esempi di codice mostrano come ottenere le informazioni del documento.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Carica il documento dal disco locale
    with Redactor("./sample.docx") as redactor:
        # Recupera le informazioni generali del documento
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` è il file di esempio usato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) per scaricarlo.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_local_file_info/get-local-file-info.txt)

## Get file info for a file from Stream

```python
from groupdocs.redaction import Redactor

def get_file_info_from_stream():
    # Apri il documento come stream binario
    with open("./sample.docx", "rb") as stream:
        # Carica il documento dallo stream
        with Redactor(stream) as redactor:
            # Recupera le informazioni generali del documento
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` è il file di esempio usato in questo esempio. Fai clic su [qui](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) per scaricarlo.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)

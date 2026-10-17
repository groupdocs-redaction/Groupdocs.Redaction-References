---
title: "Obtenir les informations du fichier"
linkTitle: "Get file info"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article explique la capacité de l'API GroupDocs.Redaction à obtenir les informations générales du document, qui comprennent FileType, PageCount et FileSize."
type: docs
url: /fr/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction fournit des informations générales sur le document, qui comprennent :

*   FileType
*   PageCount
*   FileSize

Les exemples de code suivants démontrent comment obtenir les informations du document.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Chargez le document depuis le disque local
    with Redactor("./sample.docx") as redactor:
        # Récupérez les informations générales du document
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) pour le télécharger.

  
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
    # Ouvrez le document en tant que flux binaire
    with open("./sample.docx", "rb") as stream:
        # Chargez le document depuis le flux
        with Redactor(stream) as redactor:
            # Récupérez les informations générales du document
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) pour le télécharger.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)

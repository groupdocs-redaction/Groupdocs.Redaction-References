---
title: "Λάβετε τις υποστηριζόμενες μορφές αρχείων"
linkTitle: "Get supported file formats"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αυτό το άρθρο δείχνει πώς να λάβετε τη λίστα με όλες τις υποστηριζόμενες μορφές αρχείων του GroupDocs.Redaction χρησιμοποιώντας Python."
type: docs
url: /el/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


Το GroupDocs.Redaction επιτρέπει την λήψη της λίστας με όλες τις υποστηριζόμενες μορφές αρχείων ακολουθώντας τα παρακάτω βήματα:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

Το παρακάτω παράδειγμα δείχνει πώς να λάβετε τη λίστα με τις υποστηριζόμενες μορφές αρχείων.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # Ανακτήστε τη συλλογή των υποστηριζόμενων τύπων αρχείων
    supported_file_types = FileType.get_supported_file_types()

    # Απαριθμήστε τους τύπους αρχείων ταξινομημένους κατά επέκταση
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)

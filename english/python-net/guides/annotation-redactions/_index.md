---
title: Annotation redactions
linkTitle: "Annotation redactions"
second_title: GroupDocs.Redaction for Python via .NET API References
description: "This article shows the implementation of annotation redaction for documents of different formats like PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX and others."
type: docs
url: /python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


With GroupDocs.Redaction API you can apply annotation redactions for documents of different formats like PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX and others. See full list at [supported document formats]() article.

GroupDocs.Redactions provides a flexible API that allows to remove sensitive data from annotation text, or completely remove annotations by a regular expression.

## Remove annotations (comments etc)

You can use GroupDocs.Redaction to remove all or specific comments and other annotations from the document. For example, we can remove all comments from the document, containing texts like "use", "show" or "describe" in its body:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Specify the redaction options to delete annotations matching the pattern
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Load the document to be redacted
    with Redactor("./annotated.xlsx") as redactor:
        # Apply the redaction
        result = redactor.apply(a_red)

        # Save the redacted document next to the source file
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` is the sample file used in this example. Click [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) to download it.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

You can use constructor without arguments to remove all annotations within the document.

## Redact annotations

Instead of removing all or specific annotations, you can remove sensitive data from the annotation text. For instance, we can remove all mentions of "John" in the given document, e.g.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Specify the redaction options: search pattern and replacement string
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Load the document to be redacted
    with Redactor("./annotated.xlsx") as redactor:
        # Apply the redaction
        result = redactor.apply(a_red)

        # Save the redacted document next to the source file
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` is the sample file used in this example. Click [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) to download it.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)

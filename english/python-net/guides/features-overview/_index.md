---
title: Features Overview
linkTitle: "Features overview"
second_title: GroupDocs.Redaction for Python via .NET API References
description: "GroupDocs.Redaction for Python via .NET removes sensitive information from documents through a single, format-independent API — text, metadata, image areas, annotations, and whole pages — and saves the result in the original format or as a sanitized PDF."
type: docs
url: /python-net/guides/features-overview/
is_root: false
weight: 40
---


GroupDocs.Redaction for Python via .NET removes or permanently obscures sensitive information across a wide range of [supported document formats](https://docs.groupdocs.com/redaction/python-net/supported-document-formats/). Every redaction follows the same workflow: open a document with [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), apply one or more redactions with `apply()`, then `save()` the cleaned result either in its original format or as a sanitized PDF. The capabilities below can be combined freely in a single pass.

## Text redaction

Find and replace text by an exact phrase or by a regular expression, covering both whole words and complex patterns such as e-mail addresses, phone numbers, or national ID numbers. Matched text can be replaced with substitute text or covered by a colored box so the original content cannot be recovered. In spreadsheets you can narrow the search to a single worksheet or column. See [Text Redactions](/redaction/python-net/guides/text-redactions/).

## Text in images (OCR)

Redact text in scanned pages, photos and the images a document embeds. GroupDocs.Redaction ships no OCR engine: connect the one you use, such as Tesseract, through an object with a `recognize()` method that reports the lines it found and where, and phrases and regular expressions then work on images as on text. See [Using OCR](https://docs.groupdocs.com/redaction/python-net/using-ocr/).

## Metadata redaction

Erase or rewrite document metadata — author, title, company, comments, and EXIF data on images — so no sensitive details leak through document properties. You can clear all metadata, target specific fields, or replace values with new ones. See [Metadata Redactions](/redaction/python-net/guides/metadata-redactions/).

## Image-area redaction

Black out a rectangular region of an embedded image or a scanned page by drawing a filled box over a given area — useful for hiding signatures, photos, headers, or footers where confidential data is expected to appear. See [Image Redactions](/redaction/python-net/guides/image-redactions/).

## Page-area redaction

Limit a redaction to an area of a page, such as the right half of the last page, and redact the text and the images inside it in one call. See [Use Page Area Redaction](/redaction/python-net/guides/use-page-area-redaction/).

## Annotation redaction

Rewrite or delete annotations, comments, and notes. You can remove every annotation or use a regular expression to match only the ones that contain sensitive text. See [Annotation Redactions](/redaction/python-net/guides/annotation-redactions/).

## Page removal

Remove whole pages from PDF documents, slides from presentations, and worksheets from spreadsheets. You specify a starting page and a count, together with the direction relative to the starting point. See [Remove Page Redactions](/redaction/python-net/guides/remove-page-redactions/).

## Approve or reject each redaction

A redaction callback sees every match before it is redacted, with its text and position, and decides whether it goes: log what is removed, or keep the matches a reviewer has cleared. See [Use Redaction Callback](/redaction/python-net/guides/use-redaction-callback/).

## Rasterization to PDF

Save the cleaned document as a PDF whose pages are rendered as raster images. The resulting file contains no searchable text and none of the original metadata, so the removed content cannot be recovered. Rasterization is the right choice when you must hand a document to third parties or conform to regulations that require PDF. You can select specific pages and request PDF/A compliance through the advanced rasterization options. See [Save in Rasterized PDF](https://docs.groupdocs.com/redaction/python-net/save-in-rasterized-pdf/) and [Advanced Rasterization Options](https://docs.groupdocs.com/redaction/python-net/use-advanced-rasterization-options/).

## Redaction policies

Group several redactions into a reusable policy and apply the same set of rules consistently across many documents — ideal for recurring tasks such as scrubbing a standard set of fields before publishing. See [Use Redaction Policies](/redaction/python-net/guides/use-redaction-policies/).

## Page previews

Render pages to PNG, JPEG or BMP images, in files or in memory, to show a document before you redact it. See [Get Document Page Preview](/redaction/python-net/guides/get-document-page-preview/).

## Logging

Pass a logger to see the engine's errors, warnings and trace messages while it loads, redacts and saves a document. See [Use Advanced Logging](/redaction/python-net/guides/use-advanced-logging/).

## Loading and saving

Load documents from a local path or from a stream, including password-protected files, name the format of a stream or of a file with an unusual extension ([Load with File Type](/redaction/python-net/guides/load-with-file-type/)), and optionally pre-rasterize a document before redacting. When saving, keep the original format for further editing, set the OOXML compliance level of a Word document ([Save Word with OOXML Compliance](/redaction/python-net/guides/save-word-with-ooxml-compliance/)), overwrite the original file, rasterize to PDF, or write to a stream. See [Loading Documents](https://docs.groupdocs.com/redaction/python-net/loading-documents/) and [Saving Documents](https://docs.groupdocs.com/redaction/python-net/saving-documents/).

## On-premise

GroupDocs.Redaction for Python via .NET runs entirely on your own infrastructure — your documents never leave your environment. The package is a self-contained wheel that bundles everything it needs, so no Microsoft Office, OpenOffice, Adobe Acrobat, or separate runtime has to be installed, and it works the same on Windows, Linux and macOS. See [System Requirements](https://docs.groupdocs.com/redaction/python-net/system-requirements/) for the supported platforms and the two system packages Linux needs.

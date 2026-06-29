---
title: Features Overview
linkTitle: "Features overview"
second_title: GroupDocs.Redaction for Python via .NET API References
description: "GroupDocs.Redaction for Python via .NET removes sensitive information from documents through a single, format-independent API — text, metadata, image areas, annotations, and whole pages — and saves the result in the original format or as a sanitized PDF."
type: docs
url: /python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction for Python via .NET removes or permanently obscures sensitive information across a wide range of [supported document formats](). Every redaction follows the same workflow: open a document with [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), apply one or more redactions with `apply()`, then `save()` the cleaned result either in its original format or as a sanitized PDF. The capabilities below can be combined freely in a single pass.

## Text redaction

Find and replace text by an exact phrase or by a regular expression, covering both whole words and complex patterns such as e-mail addresses, phone numbers, or national ID numbers. Matched text can be replaced with substitute text or covered by a colored box so the original content cannot be recovered. In spreadsheets you can narrow the search to a single worksheet or column. See [Text Redactions]().

## Metadata redaction

Erase or rewrite document metadata — author, title, company, comments, and EXIF data on images — so no sensitive details leak through document properties. You can clear all metadata, target specific fields, or replace values with new ones. See [Metadata Redactions]().

## Image-area redaction

Black out a rectangular region of an embedded image or a scanned page by drawing a filled box over a given area — useful for hiding signatures, photos, headers, or footers where confidential data is expected to appear. See [Image Redactions]().

## Annotation redaction

Rewrite or delete annotations, comments, and notes. You can remove every annotation or use a regular expression to match only the ones that contain sensitive text. See [Annotation Redactions]().

## Page removal

Remove whole pages from PDF documents, slides from presentations, and worksheets from spreadsheets. You specify a starting page and a count, together with the direction relative to the starting point. See [Remove Page Redactions]().

## Rasterization to PDF

Save the cleaned document as a PDF whose pages are rendered as raster images. The resulting file contains no searchable text and none of the original metadata, so the removed content cannot be recovered. Rasterization is the right choice when you must hand a document to third parties or conform to regulations that require PDF. You can select specific pages and request PDF/A compliance through the advanced rasterization options. See [Save in Rasterized PDF]() and [Advanced Rasterization Options]().

## Redaction policies

Group several redactions into a reusable policy and apply the same set of rules consistently across many documents — ideal for recurring tasks such as scrubbing a standard set of fields before publishing. See [Use Redaction Policies]().

## Loading and saving

Load documents from a local path or from a stream, including password-protected files, and optionally pre-rasterize a document before redacting. When saving, keep the original format for further editing, overwrite the original file, rasterize to PDF, or write to a stream. See [Loading Documents]() and [Saving Documents]().

## On-premise

GroupDocs.Redaction for Python via .NET runs entirely on your own infrastructure — your documents never leave your environment. The package is a self-contained wheel that bundles everything it needs, so no Microsoft Office, OpenOffice, Adobe Acrobat, or separate runtime has to be installed. See [System Requirements]() for the supported platforms and native dependencies.

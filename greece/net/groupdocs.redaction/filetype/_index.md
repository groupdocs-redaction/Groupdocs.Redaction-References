---
title: "FileType"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αναπαριστά έναν τύπο αρχείου. Παρέχει μεθόδους για την απόκτηση λίστας όλων των τύπων αρχείων που υποστηρίζονται από το GroupDocs.Redaction, ανίχνευση τύπου αρχείου με βάση την επέκταση κ.λπ."
type: docs
weight: 90
url: /el/net/groupdocs.redaction/filetype/
---
## FileType class

Αντιπροσωπεύει έναν τύπο αρχείου. Παρέχει μεθόδους για την λήψη λίστας όλων των τύπων αρχείων που υποστηρίζονται από το GroupDocs.Redaction, την ανίχνευση τύπου αρχείου με βάση την επέκταση, κ.λπ.

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | Αρχείο Bitmap Image (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | Αρχείο τιμών διαχωρισμένων με κόμμα (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | Εικόνα DjVu (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Έγγραφο Microsoft Word (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Έγγραφο Word Open XML με δυνατότητα μακροεντολών (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Έγγραφο Microsoft Word Open XML (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Πρότυπο εγγράφου Word (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Πρότυπο εγγράφου Word Open XML με δυνατότητα μακροεντολών (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Πρότυπο εγγράφου Word Open XML (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | Αρχείο μορφής Graphics Interchange Format (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | Αρχείο Hypertext Markup Language (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | Αρχείο Hypertext Markup Language (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | Αρχείο εικόνας JPEG 2000 Core (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | Εικόνα JPEG (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | Εικόνα JPEG (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | Αρχείο καταγραφής (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | Αρχείο τεκμηρίωσης Markdown (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Φύλλο εργασίας Apple Numbers (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | Παρουσίαση OpenDocument (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | Φύλλο εργασίας OpenDocument (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | Έγγραφο κειμένου OpenDocument (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | Πρότυπο παρουσίασης OpenDocument (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | Πρότυπο φύλλου εργασίας OpenDocument (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | Πρότυπο εγγράφου OpenDocument (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | Αρχείο Portable Document Format (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | Αρχείο Portable Network Graphic (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | Πρότυπο παρουσίασης PowerPoint Open XML με ενεργοποιημένες μακροεντολές (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | Πρότυπο παρουσίασης PowerPoint Open XML (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | Παρουσίαση διαφανειών PowerPoint (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | Διαφάνεια PowerPoint Open XML με ενεργοποιημένες μακροεντολές (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | Παρουσίαση διαφανειών PowerPoint Open XML (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | Παρουσίαση PowerPoint (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | Παρουσίαση PowerPoint Open XML με ενεργοποιημένες μακροεντολές |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | Παρουσίαση PowerPoint Open XML (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | Αρχείο μορφής εμπλουτισμένου κειμένου (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | Αρχείο τιμών διαχωρισμένων με καρτέλα (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | Αρχείο ετικετοποιημένης εικόνας (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | Μορφή αρχείου ετικετοποιημένης εικόνας (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | Αρχείο τιμών διαχωρισμένων με καρτέλα (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | Αρχείο απλού κειμένου (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | Αναπαριστά άγνωστο τύπο αρχείου. |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | Εικόνα WebP (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Φύλλο εργασίας Excel (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Δυαδικό φύλλο εργασίας Excel (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Φύλλο εργασίας Excel Open XML με ενεργοποιημένες μακροεντολές (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Φύλλο εργασίας Microsoft Excel Open XML (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Πρότυπο Excel (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Πρότυπο φύλλου εργασίας Excel Open XML με ενεργοποιημένες μακροεντολές (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Πρότυπο φύλλου εργασίας Excel Open XML (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | Λαμβάνει το επίθημα ονόματος αρχείου (συμπεριλαμβανομένου του σημείου "."), για παράδειγμα ".doc". |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | Λαμβάνει το όνομα τύπου αρχείου, για παράδειγμα "Microsoft Word Document". |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | Αντιστοιχίζει την επέκταση αρχείου στον τύπο αρχείου. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | Καθορίζει εάν ο τρέχων [`FileType`](../filetype) είναι ο ίδιος με το καθορισμένο αντικείμενο [`FileType`](../filetype). |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | Καθορίζει εάν ο τρέχων [`FileType`](../filetype) είναι ο ίδιος με το καθορισμένο αντικείμενο. |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | Επιστρέφει τον κωδικό κατακερματισμού για το τρέχον αντικείμενο [`FileType`](../filetype). |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο. |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | Ανακτά τους υποστηριζόμενους τύπους αρχείων |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | Καθορίζει εάν δύο αντικείμενα [`FileType`](../filetype) είναι τα ίδια. |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | Καθορίζει εάν δύο αντικείμενα [`FileType`](../filetype) δεν είναι τα ίδια. |

### Παρατηρήσεις

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Δείτε επίσης

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->

---
title: "PdfComplianceLevel"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa una lista de niveles de cumplimiento PDF compatibles."
type: docs
weight: 20
url: /es/java/com.groupdocs.redaction.options/pdfcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum PdfComplianceLevel extends Enum<PdfComplianceLevel>
```

Representa una lista de niveles de cumplimiento PDF compatibles.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Auto](#Auto) | El archivo de salida cumplirá con el estándar PDF/A-1b de forma predeterminada. |
|
|  | [PdfA1a](#PdfA1a) | El archivo de salida cumplirá con el estándar PDF/A-1a. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Auto {#Auto}
```
public static final PdfComplianceLevel Auto
```


El archivo de salida cumplirá con el estándar PDF/A-1b de forma predeterminada.


### PdfA1a {#PdfA1a}
```
public static final PdfComplianceLevel PdfA1a
```


El archivo de salida cumplirá con el estándar PDF/A-1a.


### values() {#values--}
```
public static PdfComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.PdfComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static PdfComplianceLevel valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel)

---
title: "ReplacementType"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa un tipo de reemplazo para el texto coincidente."
type: docs
weight: 38
url: /es/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Representa un tipo de reemplazo para el texto coincidente.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Reemplaza el texto coincidente con otra cadena, p. ej. |
|
|  | [DrawBox](#DrawBox) | Dibuja un rectángulo de color específico (Negro por defecto) en lugar del texto redactado. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Reemplaza el texto coincidente con otra cadena, p. ej. código de exención.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Dibuja un rectángulo de color específico (Negro por defecto) en lugar del texto redactado.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)

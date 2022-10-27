---
title: RedactionDescription
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo.
type: docs
weight: 10
url: /es/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| redactionType | RedactionType | Tipo de datos que se redactan |
| actionType | RedactionActionType | Acción a realizar sobre estos datos |
| originalText | String | Texto coincidente, comentario o cuerpo de anotación |

### Ver también

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* espacio de nombres [GroupDocs.Redaction.Redactions](../../redactiondescription)
* asamblea [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| redactionType | RedactionType | Tipo de datos que se redactan |
| actionType | RedactionActionType | Acción a realizar sobre estos datos |
| originalText | String | Texto coincidente, comentario o cuerpo de anotación |
| replacement | TextReplacement | Texto de reemplazo, texto coincidente y su posición dentro de la cadena original |

### Ver también

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* espacio de nombres [GroupDocs.Redaction.Redactions](../../redactiondescription)
* asamblea [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo del área de la imagen.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| redactionType | RedactionType | Tipo de datos que se redactan |
| actionType | RedactionActionType | Acción a realizar sobre estos datos |
| imageAreaReplacement | RegionReplacementOptions | Información de reemplazo del área de la imagen |
| imageDetails | String | Descripción textual de la imagen, por defecto es String.Empty |

### Ver también

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* espacio de nombres [GroupDocs.Redaction.Redactions](../../redactiondescription)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
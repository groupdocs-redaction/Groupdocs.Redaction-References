---
title: RemovePages
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Elimina una o varias páginas según su posición de inicio desplazamiento y recuento.
type: docs
weight: 10
url: /es/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Elimina una o varias páginas según su posición de inicio, desplazamiento y recuento.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| origin | PageSeekOrigin | Buscar la posición de origen, el principio o el final del documento |
| index | Int32 | Índice de posición inicial (basado en 0) |
| count | Int32 | Cantidad de páginas para eliminar |

### Valor_devuelto

Resultado de eliminación de páginas

### Ver también

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* espacio de nombres [GroupDocs.Redaction.Integration](../../ipaginateddocument)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

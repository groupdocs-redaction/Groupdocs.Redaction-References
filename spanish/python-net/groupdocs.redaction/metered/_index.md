---
title: "Clase Metered"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Administra la licencia por consumo (pago por uso)."
type: docs
url: /es/python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

Administra la licencia por consumo (pago por uso).

Las licencias Metered facturan según el consumo real (típicamente páginas o
documentos procesados). Establezca el par de claves pública/privada una vez en
el inicio de la aplicación; el contenedor informa el uso de vuelta a GroupDocs
el servidor de licencias en segundo plano.

El tipo Metered expone los siguientes miembros:

### Métodos
| Método | Descripción |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | Devuelve el crédito medido restante para la clave actual. |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | Devuelve la cantidad total medida consumida hasta ahora. |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | Activa la facturación medida con el par de claves públicas/privadas proporcionado. |

### Ver también
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)

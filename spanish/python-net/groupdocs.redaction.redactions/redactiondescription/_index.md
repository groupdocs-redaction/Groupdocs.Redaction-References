---
title: "Clase RedactionDescription"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa la información de una única acción de cambio que se realizó durante el proceso de redacción."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

Representa la información de una única acción de cambio que se realizó durante el proceso de redacción.

Aprende más

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

El tipo RedactionDescription expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | Inicializa una nueva instancia de la clase RedactionDescription sin información de reemplazo. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | Inicializa una nueva instancia de la clase RedactionDescription con información de reemplazo. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | Inicializa una nueva RedactionDescription con información de reemplazo de área de imagen. |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | La operación de redacción: reemplazo, limpieza o eliminación. |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | La información de detalles opcional para el elemento que se está redactando. |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | La información de reemplazo para redacciones de áreas de imagen, o None para redacciones textuales. |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | El texto coincidente, si se proporciona alguna expresión. |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | El tipo de datos del documento – texto, metadatos o anotaciones. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | La información de reemplazo, puede ser None. |

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)

---
title: GetInstance
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Proporciona una instancia singleton con configuración predeterminada de formatos integrados.
type: docs
weight: 10
url: /es/net/groupdocs.redaction.configuration/redactorconfiguration/getinstance/
---
## RedactorConfiguration.GetInstance method

Proporciona una instancia singleton con configuración predeterminada de formatos integrados.

```csharp
public static RedactorConfiguration GetInstance()
```

### Valor_devuelto

Instancia de configuración

### Ejemplos

El siguiente ejemplo muestra cómo agregar un controlador de formato personalizado.

```csharp
var adobePhotoshopSettings = new DocumentFormatConfiguration();
adobePhotoshopSettings.ExtensionFilter = ".psd";
adobePhotoshopSettings.DocumentType = typeof(MyAdobePhotoshopFormatInstance);
var configuration = RedactorConfiguration.GetInstance();
configuration.AvailableFormats.Add(adobePhotoshopSettings);
```

### Ver también

* class [RedactorConfiguration](../../redactorconfiguration)
* espacio de nombres [GroupDocs.Redaction.Configuration](../../redactorconfiguration)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

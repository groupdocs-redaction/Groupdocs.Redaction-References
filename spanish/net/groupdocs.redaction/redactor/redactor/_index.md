---
title: Redactor
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Inicializa una nueva instancia deRedactorgroupdocs.redaction/redactor clase usando la ruta del archivo.
type: docs
weight: 10
url: /es/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Inicializa una nueva instancia de[`Redactor`](../../redactor) clase usando la ruta del archivo.

```csharp
public Redactor(string filePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | Ruta al archivo |

### Ejemplos

El siguiente ejemplo muestra cómo abrir un documento para su redacción.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Aquí podemos usar la instancia del documento para realizar redacciones
}
```

### Ver también

* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Inicializa una nueva instancia de[`Redactor`](../../redactor) clase usando stream.

```csharp
public Redactor(Stream document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | Flujo de origen del documento |

### Ejemplos

El siguiente ejemplo muestra cómo abrir un documento desde stream.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Aquí podemos usar la instancia del documento para realizar redacciones
    }
}
```

### Ver también

* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Inicializa una nueva instancia de[`Redactor`](../../redactor) class para un documento protegido por contraseña utilizando su ruta.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | Ruta al archivo. |
| loadOptions | LoadOptions | Opciones, incluida la contraseña. |

### Ver también

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Inicializa una nueva instancia de[`Redactor`](../../redactor) class para un documento protegido por contraseña utilizando su ruta y configuración.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | Ruta al archivo. |
| loadOptions | LoadOptions | Opciones dependientes del archivo, incluida la contraseña. |
| settings | RedactorSettings | Configuración predeterminada para el proceso de redacción. |

### Ver también

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Inicializa una nueva instancia de[`Redactor`](../../redactor) clase para un documento protegido por contraseña usando stream.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | Flujo de entrada de origen. |
| loadOptions | LoadOptions | Opciones, incluida la contraseña. |

### Ejemplos

El siguiente ejemplo muestra cómo abrir documentos protegidos con contraseña usando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Aquí podemos usar la instancia del documento para realizar redacciones
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Inicializa una nueva instancia de[`Redactor`](../../redactor) class para un documento protegido por contraseña usando stream y settings.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | Flujo de entrada de origen. |
| loadOptions | LoadOptions | Opciones, incluida la contraseña. |
| settings | RedactorSettings | Configuración predeterminada para el proceso de redacción. |

### Ejemplos

El siguiente ejemplo muestra cómo abrir documentos protegidos con contraseña usando LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Aquí podemos usar la instancia del documento para realizar redacciones
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* espacio de nombres [GroupDocs.Redaction](../../redactor)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

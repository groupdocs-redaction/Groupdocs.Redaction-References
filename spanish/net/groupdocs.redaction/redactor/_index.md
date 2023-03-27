---
title: Redactor
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Representa una clase principal que controla el proceso de redacción de documentos lo que permite abrir redactar y guardar documentos.
type: docs
weight: 660
url: /es/net/groupdocs.redaction/redactor/
---
## Redactor class

Representa una clase principal que controla el proceso de redacción de documentos, lo que permite abrir, redactar y guardar documentos.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Inicializa una nueva instancia de[`Redactor`](../redactor) clase usando stream. |
| [Redactor](redactor#constructor_3)(string) | Inicializa una nueva instancia de[`Redactor`](../redactor) clase usando la ruta del archivo. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Inicializa una nueva instancia de[`Redactor`](../redactor) clase para un documento protegido por contraseña usando stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Inicializa una nueva instancia de[`Redactor`](../redactor) class para un documento protegido por contraseña utilizando su ruta. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Inicializa una nueva instancia de[`Redactor`](../redactor)class para un documento protegido por contraseña usando stream y settings. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Inicializa una nueva instancia de[`Redactor`](../redactor) class para un documento protegido por contraseña utilizando su ruta y configuración. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Aplica una redacción al documento. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Aplica una política de redacción al documento. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Aplica un conjunto de redacciones al documento. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Libera recursos. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Genera imágenes de vista previa de páginas específicas en un formato de imagen determinado. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Obtiene la información general sobre el documento: tamaño, número de páginas, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Guarda el documento en un archivo con las siguientes opciones: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Guarda el documento en un archivo. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Guarda el documento en un flujo, incluida la ubicación personalizada. |

### Observaciones

**Aprende más**

* Más detalles sobre la aplicación de redacciones: [Conceptos básicos de redacción](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Temas de redacción más avanzados: [Uso avanzado](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Ejemplos

El siguiente ejemplo demuestra la aplicación de una sola redacción al documento.

El siguiente ejemplo demuestra la aplicación de una lista de redacciones al documento.

El siguiente ejemplo muestra cómo aplicar una política de redacción a todos los archivos dentro de una carpeta de entrada determinada y guardarlos en una de las carpetas de salida, para archivos actualizados correctamente y para archivos fallidos.

El siguiente ejemplo muestra cómo abrir documentos protegidos con contraseña usando LoadOptions.

El siguiente ejemplo muestra cómo guardar un documento usando SaveOptions.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... otras redacciones
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // falso, si al menos una redacción falló
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Aquí podemos usar la instancia del documento para realizar redacciones
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // La redacción del documento va aquí
       // ...
    
       // Guardar el documento con las opciones predeterminadas (convertir páginas en imágenes, guardar como PDF)
       redactor.Save();
    
       // Guardar el documento en formato original sobrescribiendo el archivo original
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Guardar el documento en el archivo "*_Redacted.*" en formato original
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Guarde el documento en "*_AnyText.*" (por ejemplo, marca de tiempo en lugar de "AnyText") en su nombre de archivo sin rasterizar
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Ver también

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* espacio de nombres [GroupDocs.Redaction](../../groupdocs.redaction)
* asamblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

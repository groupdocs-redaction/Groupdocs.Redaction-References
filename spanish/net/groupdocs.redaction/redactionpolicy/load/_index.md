---
title: Load
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Carga una instancia deRedactionPolicygroupdocs.redaction/redactionpolicy desde una ruta de archivo.
type: docs
weight: 20
url: /es/net/groupdocs.redaction/redactionpolicy/load/
---
## Load(string) {#load_1}

Carga una instancia de[`RedactionPolicy`](../../redactionpolicy) desde una ruta de archivo.

```csharp
public static RedactionPolicy Load(string filePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | Ruta al archivo XML |

### Valor_devuelto

Política de redacción

### Ejemplos

El siguiente ejemplo muestra cómo aplicar una política de redacción a todos los archivos dentro de una carpeta de entrada determinada y guardarlos en una de las carpetas de salida, para archivos actualizados correctamente y para archivos fallidos.

El siguiente ejemplo contiene un archivo de política XML de muestra con configuraciones de muestra para todos los tipos de redacciones.

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Ver también

* class [RedactionPolicy](../../redactionpolicy)
* espacio de nombres [GroupDocs.Redaction](../../redactionpolicy)
* asamblea [GroupDocs.Redaction](../../../)

---

## Load(Stream) {#load}

Carga una instancia de[`RedactionPolicy`](../../redactionpolicy) de un arroyo.

```csharp
public static RedactionPolicy Load(Stream input)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| input | Stream | Secuencia que contiene la configuración XML |

### Valor_devuelto

Política de redacción

### Ejemplos

El siguiente ejemplo muestra cómo aplicar una política de redacción a todos los archivos dentro de una carpeta de entrada determinada y guardarlos en una de las carpetas de salida, para archivos actualizados correctamente y para archivos fallidos.

El siguiente ejemplo contiene un archivo de política XML de muestra con configuraciones de muestra para todos los tipos de redacciones.

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### Ver también

* class [RedactionPolicy](../../redactionpolicy)
* espacio de nombres [GroupDocs.Redaction](../../redactionpolicy)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->

---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction için Java API Referansı"
description: "Paket, farklı kırpma türleri için sınıflar sağlar."
type: docs
weight: 16
url: /tr/java/com.groupdocs.redaction.redactions/
---

Paket, farklı kırpma türleri için sınıflar sağlar.



## Sınıflar

| Sınıf | Açıklama |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Verilen bir düzenli ifadeye uyan açıklama metnini (yorumlar vb.) değiştiren bir kırpmayı temsil eder. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Bir elektronik tablo belgesindeki (CSV, Excel vb.) metni değiştiren bir metin kırpmasını temsil eder. |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | CellColumnRedaction kapsamını bir çalışma sayfası ve bir sütunla sınırlama seçeneği sunar. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) için girdi verileri sağlar. |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) tarafından döndürülen bir sonucu temsil eder. |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Metin verilen bir düzenli ifadeye uyuyorsa açıklamaları (isteğe bağlı olarak tüm açıklamaları) silen bir metin kırpmasını temsil eder. |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Belgeden tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri kırpmasını temsil eder. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Belgenin metnindeki tam ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız şekilde değiştiren bir metin kırpmasını temsil eder. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Bir görüntü belgesinin verilen alanına renkli dikdörtgen yerleştiren bir kırpmayı temsil eder. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Belge meta verilerinin en yaygın türlerinin bir listesini temsil eder. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Belge meta verisi redaksiyonları için temel soyut bir sınıfı temsil eder. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Anahtarları ve/veya değerleri eşleştirerek düzenli ifadeler kullanarak meta veriyi arayan ve redakte eden bir meta veri redaksiyonunu temsil eder. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Redaksiyon filtresini temsil eder, bir belgenin sayfası içinde redaksiyon uygulanacak bir alanı ayarlar. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Sayfanın bir alanındaki metin, görüntü ve açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Redaksiyon filtresini temsil eder, bir belge içinde redaksiyon uygulanacak sayfa aralığını ayarlar. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Redaksiyon filtresini temsil eder, bir belge içinde redaksiyonların uygulanacağı kapsamı ayarlar. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Redaksiyon tarafından etkilenen belgenin veri türünü temsil eder. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Görüntü bölgesi değiştirme için renk ve alan parametrelerini temsil eder. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Bir belgeden sayfa (slayt, çalışma sayfası vb.) kaldıran bir redaksiyonu temsil eder. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Eşleşen metin değişimi için seçenekleri temsil eder. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Belge metni redaksiyonları için temel soyut bir sınıfı temsil eder. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Metinsel bir değiştirme bilgisini temsil eder. |

## Arayüzler

| Arayüz | Açıklama |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Özel bir redaksiyon geri çağrısını tanımlar. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Her redaksiyon değişikliği hakkında bilgi almayı ve isteğe bağlı olarak engellemeyi gerektiren yöntemleri tanımlar. |

## Enumlar

| Enum | Açıklama |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Belge içinde arama yapmak için referans noktalarını temsil eden alanları sağlar. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Redaksiyon gerçekleştirmek için alınabilecek eylemleri temsil eder. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Eşleşen metin için bir değiştirme türünü temsil eder. |

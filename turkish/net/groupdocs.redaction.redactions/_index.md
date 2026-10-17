---
title: "GroupDocs.Redaction.Redactions"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Redactions ad alanı farklı redaksiyon türleri için sınıflar sağlar."
type: docs
weight: 80
url: /tr/net/groupdocs.redaction.redactions/
---
Redactions ad alanı farklı redaksiyon türleri için sınıflar sağlar.

## Sınıflar

| Sınıf | Açıklama |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Verilen bir düzenli ifadeye uyan açıklama metnini (yorumlar vb.) değiştiren bir redaksiyonu temsil eder. |
| [CellColumnRedaction](./cellcolumnredaction) | Bir elektronik tablo belgesindeki (CSV, Excel vb.) metni değiştiren bir metin redaksiyonunu temsil eder. |
| [CellFilter](./cellfilter) | [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) kapsamını bir çalışma sayfası ve bir sütunla sınırlama seçeneği sunar. |
| [CustomRedactionContext](./customredactioncontext) | Özel redaksiyon işleme için bağlam sağlar. |
| [CustomRedactionResult](./customredactionresult) | Özel bir redaksiyon işleminin sonucunu temsil eder. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Metin verilen bir düzenli ifadeye uyuyorsa açıklamaları (isteğe bağlı olarak tüm açıklamaları) silen bir metin redaksiyonunu temsil eder. |
| [EraseMetadataRedaction](./erasemetadataredaction) | Belgedeki tüm meta verileri veya belirli MetadataFilters ile eşleşen meta verileri silen bir meta veri redaksiyonunu temsil eder. |
| [ExactPhraseRedaction](./exactphraseredaction) | Belgenin metnindeki tam ifadeyi, varsayılan olarak büyük/küçük harfe duyarsız bir şekilde değiştiren bir metin redaksiyonunu temsil eder. |
| [ImageAreaRedaction](./imagearearedaction) | Bir görüntü belgesinin belirli alanına renkli dikdörtgen yerleştiren bir redaksiyonu temsil eder. |
| [MetadataRedaction](./metadataredaction) | Belge meta verisi redaksiyonları için temel soyut sınıfı temsil eder. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Anahtarları ve/veya değerleri eşleştirerek düzenli ifadelerle meta verileri arayan ve redakte eden bir meta veri redaksiyonunu temsil eder. |
| [PageAreaFilter](./pageareafilter) | Belgenin bir sayfası içinde redaksiyon uygulanacak bir alanı ayarlayan redaksiyon filtresini temsil eder. |
| [PageAreaRedaction](./pagearearedaction) | Sayfanın bir alanındaki metin, görüntü ve açıklamaları etkileyen karmaşık bir metinsel redaksiyonu temsil eder. |
| [PageRangeFilter](./pagerangefilter) | Belge içinde redaksiyon uygulanacak sayfa aralığını ayarlayan redaksiyon filtresini temsil eder. |
| [RedactionDescription](./redactiondescription) | Redaksiyon sürecinde gerçekleştirilen tek bir değişiklik eylemi bilgisini temsil eder. |
| [RedactionFilter](./redactionfilter) | Belge içinde redaksiyonların uygulanacağı kapsamı ayarlayan redaksiyon filtresini temsil eder. |
| [RegexRedaction](./regexredaction) | Sağlanan düzenli ifadeyi eşleştirerek belgede metni arayan ve değiştiren bir metin redaksiyonunu temsil eder. |
| [RegionReplacementOptions](./regionreplacementoptions) | Görüntü bölgesi değişimi için renk ve alan parametrelerini temsil eder. Bakınız [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Bir belgeden sayfa (slayt, çalışma sayfası vb.) kaldıran bir redaksiyonu temsil eder. |
| [ReplacementOptions](./replacementoptions) | Eşleşen metin değişimi için seçenekleri temsil eder. |
| [TextRedaction](./textredaction) | Belge metni redaksiyonları için temel soyut sınıfı temsil eder. |
| [TextReplacement](./textreplacement) | Metinsel bir değişim bilgisini temsil eder. |
## Arabirimler

| Arabirim | Açıklama |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Özel redaksiyon mantığını uygulamak için bir arayüz sağlar. |
| [IRedactionCallback](./iredactioncallback) | Her redaksiyon değişikliği hakkında bilgi almayı ve isteğe bağlı olarak engellemeyi gerektiren yöntemleri tanımlar. |
## Sıralama

| Sıralama | Açıklama |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Belge meta verisinin en yaygın türlerinin bir listesini temsil eder. |
| [PageSeekOrigin](./pageseekorigin) | Belge içinde arama yapmak için referans noktalarını temsil eden alanları sağlar. |
| [RedactionActionType](./redactionactiontype) | Redaksiyon gerçekleştirmek için yapılabilecek eylemleri temsil eder. |
| [RedactionType](./redactiontype) | Redaksiyon tarafından etkilenen belge verisinin bir türünü temsil eder. |
| [ReplacementType](./replacementtype) | Eşleşen metin için bir değişim türünü temsil eder. |

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->

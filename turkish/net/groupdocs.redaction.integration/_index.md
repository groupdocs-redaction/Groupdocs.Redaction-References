---
title: "GroupDocs.Redaction.Integration"
second_title: "GroupDocs.Redaction for .NET API Referansı"
description: "Integration ad alanı, farklı formatlardaki belgeleri GroupDocs.Redaction ile bütünleştirmek için kullanılan arabirimler ve sınıflar sağlar."
type: docs
weight: 40
url: /tr/net/groupdocs.redaction.integration/
---
Integration ad alanı, farklı formatlardaki belgeleri GroupDocs.Redaction ile bütünleştirmek için kullanılan arabirimler ve sınıflar sağlar.

## Sınıflar

| Sınıf | Açıklama |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Bir belgenin belirli bir formatını temsil eder. Kendi belge türlerinizi eklemek için bu sınıfı uygulayın. |
| [MetadataCollection](./metadatacollection) | Başlığını anahtar olarak kullanan bir [`MetadataItem`](../groupdocs.redaction.integration/metadataitem) sözlüğünü temsil eder. |
| [MetadataItem](./metadataitem) | Tüm desteklenen formatlar için ortak olan ve metadata redaksiyonlarında kullanılan bir metadata öğesini temsil eder. |
## Arabirimler

| Arabirim | Açıklama |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Yorumlar gibi ek açıklamalara erişim için gereken yöntemleri tanımlar. Ek açıklama redaksiyonlarını gerçekleştirmek için [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) türevi sınıfı tarafından uygulanması gerekir. |
| [ICellularFormatInstance](./icellularformatinstance) | Bir veya birden fazla çalışma sayfasına sahip elektronik tablo formatlarına erişim için gereken yöntemleri tanımlar. |
| [IFixedFormatDocument](./ifixedformatdocument) | Sabit yapıdaki erişim formatları, örneğin PDF veya sunumlar için gereken yöntemleri tanımlar. |
| [IImageFormatInstance](./iimageformatinstance) | Raster görüntü formatı redaksiyonları için gereken yöntemleri tanımlar. |
| [IMetadataAccess](./imetadataaccess) | Biçim destekliyorsa, bir belgenin meta verilerine erişim için gereken yöntemleri tanımlar. |
| [IPaginatedDocument](./ipaginateddocument) | Bir belgenin sayfalarını manipüle etmek için gereken yöntemleri tanımlar. Sayfa redaksiyonlarını gerçekleştirmek için [`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) türevi sınıfı tarafından uygulanması gerekir. |
| [IPreviewable](./ipreviewable) | Belgenin önizlemesini oluşturmak için yöntemleri tanımlar. |
| [IRasterizableDocument](./irasterizabledocument) | Belgeyi herhangi bir ikili biçimde kaydetmek için gereken yöntemleri tanımlar. Yerleşik tipler belgeyi sayfalarının görüntüleriyle bir PDF olarak kaydeder. |
| [ITextualFormatInstance](./itextualformatinstance) | Metin içeren herhangi bir belgede metinsel verileri redakte etmek için gereken yöntemleri tanımlar. |

<!-- DÜZENLEMEYİN: GroupDocs.Redaction.dll için xmldocmd tarafından oluşturuldu -->

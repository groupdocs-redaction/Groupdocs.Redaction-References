---
title: GroupDocs.Redaction.Integration
second_title: .NET API Başvurusu için GroupDocs.Redaction
description: Integrationad alanı farklı biçimlerdeki belgeleri GroupDocs.Redaction. ile entegre etmek için kullanılan arabirimler ve sınıflar sağlar
type: docs
weight: 40
url: /tr/net/groupdocs.redaction.integration/
---
Integrationad alanı, farklı biçimlerdeki belgeleri GroupDocs.Redaction. ile entegre etmek için kullanılan arabirimler ve sınıflar sağlar

## sınıflar

| Sınıf | Tanım |
| --- | --- |
| [DocumentFormatInstance](./documentformatinstance) | Belirli bir belge biçimini temsil eder. Kendi belge türlerinizi eklemek için bu sınıfı uygulayın. |
| [MetadataCollection](./metadatacollection) | Şunun sözlüğünü temsil eder:[`MetadataItem`](../groupdocs.redaction.integration/metadataitem) anahtar olarak başlığıyla. |
| [MetadataItem](./metadataitem) | Desteklenen tüm biçimler için ortak olan ve meta veri düzeltmelerinde kullanılan bir meta veri öğesini temsil eder. |
## Arayüzler

| Arayüz | Tanım |
| --- | --- |
| [IAnnotatedDocument](./iannotateddocument) | Açıklamalar gibi ek açıklamalara erişim için gerekli olan yöntemleri tanımlar. tarafından uygulanması gerekir[`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) açıklama redaksiyonları gerçekleştirmek için türetilmiş sınıf. |
| [ICellularFormatInstance](./icellularformatinstance) | Bir veya daha fazla çalışma sayfasına sahip elektronik tablo biçimlerine erişim için gerekli olan yöntemleri tanımlar. |
| [IImageFormatInstance](./iimageformatinstance) | Raster görüntü formatı redaksiyonları için gerekli olan yöntemleri tanımlar. |
| [IMetadataAccess](./imetadataaccess) | Biçim destekliyorsa, bir belgenin meta verilerine erişim için gerekli yöntemleri tanımlar. |
| [IPaginatedDocument](./ipaginateddocument) | Bir belgenin sayfalarını değiştirmek için gerekli yöntemleri tanımlar. tarafından uygulanması gerekir[`DocumentFormatInstance`](../groupdocs.redaction.integration/documentformatinstance) -türetilmiş sınıf sayfa redaksiyonları gerçekleştirmek için. |
| [IPreviewable](./ipreviewable) | Belgenin önizlemesini oluşturmak için yöntemleri tanımlar. |
| [IRasterizableDocument](./irasterizabledocument) | Belgeyi herhangi bir ikili biçimde kaydetmek için gerekli yöntemleri tanımlar. Yerleşik türler, bir belgeyi sayfalarının resimleriyle birlikte PDF olarak kaydeder. |
| [ITextualFormatInstance](./itextualformatinstance) | Metin içeren herhangi bir belgedeki metin verilerini yeniden düzenlemek için gerekli yöntemleri tanımlar. |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
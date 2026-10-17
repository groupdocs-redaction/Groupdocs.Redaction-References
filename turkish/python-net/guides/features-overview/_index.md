---
title: "Özellikler Genel Bakışı"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "GroupDocs.Redaction for Python via .NET, belgelerden tek, format bağımsız bir API aracılığıyla hassas bilgileri — metin, meta veri, görüntü alanları, açıklamalar ve tüm sayfalar — kaldırır ve sonucu orijinal formatta veya temizlenmiş bir PDF olarak kaydeder."
type: docs
url: /tr/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction for Python via .NET, geniş bir [supported document formats]() yelpazesinde hassas bilgileri kaldırır veya kalıcı olarak gizler. Her redaksiyon aynı iş akışını izler: bir belgeyi [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) ile açın, `apply()` ile bir veya daha fazla redaksiyon uygulayın, ardından temizlenmiş sonucu orijinal formatında veya temizlenmiş bir PDF olarak `save()` edin. Aşağıdaki yetenekler tek bir geçişte serbestçe birleştirilebilir.

## Text redaction

Metni tam bir ifade ya da düzenli ifade ile bul ve değiştir, tam kelimeler ve e-posta adresleri, telefon numaraları veya ulusal kimlik numaraları gibi karmaşık desenleri kapsar. Eşleşen metin, yerine başka bir metin konularak ya da renkli bir kutu ile kapatılarak orijinal içeriğin geri alınamaması sağlanabilir. Elektronik tablolarda aramayı tek bir çalışma sayfasına veya sütuna sınırlayabilirsiniz. See [Text Redactions]().

## Metadata redaction

Belge meta verilerini — yazar, başlık, şirket, yorumlar ve görüntülerdeki EXIF verileri — silin veya yeniden yazın, böylece hassas bilgiler belge özelliklerinden sızmaz. Tüm meta verileri temizleyebilir, belirli alanları hedefleyebilir veya değerleri yenileriyle değiştirebilirsiniz. See [Metadata Redactions]().

## Image-area redaction

Gömülü bir görüntünün veya taranmış bir sayfanın dikdörtgen bir bölgesini, belirli bir alana dolu bir kutu çizerek karartın — gizli verilerin bulunması muhtemel imzaları, fotoğrafları, başlıkları veya altbilgileri gizlemek için kullanışlıdır. See [Image Redactions]().

## Annotation redaction

Ek açıklamaları, yorumları ve notları yeniden yazın veya silin. Her ek açıklamayı kaldırabilir veya sadece hassas metin içerenleri eşleştirmek için düzenli ifade kullanabilirsiniz. See [Annotation Redactions]().

## Page removal

PDF belgelerinden, sunum slaytlarından ve elektronik tablo çalışma sayfalarından tüm sayfaları kaldırın. Başlangıç sayfasını ve sayısını, başlangıç noktasına göre yönüyle birlikte belirtirsiniz. See [Remove Page Redactions]().

## Rasterization to PDF

Temizlenmiş belgeyi sayfaları raster görüntüler olarak işlenen bir PDF olarak kaydedin. Oluşan dosya aranabilir metin içermez ve orijinal meta verileri taşımaz, böylece kaldırılan içerik geri alınamaz. Rasterleştirme, belgeyi üçüncü taraflara vermeniz gerektiğinde veya PDF gerektiren düzenlemelere uymanız gerektiğinde doğru seçimdir. Belirli sayfaları seçebilir ve gelişmiş rasterleştirme seçenekleri aracılığıyla PDF/A uyumluluğu talep edebilirsiniz. See [Save in Rasterized PDF]() and [Advanced Rasterization Options]().

## Redaction policies

Birçok redaksiyonu yeniden kullanılabilir bir politika içinde gruplayın ve aynı kural setini birçok belgeye tutarlı bir şekilde uygulayın — yayınlamadan önce standart bir alan kümesini temizleme gibi tekrarlayan görevler için idealdir. See [Use Redaction Policies]().

## Loading and saving

Belgeleri yerel bir yoldan veya bir akıştan yükleyin, şifre korumalı dosyalar dahil, ve isteğe bağlı olarak redaksiyon öncesinde belgeyi önceden rasterleştirin. Kaydederken, sonraki düzenleme için orijinal formatı koruyun, orijinal dosyanın üzerine yazın, PDF olarak rasterleştirin veya bir akışa yazın. See [Loading Documents]() and [Saving Documents]().

## On-premise

GroupDocs.Redaction for Python via .NET tamamen kendi altyapınızda çalışır — belgeleriniz ortamınızdan dışarı çıkmaz. Paket, ihtiyaç duyduğu her şeyi içinde barındıran bağımsız bir wheel'dir, bu yüzden Microsoft Office, OpenOffice, Adobe Acrobat veya ayrı bir çalışma zamanı kurmanız gerekmez. Desteklenen platformlar ve yerel bağımlılıklar için [System Requirements]() bölümüne bakın.

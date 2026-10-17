---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction لـ Java API Reference"
description: "توفر الحزمة فئات لأنواع مختلفة من الحذف."
type: docs
weight: 16
url: /ar/java/com.groupdocs.redaction.redactions/
---

توفر الحزمة فئات لأنواع مختلفة من الحذف.



## الفئات

| الفئة | الوصف |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | يمثل تشويهًا يستبدل نص التعليق (التعليقات، إلخ) الذي يطابق تعبيرًا نمطيًا معينًا. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | يمثل تشويه نصي يستبدل النص في مستندات جداول البيانات (CSV، Excel، إلخ). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | يوفر خيارًا لتحديد نطاق CellColumnRedaction إلى ورقة عمل وعمود. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | يوفر بيانات إدخال لـ [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | يمثل نتيجة تُرجعها [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | يمثل تشويهًا نصيًا يحذف التعليقات إذا كان النص يطابق تعبيرًا نمطيًا معينًا (يمكن حذف جميع التعليقات اختياريًا). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | يمثل تشويهًا للبيانات الوصفية يمحو جميع البيانات الوصفية أو البيانات الوصفية التي تطابق MetadataFilters المحددة من المستند. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | يمثل تشويهًا نصيًا يستبدل العبارة الدقيقة في نص المستند، غير حساس لحالة الأحرف بشكل افتراضي. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | يمثل تشويهًا يضع مستطيلًا ملونًا في المنطقة المحددة من مستند صورة. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | يمثل قائمة بأكثر أنواع البيانات الوصفية شيوعًا للمستند. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | يمثل فئة أساسية مجردة لإزالة بيانات تعريف المستند. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | يمثل إزالة بيانات تعريف تبحث وتزيل بيانات التعريف باستخدام التعبيرات النمطية، مطابقة المفاتيح و/أو القيم. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | يمثل مرشح الإزالة، يحدد منطقة داخل صفحة من المستند لتطبيق الإزالة. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | يمثل إزالة نصية معقدة تؤثر على النصوص والصور والتعليقات التوضيحية في منطقة من الصفحة. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | يمثل مرشح الإزالة، يحدد نطاق الصفحات داخل المستند لتطبيق الإزالة. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | يمثل معلومات إجراء تغيير واحد تم تنفيذها أثناء عملية الإزالة. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | يمثل مرشح الإزالة، يحدد النطاق داخل المستند لتطبيق الإزالة. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | يمثل نوعًا من بيانات المستند المتأثرة بالإزالة. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | يمثل إزالة نصية تبحث وتستبدل النص في المستند عن طريق مطابقة التعبير النمطي المقدم. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | يمثل معلمات اللون والمساحة لاستبدال منطقة الصورة. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | يمثل إزالة تزيل صفحة (شريحة، ورقة عمل، إلخ) من المستند. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | يمثل خيارات استبدال النص المطابق. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | يمثل فئة أساسية مجردة لإزالة نصوص المستند. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | يمثل معلومات استبدال نصية. |

## الواجهات

| الواجهة | الوصف |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | يحدد رد اتصال مخصص للإزالة. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | يحدد الطرق المطلوبة لتلقي المعلومات عن كل تغيير في الإزالة وإمكانية منعها. |

## التعدادات

| تعداد | الوصف |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | يوفر الحقول التي تمثل نقاط مرجعية في المستند للبحث. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | يمثل الإجراءات التي يمكن اتخاذها لتنفيذ الإزالة. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | يمثل نوعًا من الاستبدال للنص المطابق. |

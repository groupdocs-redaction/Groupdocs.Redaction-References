---
title: "Metered класс"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Управляет измеряемым (по‑использованию) лицензированием."
type: docs
url: /ru/python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

Управляет измеряемым (по‑использованию) лицензированием.

Лицензии Metered тарифицируются по фактическому потреблению (обычно страниц или
обработанных документов). Установите пару публичного/приватного ключа один раз в
запуске приложения; обёртка отправляет данные об использовании обратно в GroupDocs
лицензионный сервер в фоновом режиме.

Тип Metered раскрывает следующие члены:

### Методы
| Метод | Описание |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | Верните оставшийся измеряемый кредит для текущего ключа. |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | Верните общее измеряемое количество, потребленное до сих пор. |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | Активируйте измеряемую оплату с помощью данной пары публичного/приватного ключа. |

### См. также
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)

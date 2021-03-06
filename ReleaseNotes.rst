﻿История изменений API
=====================
24.04.2018
---------------------

В связи с внесенными изменениями в структуру :doc:`BoxEvent<../structures/BoxEvent>`, обновлена :doc:`рекомендованная схема обращения к API<../OperationScheme>`: при необходимости получить список новых событий, начиная с определенного события, при отправке запроса GetEvents, в параметре exclusiveEventId необходимо использовать указатель **EventPointer**. Использование идентификатора EventId в качестве значения параметра exclusiveEventId в последующих обновлениях поддерживаться не будет.

Обновлены описания событий и структур:

- в :doc:`BoxEvent<../structures/BoxEvent>` добавлен указатель на событие EventPointer,
- в описания событий, связанных с документами в Диадоке, добавлена функция УПД UniversalDocumentFunction,
- добавлены описания событий :doc:`ProcessingTimesReportEvent<../structures/events/ProcessingTimesReportEventContent>` и :doc:`DiadocDocumentDeliveredEvent<../structures/events/DiadocDocumentDeliveredEventContent>`,
- исправлены опечатки и неточности.


29.05.2017
---------------------

У документации API EDI.Контур изменился интерфейс. В новом интерфейсе реализованы:

- удобное древовидное меню,
- система поиска по страницам,
- страница с описанием изменений.

Если вы заметили в документации ошибку, вы можете предложить ее исправление, нажав на ссылку "Edit on GitHub" на соответствующей странице.
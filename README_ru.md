<div align="center">

<a href="https://evolink.ai/gemini-omni?utm_source=github&utm_medium=banner&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=readme_banner"><img src="image/guide-banner.png" width="760" alt="Руководство и библиотека промптов Gemini Omni"></a>

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Попробовать Gemini Omni 1.2 Flash](https://img.shields.io/badge/Try_Gemini_Omni_1.2_Flash-EvoLink-black)](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=badge&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=model_try)

[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Default_Source-111111)](README.md) [![🇪🇸 Español](https://img.shields.io/badge/🇪🇸_Español-Ver-ffb703)](README_es.md) [![🇵🇹 Português](https://img.shields.io/badge/🇵🇹_Português-Ver-2a9d8f)](README_pt.md) [![🇯🇵 日本語](https://img.shields.io/badge/🇯🇵_日本語-表示-52b788)](README_ja.md) [![🇰🇷 한국어](https://img.shields.io/badge/🇰🇷_한국어-보기-4ea8de)](README_ko.md) [![🇩🇪 Deutsch](https://img.shields.io/badge/🇩🇪_Deutsch-Ansehen-f4a261)](README_de.md) [![🇫🇷 Français](https://img.shields.io/badge/🇫🇷_Français-Voir-e76f51)](README_fr.md) [![🇹🇷 Türkçe](https://img.shields.io/badge/🇹🇷_Türkçe-Görüntüle-d62828)](README_tr.md) [![🇹🇼 繁體中文](https://img.shields.io/badge/🇹🇼_繁體中文-查看-8338ec)](README_zh-TW.md) [![🇨🇳 简体中文](https://img.shields.io/badge/🇨🇳_简体中文-查看-ef476f)](README_zh-CN.md) [![🇷🇺 Русский](https://img.shields.io/badge/🇷🇺_Русский-Смотреть-577590)](README_ru.md)

</div>

# Gemini Omni 1.2 Flash: руководство и библиотека промптов

## 🍌 Введение
**Руководство по Gemini Omni 1.2 Flash с сохранённой библиотекой промптов, демонстраций редактирования, сравнений и видео сообщества для семейства Gemini Omni.** Руководство помогает авторам и разработчикам выбрать задачу и разобраться в ограничениях входных и выходных данных.

> [!NOTE]
> Прежние кейсы с промптами, сравнения и галерея сообщества — исторические материалы семейства Gemini Omni. Их исходные промпты, источники и медиа сохранены; они не представлены как результаты или бенчмарки Gemini Omni 1.2 Flash.

<a id="omni-1-2-guide"></a>
## 🆕 Gemini Omni 1.2 Flash

Google указывает, что Gemini Omni 1.2 Flash находится в общем доступе (GA) с **5 ноября 2026 года**. Главные изменения по сравнению с версией 1.1 — генерация до **15 секунд** в соответствующих API-маршрутах и **отдельное повышение разрешения видео**. См. [спецификацию модели Google](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-1-2-flash) и [объявление EvoLink от 5 ноября](https://evolink.ai/changelog?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=release_source#2026-11-05-gemini-omni-1-2-flash).

- На входе — текст, изображения и видео; на выходе — видео с синхронизированной речью, музыкой и звуковыми эффектами. Аудиофайлы на входе и редактирование звука не поддерживаются.
- Нативный вывод в **360p / 720p**; **1080p / 4K достигаются повышением разрешения**, а не нативной генерацией в 4K. Документированный вывод — 24 кадра в секунду, 16:9 или 9:16.
- Генерация видео по тексту и по одному начальному кадру поддерживает **3–15 секунд**. Интерполяция между первым и последним кадрами остаётся в пределах **3–10 секунд**.
- Продление добавляет **3–10 секунд**; это добавленная длительность, а не общая длина готового видео.

### Выбор задачи EvoLink

Для каждой задачи приведена ссылка на её контракт запроса. Прочитайте [полную документацию параметров](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=parameter_overview) перед сменой API-маршрута.

| Задача | Когда использовать | Ограничения API-маршрута |
| :--- | :--- | :--- |
| [Читать документацию генерации по тексту](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-text-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_text) | Создать план по текстовому промпту. | 3–15 секунд. |
| [Читать документацию генерации по изображениям](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-image-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_image) | Анимировать начальный кадр или соединить первый и последний кадры. | Одно изображение: 3–15 секунд; два изображения: 3–10 секунд. |
| [Читать документацию генерации по референсам](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-reference-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_reference) | Задать направление нового плана с помощью изображений и видео-референсов. | До 10 изображений и 3 видео-референсов; при длительности более 10 секунд — не более 1 видео-референса. |
| [Читать документацию редактирования видео](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-edit?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_edit) | Изменить существующий клип с помощью промпта. | Одно входное видео до 15 секунд; изображения-референсы необязательны; качество по умолчанию — `auto`. |
| [Читать документацию продления видео](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-extend?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_extend) | Продолжить клип с его конца. | Одно входное видео до 30 секунд; добавляется 3–10 секунд. |
| [Читать документацию повышения разрешения видео](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-upscale?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_upscale) | Повысить разрешение выбранного готового клипа. | Входное видео до 15 секунд с поддерживаемым стандартным размером; без промпта. См. различия между платформами ниже. |

### Различия между платформами и версиями

- **Референсы:** [Руководство по использованию AI Studio](https://aistudio.google.com/docs/omni) допускает до 6 изображений, тогда как Google Cloud и EvoLink документируют до 10. Ограничения видео-референсов также зависят от длительности вывода; используйте контракт выбранной платформы.
- **Повышение разрешения:** Google Cloud документирует 360p→720p/1080p и 720p→1080p/4K и исключает 1080p→4K. В документации EvoLink также указан вариант 1080p→4K. Уточните поддержку этой дополнительной пары на выбранной платформе; она не гарантирована для всех платформ. См. [ограничения Google на повышение разрешения](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/video/upscale-videos).
- **Состояние диалога:** Interactions API Google поддерживает редактирование в диалоге. Асинхронные видеозадачи EvoLink используют собственный контракт запроса; не переносите в них `previous_interaction_id` и другие параметры, предназначенные только для Google.
- **Миграция:** [Страница модели Google](https://aistudio.google.com/docs/models/gemini-omni-flash) указывает, что 3 декабря 2026 года стабильный ID 1.1 в Gemini API начнёт перенаправлять запросы на версию 1.2. Это не подтверждает миграцию API-маршрутов EvoLink версии 1.1. Выбирайте явную задачу версии 1.2, а не считайте старый общий ID её псевдонимом.
- **Стоимость:** На странице модели EvoLink указана тарификация по токенам; ставка за токен не является фиксированной ценой за секунду или за готовый клип. Перед оценкой стоимости задачи проверьте текущий API-маршрут, разрешение и фактическое использование.

Источники проверены **6 ноября 2026 года**.

<a id="quick-start"></a>
## ⚡ Быстрый старт

[Попробовать Gemini Omni 1.2 Flash в браузере](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=browser_try) или [прочитать актуальную документацию задач](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=task_docs).

Выберите генерацию видео по тексту, генерацию по изображению, работу с референсами, редактирование, продление или повышение разрешения в таблице задач выше. Следуйте актуальной документации выбранной задачи: в ней описаны входные данные, ограничения и порядок получения результата.

## 📑 Меню
- [Руководство по Gemini Omni 1.2 Flash](#omni-1-2-guide)
- [Быстрый старт](#quick-start)
- [Официальные демонстрации Gemini Omni 1.2](#omni12-demos)
- [🎯 Ингредиенты промптов](#-ингредиенты-промптов)
- [✂️ Редактирование](#️-редактирование)
  - [🔄 Замена элементов](#-замена-элементов)
    - [Кейс 1: Бабочка в пчелу](#кейс-1-бабочка-в-пчелу)
    - [Кейс 2: Пчела в светлячков](#кейс-2-пчела-в-светлячков)
    - [Кейс 3-5: Серия «Космические корабли и астронавт»](#кейс-3-5-серия-космические-корабли-и-астронавт)
    - [Кейс 6: Трансформация поезда 1896 (от @emollick)](#кейс-6-трансформация-поезда-1896-от-emollick)
    - [Кейс 7: Удаление человека из видео (от @arrakis_ai)](#кейс-7-удаление-человека-из-видео-от-arrakis_ai)
    - [Кейс 8: Невидимая скрипка](#кейс-8-невидимая-скрипка)
    - [Кейс 9: Смена локации через знание мира (от @venturetwins)](#кейс-9-смена-локации-через-знание-мира-от-venturetwins)
    - [Кейс 10: Анимация в реальную съёмку (от @arrakis_ai)](#кейс-10-анимация-в-реальную-съёмку-от-arrakis_ai)
  - [🎬 Базовая сцена](#-базовая-сцена)
    - [Кейс 1: Базовый кадр скрипача](#кейс-1-базовый-кадр-скрипача)
  - [📷 Управление камерой](#-управление-камерой)
    - [Кейс 1: Ракурс через плечо](#кейс-1-ракурс-через-плечо)
    - [Кейс 2: Наклон камеры от обуви к среднему плану](#кейс-2-наклон-камеры-от-обуви-к-среднему-плану)
    - [Кейс 3: Гиперлапс-селфи из путешествия (от @ZaraIrahh)](#кейс-3-гиперлапс-селфи-из-путешествия-от-zarairahh)
    - [Кейс 4: Дрон-съёмка моды (от @ariaxawan)](#кейс-4-дрон-съёмка-моды-от-ariaxawan)
    - [Кейс 5: Вид сверху с вращением на 360° (от @npaka123)](#кейс-5-вид-сверху-с-вращением-на-360-от-npaka123)
    - [Кейс 6: Omnizoom — Погружение в фото (от @alexanderchen)](#кейс-6-omnizoom--погружение-в-фото-от-alexanderchen)
  - [🎬 Действие и синхронизация](#-действие-и-синхронизация)
    - [Кейс 1: Звук игрушечного животного](#кейс-1-звук-игрушечного-животного)
    - [Кейс 2: Синхронизация огней квартир](#кейс-2-синхронизация-огней-квартир)
    - [Кейс 3: Цепная реакция с шариком](#кейс-3-цепная-реакция-с-шариком)
    - [Кейс 4: Огни зданий](#кейс-4-огни-зданий)
    - [Кейс 5: Реалистичный боксёрский бой (от @RuzainaMeer)](#кейс-5-реалистичный-боксёрский-бой-от-ruzainameer)
- [🎨 Продвинутый мультимодальный режим](#-продвинутый-мультимодальный-режим)
  - [🪞 Художественный стиль](#-художественный-стиль)
    - [Кейс 1-3: Серия «Зеркало»](#кейс-1-3-серия-зеркало)
    - [Кейс 4: Анимационная реклама в один кадр (от @DenneyDara)](#кейс-4-анимационная-реклама-в-один-кадр-от-denneydara)
    - [Кейс 5: Изоляция линейного рисунка (от @alexanderchen)](#кейс-5-изоляция-линейного-рисунка-от-alexanderchen)
  - [✨ Визуальные эффекты](#-визуальные-эффекты)
    - [Кейс 1: Суперзум через отверстие в руке](#кейс-1-суперзум-через-отверстие-в-руке)
    - [Кейс 2: Эффекты движения скейтборда](#кейс-2-эффекты-движения-скейтборда)
    - [Кейс 3: AR HUD-наложение (от @jerrod_lew)](#кейс-3-ar-hud-наложение-от-jerrod_lew)
  - [🔗 Кросс-модальность](#-кросс-модальность)
    - [Кейс 1: Перенос в новое окружение](#кейс-1-перенос-в-новое-окружение)
    - [Кейс 2: Форма птиц со звуком](#кейс-2-форма-птиц-со-звуком)
    - [Кейс 3: От слайда к движению (от @yoshifujidesign)](#кейс-3-от-слайда-к-движению-от-yoshifujidesign)
    - [Кейс 4: Изометрический персонаж-повар с референсным изображением (от @kumiko_shiraki)](#кейс-4-изометрический-персонаж-повар-с-референсным-изображением-от-kumiko_shiraki)
    - [Кейс 5: Картинка с инструкциями из ChatGPT как ввод (от @Majin_AppSheet)](#кейс-5-картинка-с-инструкциями-из-chatgpt-как-ввод-от-majin_appsheet)
    - [Кейс 6: Иллюстрация ChatGPT в анимацию Omni (от @mmmiyama_D)](#кейс-6-иллюстрация-chatgpt-в-анимацию-omni-от-mmmiyama_d)
  - [📋 Раскадровка](#-раскадровка)
    - [Кейс 1: Реклама люксовой косметики (от @aiwithaly)](#кейс-1-реклама-люксовой-косметики-от-aiwithaly)
    - [Кейс 2: Покажи меня в этой истории](#кейс-2-покажи-меня-в-этой-истории)
    - [Кейс 3: Разделённый экран 3x3 (от @alexanderchen)](#кейс-3-разделённый-экран-3x3-от-alexanderchen)
    - [Кейс 4: Повтор действия с разных ракурсов (от @jerrod_lew)](#кейс-4-повтор-действия-с-разных-ракурсов-от-jerrod_lew)
    - [Кейс 5: Видео с разделённым экраном (от @jerrod_lew)](#кейс-5-видео-с-разделённым-экраном-от-jerrod_lew)
  - [🔤 Рендеринг текста](#-рендеринг-текста)
    - [Кейс 1: Последовательность предметов по алфавиту](#кейс-1-последовательность-предметов-по-алфавиту)
    - [Кейс 2: Пословная синхронизация текста](#кейс-2-пословная-синхронизация-текста)
    - [Кейс 3: Рендеринг текста — новости ИИ (от @chrisfirst)](#кейс-3-рендеринг-текста--новости-ии-от-chrisfirst)
    - [Кейс 4: Показ мод шрифтов (от @HBCoop_)](#кейс-4-показ-мод-шрифтов-от-hbcoop_)
- [⚖️ Сравнение](#️-сравнение)
  - [Кейс 1: Seedance 2.0 vs Gemini Omni Flash (от @JSFILMZ0412)](#кейс-1-seedance-20-vs-gemini-omni-flash-от-jsfilmz0412)
  - [Кейс 2: Gemini Omni vs Seedance 2.0 — экшн-сцены (от @CuriousRefuge)](#кейс-2-gemini-omni-vs-seedance-20--экшн-сцены-от-curiousrefuge)
- [🧪 Оценка](#-оценка)
  - [Кейс 1: Оценка качества Gemini Omni (от @kenichiota0711)](#кейс-1-оценка-качества-gemini-omni-от-kenichiota0711)
- [🌐 Галерея сообщества](#-галерея-сообщества)
- [Связанные репозитории](#related-repositories)
- [🙏 Благодарности](#-благодарности)

<a id="omni12-demos"></a>
## 🎬 Демонстрации Gemini Omni 1.2

Восемь официальных демонстраций, опубликованных Google **5 ноября 2026 года**. Прочитайте [оригинальную статью о запуске](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/); нажмите на изображение предпросмотра, чтобы посмотреть исходное видео Google.

<table>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-1"></a>
**[Виртуальная примерка длительностью 15 секунд](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)**

[![Виртуальная примерка длительностью 15 секунд](image/omni-1.2/15-second-virtual-try-on.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)

Одна фотография модели и три комплекта одежды задают 15-секундный монтаж виртуальной примерки.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-2"></a>
**[Послойная типографическая анимация](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)**

[![Послойная типографическая анимация](image/omni-1.2/layered-typography-animation.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)

Анимированный плакат собирает материалы и надписи; Google показывает результаты версий 1.1 и 1.2.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-3"></a>
**[Смена фона в диалоге](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)**

[![Смена фона в диалоге](image/omni-1.2/conversational-background-changes.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)

Последовательные диалоги меняют фон клипа, сохраняя двух персонажей в доспехах.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-4"></a>
**[Непрерывный пролёт через Пантеон](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)**

[![Непрерывный пролёт через Пантеон](image/omni-1.2/continuous-pantheon-flythrough.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)

Две архитектурные фотографии направляют непрерывный пролёт камеры через купол Пантеона.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-5"></a>
**[15-секундный ролик об улье](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)**

[![15-секундный ролик об улье](image/omni-1.2/15-second-beehive-explainer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)

Один стилевой кадр превращается в 15-секундный иллюстрированный ролик об улье из четырёх планов.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-6"></a>
**[Перенос движения от осьминога к танцовщице](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)**

[![Перенос движения от осьминога к танцовщице](image/omni-1.2/octopus-to-dancer-motion-transfer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)

Последующее редактирование переносит плавное движение осьминога на платье танцовщицы.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-7"></a>
**[Раменная: от первого к последнему кадру](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)**

[![Раменная: от первого к последнему кадру](image/omni-1.2/first-to-last-frame-ramen-shop.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)

Первый и последний кадры соединяют внешний и внутренний вид раменной; в сравнении Google видны несоответствия.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-8"></a>
**[Непрерывное отдаление от острова](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)**

[![Непрерывное отдаление от острова](image/omni-1.2/continuous-island-zoom-out.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)

За один десятисекундный план камера отдаляется от крупного плана берега до общего вида острова.

</td>
</tr>
</table>

## 🎯 Ингредиенты промптов
Gemini Omni обладает глубоким **пониманием мира** — модель опирается на реальные знания из истории, науки и культуры. Вам не нужно объяснять каждую деталь. Вместо этого выразите свой творческий замысел на естественном языке, и Omni дополнит остальное своими рассуждениями.
При создании нового видео с нуля комбинируйте эти параметры для управления результатом:
| Параметр | Что указывать | Пример |
| :--- | :--- | :--- |
| **Кадрирование и движение** | Широкий угол, средний или крупный план. Траектория камеры: плавное скольжение, резкий наезд, статичная фиксация, долли-зум и т.д. | `A close-up tracking shot smoothly pushing in` |
| **Стиль** | Общее визуальное художественное направление | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **Освещение** | Настроение сцены и схема освещения | `Warm champagne lighting`, `dim overhead gym lights` |
| **Локация** | Окружение и фон | `Small underground gym`, `futuristic neon cityscape` |
| **Действие** | Поведение и движение объекта | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **Итеративное редактирование:** Omni поддерживает многоходовое редактирование в диалоге. Модель сохраняет то, что работает, и изменяет только то, что вы просите — не нужно заново описывать всю сцену каждый раз. Просто скажите, что изменить дальше.

> [!TIP]
> **[Сохранить неизмененные области](https://x.com/tanabe_fragm/status/2058103447006896406) (от [@tanabe_fragm](https://x.com/tanabe_fragm)):** При редактировании видео добавьте фразы вроде "Не меняй ничего больше" или "Оставь всё остальное как есть" в ваш prompt. Это значительно снижает нежелательные изменения частей, которые вы не собирались модифицировать.
>
> https://github.com/user-attachments/assets/285ee7d8-7dfe-4304-a9a4-648026073b80

## ✂️ Редактирование

### 🔄 Замена элементов

<a id="кейс-1-бабочка-в-пчелу"></a>
### Кейс 1: Бабочка в пчелу `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**Промпт:**

```
Change the butterfly to a bee.
```

---

<a id="кейс-2-пчела-в-светлячков"></a>
### Кейс 2: Пчела в светлячков `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**Промпт:**

```
Change the bee into a small swarm of fireflies.
```

---

<a id="кейс-3-5-серия-космические-корабли-и-астронавт"></a>
### Кейс 3-5: Серия «Космические корабли и астронавт» `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**Вход:**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

### Кейс 3: Корабли в белое оригами

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

### Кейс 4: Астронавт в морскую анемону

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

### Кейс 5: Малые корабли в скатов

</td>
</tr>
</table>

**Промпты:**

```
Case 3: Change the ships to be made from white origami paper.
```

```
Case 4: Change the astronaut to a sea anemone.
```

```
Case 5: Change the small ships to stingrays.
```

---

<a id="кейс-6-трансформация-поезда-1896-от-emollick"></a>
### Кейс 6: [Трансформация поезда 1896](https://x.com/emollick/status/2057874739817808223) (от [@emollick](https://x.com/emollick)) `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Промпт:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

---

<a id="кейс-7-удаление-человека-из-видео-от-arrakis_ai"></a>
### Кейс 7: [Удаление человека из видео](https://x.com/arrakis_ai/status/2057939231755178439) (от [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Промпт:**

```
Remove the person from this video perfectly.
```

---

<a id="кейс-8-невидимая-скрипка"></a>
### Кейс 8: Невидимая скрипка `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**Промпт:**

```
Make the violin invisible
```

---

<a id="кейс-9-смена-локации-через-знание-мира-от-venturetwins"></a>
### Кейс 9: [Смена локации через знание мира](https://x.com/venturetwins/status/2058235415883313361) (от [@venturetwins](https://x.com/venturetwins)) `🎬 Video→Video`

https://github.com/user-attachments/assets/daa90750-fc7b-49ea-b85d-364411159663

**Промпт:**

```
Re-shoot this video in [location] based on the screenshot from Google Maps.
```

> Загружено видео поездки Waymo, затем Omni попросили пересъемку в разных локациях с использованием скриншотов Google Maps. Модель использует свои знания о мире для бесшовной смены окружений.

---

<a id="кейс-10-анимация-в-реальную-съёмку-от-arrakis_ai"></a>
### Кейс 10: [Анимация в реальную съёмку](https://x.com/arrakis_ai/status/2058488373057302797) (от [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/3c6be2a9-3e67-4deb-8ccd-fb493b715f65

**Промпт:**

```
Turn this animation into live action.
```

### 🎬 Базовая сцена

<a id="кейс-1-базовый-кадр-скрипача"></a>
### Кейс 1: Базовый кадр скрипача `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Промпт:**

```
A video of a violinist playing a song.
```

### 📷 Управление камерой

<a id="кейс-1-ракурс-через-плечо"></a>
### Кейс 1: Ракурс через плечо `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**Промпт:**

```
Change the camera angle to be over the violinist's shoulder.
```

---

<a id="кейс-2-наклон-камеры-от-обуви-к-среднему-плану"></a>
### Кейс 2: Наклон камеры от обуви к среднему плану `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/19dbc1ae-1e9e-4b7b-9069-e979fffe3651

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**Промпт:**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

<a id="кейс-3-гиперлапс-селфи-из-путешествия-от-zarairahh"></a>
### Кейс 3: [Гиперлапс-селфи из путешествия](https://x.com/ZaraIrahh/status/2057775215749349520) (от [@ZaraIrahh](https://x.com/ZaraIrahh)) `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Промпт:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

---

<a id="кейс-4-дрон-съёмка-моды-от-ariaxawan"></a>
### Кейс 4: [Дрон-съёмка моды](https://x.com/ariaxawan/status/2057794715744084042) (от [@ariaxawan](https://x.com/ariaxawan)) `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Промпт:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

---

<a id="кейс-5-вид-сверху-с-вращением-на-360-от-npaka123"></a>
### Кейс 5: [Вид сверху с вращением на 360°](https://x.com/npaka123/status/2058033145845575735) (от [@npaka123](https://x.com/npaka123)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Промпт:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

---

<a id="кейс-6-omnizoom--погружение-в-фото-от-alexanderchen"></a>
### Кейс 6: [Omnizoom — Погружение в фото](https://x.com/alexanderchen/status/2058330610574221672) (от [@alexanderchen](https://x.com/alexanderchen)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/9fd3ad2a-6e4a-4ac0-ab29-48f1c303b95f

**Промпт:**

```
Omnizoom — diving into a photo.
```

### 🎬 Действие и синхронизация

<a id="кейс-1-звук-игрушечного-животного"></a>
### Кейс 1: Звук игрушечного животного `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Промпт:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

<a id="кейс-2-синхронизация-огней-квартир"></a>
### Кейс 2: Синхронизация огней квартир `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/6fa879c3-5ee8-4ff1-bbe9-6648d750277d

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**Промпт:**

```
The lights of the apartments start turning on in sync with the music.
```

---

<a id="кейс-3-цепная-реакция-с-шариком"></a>
### Кейс 3: Цепная реакция с шариком `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Промпт:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

<a id="кейс-4-огни-зданий"></a>
### Кейс 4: Огни зданий `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**Промпт:**

```
The lights of the buildings start turning on in sync with the music.
```

---

<a id="кейс-5-реалистичный-боксёрский-бой-от-ruzainameer"></a>
### Кейс 5: [Реалистичный боксёрский бой](https://x.com/RuzainaMeer/status/2057785474446741728) (от [@RuzainaMeer](https://x.com/RuzainaMeer)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Промпт:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

## 🎨 Продвинутый мультимодальный режим

### 🪞 Художественный стиль

<a id="кейс-1-3-серия-зеркало"></a>
### Кейс 1-3: Серия «Зеркало» `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

### Кейс 1: Зеркало — рябь жидкого металла

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

### Кейс 2: Зеркало — линейный рисунок

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

### Кейс 3: Зеркало — кукла

</td>
</tr>
</table>

**Промпты:**

```
Case 1: When the person touches the mirror, make the mirror ripple beautifully like liquid, and the person's arm turns into reflective mirror material
```

```
Case 2: When the person touches the mirror, the person transforms into a detailed monochrome line art drawing
```

```
Case 3: When the person touches the mirror, the person suddenly transforms into a cute felted stuffed puppet version with large googley eyes and glasses
```

---

<a id="кейс-4-анимационная-реклама-в-один-кадр-от-denneydara"></a>
### Кейс 4: [Анимационная реклама в один кадр](https://x.com/DenneyDara/status/2057844409639551380) (от [@DenneyDara](https://x.com/DenneyDara)) `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Промпт:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

---

<a id="кейс-5-изоляция-линейного-рисунка-от-alexanderchen"></a>
### Кейс 5: [Изоляция линейного рисунка](https://x.com/alexanderchen/status/2057925025915666673) (от [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Промпт:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

### ✨ Визуальные эффекты

<a id="кейс-1-суперзум-через-отверстие-в-руке"></a>
### Кейс 1: Суперзум через отверстие в руке `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Промпт:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

<a id="кейс-2-эффекты-движения-скейтборда"></a>
### Кейс 2: Эффекты движения скейтборда `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Промпт:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

<a id="кейс-3-ar-hud-наложение-от-jerrod_lew"></a>
### Кейс 3: [AR HUD-наложение](https://x.com/jerrod_lew/status/2058337271947079977) (от [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/04b11cd7-d345-4172-b6e5-38301e73bb77

**Промпт:**

```
Create a virtual HUD and UI overlay for this recorded phone video, like an AR glasses experience with secondary screens.
```

### 🔗 Кросс-модальность

<a id="кейс-1-перенос-в-новое-окружение"></a>
### Кейс 1: Перенос в новое окружение `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**Промпт:**

```
Transport the violinist to the image environment
```

---

<a id="кейс-2-форма-птиц-со-звуком"></a>
### Кейс 2: Форма птиц со звуком `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**Входное видео:**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**Входное изображение:**

<img src="image/crossmodal-01.webp" width="200">

**Входное аудио:**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**Промпт:**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

<a id="кейс-3-от-слайда-к-движению-от-yoshifujidesign"></a>
### Кейс 3: [От слайда к движению](https://x.com/yoshifujidesign/status/2058032203175731293) (от [@yoshifujidesign](https://x.com/yoshifujidesign)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Промпт:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

---

<a id="кейс-4-изометрический-персонаж-повар-с-референсным-изображением-от-kumiko_shiraki"></a>
### Кейс 4: [Изометрический персонаж-повар с референсным изображением](https://x.com/kumiko_shiraki/status/2058337185099546885) (от [@kumiko_shiraki](https://x.com/kumiko_shiraki)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/d5e9b97e-cefa-4cd8-bf70-4e633020f092

**Промпт:**

```
Narrow down reference images and add negative prompts to get closer to your ideal output.
```

> Техника: когда сгенерированное видео не соответствует вашему видению, (1) сузьте набор референсных изображений и (2) добавьте негативные промпты для подавления нежелательных элементов.

---

<a id="кейс-5-картинка-с-инструкциями-из-chatgpt-как-ввод-от-majin_appsheet"></a>
### Кейс 5: [Картинка с инструкциями из ChatGPT как ввод](https://x.com/Majin_AppSheet/status/2058191091070058846) (от [@Majin_AppSheet](https://x.com/Majin_AppSheet)) `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Вход (картинка-инструкция из ChatGPT):**

<img src="image/049_majin_appsheet_instruction_image_photo_0.jpg" width="280">

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/578d6968-c6dd-417a-b6fe-100468851f3d

</td>
</tr>
</table>

> Рабочий процесс: создайте изображения-инструкции/раскадровки в ChatGPT, затем передайте их напрямую в Gemini Omni как визуальные промпты.

---

<a id="кейс-6-иллюстрация-chatgpt-в-анимацию-omni-от-mmmiyama_d"></a>
### Кейс 6: [Иллюстрация ChatGPT в анимацию Omni](https://x.com/mmmiyama_D/status/2058654389326516656) (от [@mmmiyama_D](https://x.com/mmmiyama_D)) `🖼️ Image→Video`

<table>
<tr>
<td width="280">

https://github.com/user-attachments/assets/5759f07e-6b2a-4b7d-bb36-52e960a6559e

</td>
<td width="280">

https://github.com/user-attachments/assets/b4fea213-9a0e-46c9-8a6e-9e98b566ffab

</td>
<td width="280">

https://github.com/user-attachments/assets/289e5378-60ad-472b-ba51-da710da81270

</td>
</tr>
</table>

> Рабочий процесс: создайте иллюстративные схемы с помощью генерации изображений ChatGPT → анимируйте их с помощью Gemini Omni. Качество рендеринга текста можно улучшить, добавив специфические промпты для подавления искажений текста.

### 📋 Раскадровка

<a id="кейс-1-реклама-люксовой-косметики-от-aiwithaly"></a>
### Кейс 1: [Реклама люксовой косметики](https://x.com/aiwithaly/status/2057806821138858314) (от [@aiwithaly](https://x.com/aiwithaly)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Промпт:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

---

<a id="кейс-2-покажи-меня-в-этой-истории"></a>
### Кейс 2: Покажи меня в этой истории `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Вход:**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**Выход:**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**Промпт:**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

<a id="кейс-3-разделённый-экран-3x3-от-alexanderchen"></a>
### Кейс 3: [Разделённый экран 3x3](https://x.com/alexanderchen/status/2057861567396368841) (от [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Промпт:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

---

<a id="кейс-4-повтор-действия-с-разных-ракурсов-от-jerrod_lew"></a>
### Кейс 4: [Повтор действия с разных ракурсов](https://x.com/jerrod_lew/status/2057838324140953773) (от [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Промпт:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

---

<a id="кейс-5-видео-с-разделённым-экраном-от-jerrod_lew"></a>
### Кейс 5: [Видео с разделённым экраном](https://x.com/jerrod_lew/status/2057944349846249975) (от [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Промпт:**

```
Use a reference video and ask the agent for a split screen video.
```

### 🔤 Рендеринг текста

<a id="кейс-1-последовательность-предметов-по-алфавиту"></a>
### Кейс 1: Последовательность предметов по алфавиту `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Промпт:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

<a id="кейс-2-пословная-синхронизация-текста"></a>
### Кейс 2: Пословная синхронизация текста `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Промпт:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

<a id="кейс-3-рендеринг-текста--новости-ии-от-chrisfirst"></a>
### Кейс 3: [Рендеринг текста — новости ИИ](https://x.com/chrisfirst/status/2057863432469361098) (от [@chrisfirst](https://x.com/chrisfirst)) `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Промпт:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

---

<a id="кейс-4-показ-мод-шрифтов-от-hbcoop_"></a>
### Кейс 4: [Показ мод шрифтов](https://x.com/HBCoop_/status/2057856570558452142) (от [@HBCoop_](https://x.com/HBCoop_)) `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Промпт:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

## ⚖️ Сравнение

<a id="кейс-1-seedance-20-vs-gemini-omni-flash-от-jsfilmz0412"></a>
### Кейс 1: [Seedance 2.0 vs Gemini Omni Flash](https://x.com/JSFILMZ0412/status/2057926749598736635) (от [@JSFILMZ0412](https://x.com/JSFILMZ0412)) `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — сравнение переноса стиля, качества движения и цензуры.

---

<a id="кейс-2-gemini-omni-vs-seedance-20--экшн-сцены-от-curiousrefuge"></a>
### Кейс 2: [Gemini Omni vs Seedance 2.0 — экшн-сцены](https://x.com/CuriousRefuge/status/2057929340562907451) (от [@CuriousRefuge](https://x.com/CuriousRefuge)) `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Модель видеоредактирования Gemini Omni vs Seedance 2.0 — сравнение масштабных экшн-сцен.

## 🧪 Оценка

<a id="кейс-1-оценка-качества-gemini-omni-от-kenichiota0711"></a>
### Кейс 1: [Оценка качества Gemini Omni](https://x.com/kenichiota0711/status/2057820346850660769) (от [@kenichiota0711](https://x.com/kenichiota0711)) `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

## 🌐 Галерея сообщества

Творческие эксперименты и витрины из сообщества. Эти кейсы демонстрируют широту возможностей Gemini Omni.

<table>
<tr>
<td width="50%" valign="top">

**[Концептуальное учебное видео](https://x.com/VORTEX_Promos/status/2058083405204459621)** — от [@VORTEX_Promos](https://x.com/VORTEX_Promos)

https://github.com/user-attachments/assets/ca450aec-a6c8-455f-973d-087bfb3da742

</td>
<td width="50%" valign="top">

**[Showcase](https://x.com/paji_a/status/2058070248436445600)** — от [@paji_a](https://x.com/paji_a)

https://github.com/user-attachments/assets/8ecfe4b0-6de7-47f0-9b83-3dc736512e54

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Nano Banana для видео — Тест согласованности](https://x.com/WolfRiccardo/status/2058296266270945483)** — от [@WolfRiccardo](https://x.com/WolfRiccardo)

https://github.com/user-attachments/assets/0cabc195-8a2b-47e6-a649-d95b15003964

</td>
<td width="50%" valign="top">

**[Презентующий изометрический персонаж](https://x.com/kumiko_shiraki/status/2058699566938194382)** — от [@kumiko_shiraki](https://x.com/kumiko_shiraki)

https://github.com/user-attachments/assets/d38627cd-6f23-4ea3-8a95-7cd831229364

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Одно предложение, кинематографический дзен](https://x.com/Dheepanratnam/status/2058372209681342806)** — от [@Dheepanratnam](https://x.com/Dheepanratnam)

https://github.com/user-attachments/assets/d33d9c9d-a68f-4e01-bf1e-c4c8ee60c8ee

</td>
<td width="50%" valign="top">

**[Превращение персонажа — От гламура к повседневности](https://x.com/HBCoop_/status/2058221428780970398)** — от [@HBCoop_](https://x.com/HBCoop_)

https://github.com/user-attachments/assets/239ca343-cb71-4254-8478-d8947d6c33aa

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Waymo в Индии](https://x.com/iHarnoorSingh/status/2058352557819621617)** — от [@iHarnoorSingh](https://x.com/iHarnoorSingh)

https://github.com/user-attachments/assets/7d23ad1f-63bf-4a3c-ab94-09e8f26c570e

</td>
<td width="50%" valign="top">

**[Неотправленное письмо — Короткий фильм](https://x.com/Strength04_X/status/2058367252299452851)** — от [@Strength04_X](https://x.com/Strength04_X)

https://github.com/user-attachments/assets/df8dcb7c-c918-4fc2-b952-0cb2bcdddfee

</td>
</tr>
</table>

<a id="related-repositories"></a>
## 🔗 Связанные репозитории

- [Изучить руководство EvoLink по API видеомоделей](https://github.com/EvoLinkAI/awesome-ai-video-models-api-guide).
- [Использовать репозиторий EvoLink Media MCP](https://github.com/EvoLinkAI/evolink-media-mcp).
- [Изучить Seedance 2.5 на EvoLink](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=related_seedance).

## 🙏 Благодарности

Этот репозиторий был вдохновлён отличными открытыми коллекциями промптов и примерами, которыми делится сообщество.

Спасибо Google DeepMind за публикацию официальных демонстраций и руководств по промптам Gemini Omni, которые сделали эти кейсы возможными.

**Участники сообщества:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711), [@tanabe_fragm](https://x.com/tanabe_fragm), [@venturetwins](https://x.com/venturetwins), [@kumiko_shiraki](https://x.com/kumiko_shiraki), [@Majin_AppSheet](https://x.com/Majin_AppSheet), [@mmmiyama_D](https://x.com/mmmiyama_D), [@VORTEX_Promos](https://x.com/VORTEX_Promos), [@paji_a](https://x.com/paji_a), [@WolfRiccardo](https://x.com/WolfRiccardo), [@Dheepanratnam](https://x.com/Dheepanratnam), [@iHarnoorSingh](https://x.com/iHarnoorSingh), [@Strength04_X](https://x.com/Strength04_X)

*Если что-то нужно исправить, свяжитесь с нами, и мы обновим информацию.*

Если у вас есть интересные кейсы промптов, которыми вы хотите поделиться, свяжитесь с нами и помогите расширить библиотеку промптов Evolink.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&Date)

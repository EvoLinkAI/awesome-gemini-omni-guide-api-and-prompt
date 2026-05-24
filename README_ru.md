<div align="center">
<a href="https://evolink.ai/gemini-omni?utm_source=github&utm_medium=banner&utm_campaign=awesome-gemini-omni"><img src="image/logo.png" alt="awesome-gemini-omni-api-and-prompt logo"></a>
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Try it on Evolink](https://img.shields.io/badge/Try_it_on-Evolink-black)](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
[![Model API](https://img.shields.io/badge/Model-Explore-purple)](https://evolink.ai?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Default_Source-111111)](README.md)
[![🇪🇸 Español](https://img.shields.io/badge/🇪🇸_Español-Ver-ffb703)](README_es.md)
[![🇵🇹 Português](https://img.shields.io/badge/🇵🇹_Português-Ver-2a9d8f)](README_pt.md)
[![🇯🇵 日本語](https://img.shields.io/badge/🇯🇵_日本語-表示-52b788)](README_ja.md)
[![🇰🇷 한국어](https://img.shields.io/badge/🇰🇷_한국어-보기-4ea8de)](README_ko.md)
[![🇩🇪 Deutsch](https://img.shields.io/badge/🇩🇪_Deutsch-Ansehen-f4a261)](README_de.md)
[![🇫🇷 Français](https://img.shields.io/badge/🇫🇷_Français-Voir-e76f51)](README_fr.md)
[![🇹🇷 Türkçe](https://img.shields.io/badge/🇹🇷_Türkçe-Görüntüle-d62828)](README_tr.md)
[![🇹🇼 繁體中文](https://img.shields.io/badge/🇹🇼_繁體中文-查看-8338ec)](README_zh-TW.md)
[![🇨🇳 简体中文](https://img.shields.io/badge/🇨🇳_简体中文-查看-ef476f)](README_zh-CN.md)
[![🇷🇺 Русский](https://img.shields.io/badge/🇷🇺_Русский-Смотреть-577590)](README_ru.md)
</div>
## 🍌 Введение
Добро пожаловать в репозиторий Gemini Omni API и промптов! 🤗
**Мы собираем высококачественные промпты и видеопримеры для Google Gemini Omni, охватывающие широкий спектр творческих задач, включая трансформацию, движение, управление камерой, текстовые последовательности и мультимодальные рабочие процессы.**
Большинство кейсов в этом репозитории отобраны из официальных демонстраций DeepMind, руководств по промптам и экспериментов сообщества.
Попробуйте на Evolink: [Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
Если вам это полезно, поставьте звезду. ⭐
> [!NOTE]
> Этот репозиторий сосредоточен на переиспользуемых паттернах промптов и справочных кейсах для генерации видео Gemini Omni на Evolink.
## 📰 Новости
- **23 мая 2026:** Добавлено 10 кейсов из сообщества на основе популярных твитов
- **22 мая 2026:** Первое обновление репозитория с 25 отобранными промптами Gemini Omni
## 📑 Меню
- [🎯 Ингредиенты промптов](#-ингредиенты-промптов)
- [✂️ Редактирование](#️-редактирование)
  - [🔄 Замена элементов](#-замена-элементов)
  - [🎬 Базовая сцена](#-базовая-сцена)\n  - [📷 Управление камерой](#-управление-камерой)
  - [🎬 Действие и синхронизация](#-действие-и-синхронизация)
- [🎨 Продвинутый мультимодальный режим](#-продвинутый-мультимодальный-режим)
  - [🪞 Художественный стиль](#-художественный-стиль)
  - [✨ Визуальные эффекты](#-визуальные-эффекты)\n  - [🔗 Кросс-модальность](#-кросс-модальность)
  - [📋 Раскадровка](#-раскадровка)
  - [🔤 Рендеринг текста](#-рендеринг-текста)
- [⚖️ Сравнение](#️-сравнение)
- [🧪 Оценка](#-оценка)
- [🙏 Благодарности](#-благодарности)
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
## ✂️ Редактирование
### 🔄 Замена элементов

**Кейс 1: Бабочка в пчелу** `🎬 Video→Video`

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


**Кейс 2: Пчела в светлячков** `🎬 Video→Video`

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

**Кейс 3-5: Серия «Космические корабли и астронавт»** `🎬 Video→Video`

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

**Кейс 3: Корабли в белое оригами**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**Кейс 4: Астронавт в морскую анемону**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**Кейс 5: Малые корабли в скатов**

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

**Кейс 6: Трансформация поезда 1896 (от [@emollick](https://x.com/emollick))** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Промпт:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> Источник: [Original Tweet](https://x.com/emollick/status/2057874739817808223)

---

**Кейс 7: Удаление человека из видео (от [@arrakis_ai](https://x.com/arrakis_ai))** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Промпт:**

```
Remove the person from this video perfectly.
```

> Источник: [Original Tweet](https://x.com/arrakis_ai/status/2057939231755178439)

---

**Кейс 8: Невидимая скрипка** `🎬 Video→Video`

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

### 🎬 Базовая сцена

**Кейс 1: Базовый кадр скрипача** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Промпт:**

```
A video of a violinist playing a song.
```


### 📷 Управление камерой

**Кейс 1: Ракурс через плечо** `🎬 Video→Video`

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


**Кейс 2: Наклон камеры от обуви к среднему плану** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

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

**Кейс 3: Гиперлапс-селфи из путешествия (от [@ZaraIrahh](https://x.com/ZaraIrahh))** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Промпт:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> Источник: [Original Tweet](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**Кейс 4: Дрон-съёмка моды (от [@ariaxawan](https://x.com/ariaxawan))** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Промпт:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> Источник: [Original Tweet](https://x.com/ariaxawan/status/2057794715744084042)

---

**Кейс 5: Вид сверху с вращением на 360° (от [@npaka123](https://x.com/npaka123))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Промпт:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> Источник: [Original Tweet](https://x.com/npaka123/status/2058033145845575735)

### 🎬 Действие и синхронизация


**Кейс 1: Звук игрушечного животного** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Промпт:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**Кейс 2: Синхронизация огней квартир** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Вход:**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

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

**Кейс 3: Цепная реакция с шариком** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Промпт:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**Кейс 4: Огни зданий** `🎬+🎵 Video+Audio→Video`

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

**Кейс 5: Реалистичный боксёрский бой (от [@RuzainaMeer](https://x.com/RuzainaMeer))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Промпт:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> Источник: [Original Tweet](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 Продвинутый мультимодальный режим

### 🪞 Художественный стиль

**Кейс 1-3: Серия «Зеркало»** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**Кейс 1: Зеркало — рябь жидкого металла**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**Кейс 2: Зеркало — линейный рисунок**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**Кейс 3: Зеркало — кукла**

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


**Кейс 4: Анимационная реклама в один кадр (от [@DenneyDara](https://x.com/DenneyDara))** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Промпт:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> Источник: [Original Tweet](https://x.com/DenneyDara/status/2057844409639551380)

---

**Кейс 5: Изоляция линейного рисунка (от [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Промпт:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> Источник: [Original Tweet](https://x.com/alexanderchen/status/2057925025915666673)

---

### ✨ Визуальные эффекты

**Кейс 1: Суперзум через отверстие в руке** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Промпт:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```


**Кейс 2: Эффекты движения скейтборда** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Промпт:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

### 🔗 Кросс-модальность

**Кейс 1: Перенос в новое окружение** `🎬+🖼️ Video+Image→Video`

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


**Кейс 2: Форма птиц со звуком** `🎬+🖼️+🎵 Multi-Modal`

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

**Кейс 3: От слайда к движению (от [@yoshifujidesign](https://x.com/yoshifujidesign))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Промпт:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> Источник: [Original Tweet](https://x.com/yoshifujidesign/status/2058032203175731293)

### 📋 Раскадровка

**Кейс 1: Реклама люксовой косметики (от [@aiwithaly](https://x.com/aiwithaly))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Промпт:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> Источник: [Original Tweet](https://x.com/aiwithaly/status/2057806821138858314)


**Кейс 2: Покажи меня в этой истории** `🖼️ Image→Video`

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

**Кейс 3: Разделённый экран 3x3 (от [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Промпт:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> Источник: [Original Tweet](https://x.com/alexanderchen/status/2057861567396368841)

---

**Кейс 4: Повтор действия с разных ракурсов (от [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Промпт:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> Источник: [Original Tweet](https://x.com/jerrod_lew/status/2057838324140953773)

---

**Кейс 5: Видео с разделённым экраном (от [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Промпт:**

```
Use a reference video and ask the agent for a split screen video.
```

> Источник: [Original Tweet](https://x.com/jerrod_lew/status/2057944349846249975)

---

### 🔤 Рендеринг текста

**Кейс 1: Последовательность предметов по алфавиту** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Промпт:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```


**Кейс 2: Пословная синхронизация текста** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Промпт:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**Кейс 3: Рендеринг текста — новости ИИ (от [@chrisfirst](https://x.com/chrisfirst))** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Промпт:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> Источник: [Original Tweet](https://x.com/chrisfirst/status/2057863432469361098)

---

**Кейс 4: Показ мод шрифтов (от [@HBCoop_](https://x.com/HBCoop_))** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Промпт:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> Источник: [Original Tweet](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ Сравнение

**Кейс 1: Seedance 2.0 vs Gemini Omni Flash (от [@JSFILMZ0412](https://x.com/JSFILMZ0412))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — сравнение переноса стиля, качества движения и цензуры.

> Источник: [Original Tweet](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**Кейс 2: Gemini Omni vs Seedance 2.0 — экшн-сцены (от [@CuriousRefuge](https://x.com/CuriousRefuge))** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Модель видеоредактирования Gemini Omni vs Seedance 2.0 — сравнение масштабных экшн-сцен.

> Источник: [Original Tweet](https://x.com/CuriousRefuge/status/2057929340562907451)

---

## 🧪 Оценка

**Кейс 1: Оценка качества Gemini Omni (от [@kenichiota0711](https://x.com/kenichiota0711))** `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> Источник: [Original Tweet](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 Благодарности

Этот репозиторий был вдохновлён отличными открытыми коллекциями промптов и примерами, которыми делится сообщество.

Спасибо Google DeepMind за публикацию официальных демонстраций и руководств по промптам Gemini Omni, которые сделали эти кейсы возможными.

**Участники сообщества:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*Если что-то нужно исправить, свяжитесь с нами, и мы обновим информацию.*

Если у вас есть интересные кейсы промптов, которыми вы хотите поделиться, свяжитесь с нами и помогите расширить библиотеку промптов Evolink.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

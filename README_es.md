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

## 🍌 Introducción
Bienvenido al repositorio de Gemini Omni API y Prompts! 🤗
**Recopilamos prompts de alta calidad y ejemplos en video para Google Gemini Omni en una amplia variedad de tareas creativas, incluyendo transformación, movimiento, control de cámara, secuencias de texto y flujos de trabajo multi-entrada.**
La mayoría de los casos en este repositorio están seleccionados de demos oficiales de DeepMind, guías de prompts y experimentos de la comunidad.
Pruébalo en Evolink: [Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
Si te resulta útil, considera darle una estrella. ⭐
> [!NOTE]
> Este repositorio se centra en patrones de prompts reutilizables y casos de referencia para la generación de video con Gemini Omni en Evolink.

## 📰 Novedades
- **23 de mayo de 2026:** Se añadieron 10 casos de la comunidad desde tweets destacados
- **22 de mayo de 2026:** Primera actualización del repositorio con 25 prompts seleccionados de Gemini Omni

## 📑 Menú
- [🎯 Ingredientes del Prompt](#-ingredientes-del-prompt)
- [✂️ Edición](#️-edición)
  - [🔄 Reemplazo de Elementos](#-reemplazo-de-elementos)
  - [🎬 Escena Base](#-escena-base)
  - [📷 Dirección de Cámara](#-dirección-de-cámara)
  - [🎬 Acción y Sincronización](#-acción--sincronización)
- [🎨 Multi-Modal Avanzado](#-multi-modal-avanzado)
  - [🪞 Estilo Artístico](#-estilo-artístico)
  - [✨ Efectos Visuales](#-efectos-visuales)
  - [🔗 Cross-Modal](#-cross-modal)
  - [📋 Storyboard](#-storyboard)
  - [🔤 Renderizado de Texto](#-renderizado-de-texto)
- [⚖️ Comparación](#️-comparación)
- [🧪 Evaluación](#-evaluación)
- [🙏 Agradecimientos](#-agradecimientos)

## 🎯 Ingredientes del Prompt
Gemini Omni tiene una fuerte **comprensión del mundo** — se basa en conocimientos del mundo real sobre historia, ciencia y cultura. No necesitas explicar cada detalle en exceso. En su lugar, expresa tu intención creativa en lenguaje natural y deja que el razonamiento de Omni complete el resto.
Al crear un nuevo video desde cero, combina estas dimensiones para controlar el resultado:
| Dimensión | Qué especificar | Ejemplo |
| :--- | :--- | :--- |
| **Encuadre y Movimiento** | Gran angular, plano medio o primer plano. Trayectoria de cámara: deslizamiento suave, movimiento súbito, plano fijo, dolly zoom, etc. | `A close-up tracking shot smoothly pushing in` |
| **Estilo** | Dirección artística visual general | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **Iluminación** | Ambiente de la escena y configuración de luz | `Warm champagne lighting`, `dim overhead gym lights` |
| **Ubicación** | Entorno y fondo | `Small underground gym`, `futuristic neon cityscape` |
| **Acción** | Comportamiento y movimiento del sujeto | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **Edición Iterativa:** Omni soporta edición mediante conversación multi-turno. Preserva lo que funciona y solo modifica lo que pides — no necesitas re-describir toda la escena cada vez. Solo di qué cambiar a continuación.

## ✂️ Edición

### 🔄 Reemplazo de Elementos

**Caso 1: Mariposa a Abeja** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**Prompt:**

```
Change the butterfly to a bee.
```

---

**Caso 2: Abeja a Luciérnagas** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**Prompt:**

```
Change the bee into a small swarm of fireflies.
```

---

**Casos 3-5: Serie de Naves Espaciales y Astronauta** `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**Entrada:**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

**Caso 3: Naves a Origami Blanco**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**Caso 4: Astronauta a Anémona de Mar**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**Caso 5: Naves Pequeñas a Mantarrayas**

</td>
</tr>
</table>

**Prompts:**

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

**Caso 6: Transformación del Tren de 1896 (por [@emollick](https://x.com/emollick))** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Prompt:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> Fuente: [Tweet Original](https://x.com/emollick/status/2057874739817808223)

---

**Caso 7: Eliminar Persona del Video (por [@arrakis_ai](https://x.com/arrakis_ai))** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Prompt:**

```
Remove the person from this video perfectly.
```

> Fuente: [Tweet Original](https://x.com/arrakis_ai/status/2057939231755178439)

---

**Caso 8: Violín Invisible** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**Prompt:**

```
Make the violin invisible
```

### 🎬 Escena Base

**Caso 1: Toma Base del Violinista** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Prompt:**

```
A video of a violinist playing a song.
```

### 📷 Dirección de Cámara

**Caso 1: Ángulo Sobre el Hombro** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle to be over the violinist's shoulder.
```

---

**Caso 2: Inclinación de Cámara de Zapatos a Plano Medio** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**Caso 3: Hyperlapse de Selfie de Viaje (por [@ZaraIrahh](https://x.com/ZaraIrahh))** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Prompt:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> Fuente: [Tweet Original](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**Caso 4: Toma de Dron de Moda (por [@ariaxawan](https://x.com/ariaxawan))** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Prompt:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> Fuente: [Tweet Original](https://x.com/ariaxawan/status/2057794715744084042)

---

**Caso 5: Vista Superior a Rotación 360 (por [@npaka123](https://x.com/npaka123))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Prompt:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> Fuente: [Tweet Original](https://x.com/npaka123/status/2058033145845575735)

### 🎬 Acción y Sincronización

**Caso 1: Sonido de Juguete Animal** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Prompt:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**Caso 2: Sincronización de Luces de Apartamentos** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**Prompt:**

```
The lights of the apartments start turning on in sync with the music.
```

---

**Caso 3: Reacción en Cadena de Canica** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Prompt:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**Caso 4: Luces de Edificios** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**Prompt:**

```
The lights of the buildings start turning on in sync with the music.
```

---

**Caso 5: Pelea de Boxeo Realista (por [@RuzainaMeer](https://x.com/RuzainaMeer))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Prompt:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> Fuente: [Tweet Original](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 Multi-Modal Avanzado

### 🪞 Estilo Artístico

**Casos 1-3: Serie del Espejo** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**Caso 1: Espejo con Ondulación de Metal Líquido**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**Caso 2: Espejo con Arte Lineal**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**Caso 3: Espejo con Marioneta**

</td>
</tr>
</table>

**Prompts:**

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

**Caso 4: Anuncio Animado en Una Toma (por [@DenneyDara](https://x.com/DenneyDara))** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Prompt:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> Fuente: [Tweet Original](https://x.com/DenneyDara/status/2057844409639551380)

---

**Caso 5: Aislamiento de Dibujo Lineal (por [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Prompt:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> Fuente: [Tweet Original](https://x.com/alexanderchen/status/2057925025915666673)

### ✨ Efectos Visuales

**Caso 1: Super Zoom por el Hueco de la Mano** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Prompt:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

**Caso 2: Efectos de Movimiento en Skateboard** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Prompt:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

### 🔗 Cross-Modal

**Caso 1: Transportar a Nuevo Entorno** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**Prompt:**

```
Transport the violinist to the image environment
```

---

**Caso 2: Forma de Pájaros con Audio** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**Video de Entrada:**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**Imagen de Entrada:**

<img src="image/crossmodal-01.webp" width="200">

**Audio de Entrada:**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**Prompt:**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

**Caso 3: De Diapositiva a Movimiento (por [@yoshifujidesign](https://x.com/yoshifujidesign))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Prompt:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> Fuente: [Tweet Original](https://x.com/yoshifujidesign/status/2058032203175731293)

### 📋 Storyboard

**Caso 1: Comercial de Cosmética de Lujo (por [@aiwithaly](https://x.com/aiwithaly))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Prompt:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> Fuente: [Tweet Original](https://x.com/aiwithaly/status/2057806821138858314)

---

**Caso 2: Muéstrame en Esta Historia** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Entrada:**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**Salida:**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**Prompt:**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**Caso 3: Pantalla Dividida 3x3 (por [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Prompt:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> Fuente: [Tweet Original](https://x.com/alexanderchen/status/2057861567396368841)

---

**Caso 4: Repetición de Acción desde Diferentes Ángulos (por [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Prompt:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> Fuente: [Tweet Original](https://x.com/jerrod_lew/status/2057838324140953773)

---

**Caso 5: Video en Pantalla Dividida (por [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Prompt:**

```
Use a reference video and ask the agent for a split screen video.
```

> Fuente: [Tweet Original](https://x.com/jerrod_lew/status/2057944349846249975)

### 🔤 Renderizado de Texto

**Caso 1: Secuencia de Objetos del Alfabeto** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Prompt:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

**Caso 2: Sincronización de Texto Palabra por Palabra** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Prompt:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**Caso 3: Renderizado de Texto Noticias de IA (por [@chrisfirst](https://x.com/chrisfirst))** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Prompt:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> Fuente: [Tweet Original](https://x.com/chrisfirst/status/2057863432469361098)

---

**Caso 4: Desfile de Moda de Fuentes (por [@HBCoop_](https://x.com/HBCoop_))** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Prompt:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> Fuente: [Tweet Original](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ Comparación

**Caso 1: Seedance 2.0 vs Gemini Omni Flash (por [@JSFILMZ0412](https://x.com/JSFILMZ0412))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — comparación de transferencia de estilo, calidad de movimiento y censura.

> Fuente: [Tweet Original](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**Caso 2: Gemini Omni vs Seedance 2.0 Escenas de Acción (por [@CuriousRefuge](https://x.com/CuriousRefuge))** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Modelo de edición de video Gemini Omni vs Seedance 2.0 — comparación de grandes escenas de acción.

> Fuente: [Tweet Original](https://x.com/CuriousRefuge/status/2057929340562907451)

---

## 🧪 Evaluación

**Caso 1: Evaluación de Calidad de Gemini Omni (por [@kenichiota0711](https://x.com/kenichiota0711))** `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> Fuente: [Tweet Original](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 Agradecimientos

Este repositorio fue inspirado por excelentes colecciones abiertas de prompts y ejemplos compartidos por la comunidad.

Gracias a Google DeepMind por publicar demos oficiales de Gemini Omni y guías de prompts que hicieron posibles estos casos de estudio.

**Colaboradores de la Comunidad:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*Si algo necesita ser corregido, por favor contáctanos y lo actualizaremos.*

Si tienes más casos interesantes de prompts para compartir, no dudes en contactarnos y ayudarnos a expandir la biblioteca de prompts de Evolink.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)


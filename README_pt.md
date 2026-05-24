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
## 🍌 Introdução
Bem-vindo ao repositório de API e Prompts do Gemini Omni! 🤗
**Coletamos prompts de alta qualidade e exemplos de vídeo para o Google Gemini Omni em uma ampla variedade de tarefas criativas, incluindo transformação, movimento, controle de câmera, sequências de texto e fluxos de trabalho multi-entrada.**
A maioria dos casos neste repositório são curados a partir de demos oficiais do DeepMind, guias de prompts e experimentos da comunidade.
Experimente no Evolink: [Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
Se você achar útil, considere dar uma estrela. ⭐
> [!NOTE]
> Este repositório foca em padrões de prompts reutilizáveis e casos de referência para geração de vídeo com Gemini Omni no Evolink.
## 📰 Novidades
- **23 de maio de 2026:** Adicionados 10 casos de destaque da comunidade a partir de tweets em alta
- **22 de maio de 2026:** Primeira atualização do repositório com 25 prompts curados do Gemini Omni
## 📑 Menu
- [🎯 Ingredientes do Prompt](#-ingredientes-do-prompt)
- [✂️ Edição](#️-edição)
  - [🔄 Substituição de Elementos](#-substituição-de-elementos)
  - [🎬 Cena Base](#-cena-base)\n  - [📷 Direção de Câmera](#-direção-de-câmera)
  - [🎬 Ação e Sincronização](#-ação--sincronização)
- [🎨 Multi-Modal Avançado](#-multi-modal-avançado)
  - [🪞 Estilo Artístico](#-estilo-artístico)
  - [✨ Efeitos Visuais](#-efeitos-visuais)\n  - [🔗 Cross-Modal](#-cross-modal)
  - [📋 Storyboard](#-storyboard)
  - [🔤 Renderização de Texto](#-renderização-de-texto)
- [⚖️ Comparação](#️-comparação)
- [🧪 Avaliação](#-avaliação)
- [🙏 Agradecimentos](#-agradecimentos)
## 🎯 Ingredientes do Prompt
O Gemini Omni possui forte **compreensão do mundo** — ele se baseia em conhecimento do mundo real sobre história, ciência e cultura. Você não precisa explicar cada detalhe em excesso. Em vez disso, expresse sua intenção criativa em linguagem natural e deixe o raciocínio do Omni preencher o resto.
Ao criar um novo vídeo do zero, combine estas dimensões para controlar o resultado:
| Dimensão | O que especificar | Exemplo |
| :--- | :--- | :--- |
| **Enquadramento e Movimento** | Grande angular, médio ou close-up. Trajetória da câmera: deslize suave, avanço repentino, estático, dolly zoom, etc. | `A close-up tracking shot smoothly pushing in` |
| **Estilo** | Direção de arte visual geral | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **Iluminação** | Clima da cena e configuração de luz | `Warm champagne lighting`, `dim overhead gym lights` |
| **Locação** | Ambiente e cenário | `Small underground gym`, `futuristic neon cityscape` |
| **Ação** | Comportamento e movimento do sujeito | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **Edição Iterativa:** O Omni suporta edição por conversa multi-turno. Ele preserva o que funciona e modifica apenas o que você pede — não é necessário redescrever a cena inteira a cada vez. Apenas diga o que mudar em seguida.
## ✂️ Edição
### 🔄 Substituição de Elementos

**Caso 1: Borboleta para Abelha** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**Prompt:**

```
Change the butterfly to a bee.
```


**Caso 2: Abelha para Vagalumes** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**Prompt:**

```
Change the bee into a small swarm of fireflies.
```

---

**Casos 3-5: Série Naves Espaciais e Astronauta** `🎬 Video→Video`

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

**Caso 3: Naves para Origami Branco**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**Caso 4: Astronauta para Anêmona do Mar**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**Caso 5: Pequenas Naves para Arraias**

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

**Caso 6: Transformação do Trem de 1896 (por [@emollick](https://x.com/emollick))** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Prompt:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> Fonte: [Tweet Original](https://x.com/emollick/status/2057874739817808223)

---

**Caso 7: Remover Pessoa do Vídeo (por [@arrakis_ai](https://x.com/arrakis_ai))** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Prompt:**

```
Remove the person from this video perfectly.
```

> Fonte: [Tweet Original](https://x.com/arrakis_ai/status/2057939231755178439)

---

**Caso 8: Violino Invisível** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**Prompt:**

```
Make the violin invisible
```

### 🎬 Cena Base

**Caso 1: Tomada Base do Violinista** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Prompt:**

```
A video of a violinist playing a song.
```

### 📷 Direção de Câmera

**Caso 1: Ângulo por Cima do Ombro** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle to be over the violinist's shoulder.
```


**Caso 2: Inclinação da Câmera dos Sapatos ao Plano Médio** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**Caso 3: Hyperlapse de Selfie de Viagem (por [@ZaraIrahh](https://x.com/ZaraIrahh))** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Prompt:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> Fonte: [Tweet Original](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**Caso 4: Tomada de Drone de Moda (por [@ariaxawan](https://x.com/ariaxawan))** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Prompt:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> Fonte: [Tweet Original](https://x.com/ariaxawan/status/2057794715744084042)

---

---

**Caso 5: Vista Superior para Rotação 360 (por [@npaka123](https://x.com/npaka123))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Prompt:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> Fonte: [Tweet Original](https://x.com/npaka123/status/2058033145845575735)

### 🎬 Ação e Sincronização


**Caso 1: Som de Brinquedo Animal** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Prompt:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**Caso 2: Sincronização de Luzes dos Apartamentos** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**Prompt:**

```
The lights of the apartments start turning on in sync with the music.
```

---

**Caso 3: Reação em Cadeia com Bolinha de Gude** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Prompt:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**Caso 4: Luzes do Edifício** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**Prompt:**

```
The lights of the buildings start turning on in sync with the music.
```

---

**Caso 5: Luta de Boxe Realista (por [@RuzainaMeer](https://x.com/RuzainaMeer))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Prompt:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> Fonte: [Tweet Original](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 Multi-Modal Avançado

### 🪞 Estilo Artístico

**Casos 1-3: Série do Espelho** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**Caso 1: Espelho com Ondulação de Metal Líquido**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**Caso 2: Espelho com Arte em Linhas**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**Caso 3: Espelho com Fantoche**

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


**Caso 4: Anúncio Animado em Uma Tomada (por [@DenneyDara](https://x.com/DenneyDara))** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Prompt:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> Fonte: [Tweet Original](https://x.com/DenneyDara/status/2057844409639551380)

---

**Caso 5: Isolamento de Desenho em Linhas (por [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Prompt:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> Fonte: [Tweet Original](https://x.com/alexanderchen/status/2057925025915666673)

### ✨ Efeitos Visuais

**Caso 1: Super Zoom pelo Buraco da Mão** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Prompt:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```


**Caso 2: Efeitos de Movimento no Skate** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Prompt:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

### 🔗 Cross-Modal

**Caso 1: Transportar para Novo Ambiente** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**Prompt:**

```
Transport the violinist to the image environment
```


**Caso 2: Forma de Pássaros com Áudio** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**Vídeo de Entrada:**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**Imagem de Entrada:**

<img src="image/crossmodal-01.webp" width="200">

**Áudio de Entrada:**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**Prompt:**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

**Caso 3: Slide para Movimento (por [@yoshifujidesign](https://x.com/yoshifujidesign))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Prompt:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> Fonte: [Tweet Original](https://x.com/yoshifujidesign/status/2058032203175731293)

### 📋 Storyboard

**Caso 1: Comercial de Cosmético de Luxo (por [@aiwithaly](https://x.com/aiwithaly))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Prompt:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> Fonte: [Tweet Original](https://x.com/aiwithaly/status/2057806821138858314)


**Caso 2: Me Mostre Nesta História** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Entrada:**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**Prompt:**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**Caso 3: Tela Dividida 3x3 (por [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Prompt:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> Fonte: [Tweet Original](https://x.com/alexanderchen/status/2057861567396368841)

---

**Caso 4: Replay de Ação de Diferentes Ângulos (por [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Prompt:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> Fonte: [Tweet Original](https://x.com/jerrod_lew/status/2057838324140953773)

---

**Caso 5: Vídeo em Tela Dividida (por [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Prompt:**

```
Use a reference video and ask the agent for a split screen video.
```

> Fonte: [Tweet Original](https://x.com/jerrod_lew/status/2057944349846249975)

### 🔤 Renderização de Texto

**Caso 1: Sequência de Itens do Alfabeto** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Prompt:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```


**Caso 2: Sincronização de Texto Palavra por Palavra** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Prompt:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**Caso 3: Renderização de Texto com Notícias de IA (por [@chrisfirst](https://x.com/chrisfirst))** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Prompt:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> Fonte: [Tweet Original](https://x.com/chrisfirst/status/2057863432469361098)

---

**Caso 4: Desfile de Fontes (por [@HBCoop_](https://x.com/HBCoop_))** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Prompt:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> Fonte: [Tweet Original](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ Comparação

**Caso 1: Seedance 2.0 vs Gemini Omni Flash (por [@JSFILMZ0412](https://x.com/JSFILMZ0412))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — comparação de transferência de estilo, qualidade de movimento e censura.

> Fonte: [Tweet Original](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**Caso 2: Gemini Omni vs Seedance 2.0 Cenas de Ação (por [@CuriousRefuge](https://x.com/CuriousRefuge))** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Modelo de edição de vídeo Gemini Omni vs Seedance 2.0 — comparação de grandes cenas de ação.

> Fonte: [Tweet Original](https://x.com/CuriousRefuge/status/2057929340562907451)

---

## 🧪 Avaliação

**Caso 1: Avaliação de Qualidade do Gemini Omni (por [@kenichiota0711](https://x.com/kenichiota0711))** `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> Fonte: [Tweet Original](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 Agradecimentos

Este repositório foi inspirado por excelentes coleções abertas de prompts e exemplos compartilhados pela comunidade.

Agradecemos ao Google DeepMind por publicar demos oficiais e guias de prompts do Gemini Omni que tornaram estes estudos de caso possíveis.

**Contribuidores da Comunidade:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*Se algo precisar ser corrigido, entre em contato conosco e atualizaremos.*

Se você tem mais casos interessantes de prompts para compartilhar, sinta-se à vontade para entrar em contato e nos ajudar a expandir a biblioteca de prompts do Evolink.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

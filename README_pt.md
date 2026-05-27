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
- **25 de maio de 2026:** Adicionados 16 novos casos da comunidade + nova seção Galeria da Comunidade
- **23 de maio de 2026:** Adicionados 10 casos de destaque da comunidade a partir de tweets em alta
- **22 de maio de 2026:** Primeira atualização do repositório com 25 prompts curados do Gemini Omni

## 📑 Menu
- [🎯 Ingredientes do Prompt](#-ingredientes-do-prompt)
- [✂️ Edição](#️-edição)
  - [🔄 Substituição de Elementos](#-substituição-de-elementos)
    - [Caso 1: Borboleta para Abelha](#caso-1-borboleta-para-abelha)
    - [Caso 2: Abelha para Vagalumes](#caso-2-abelha-para-vagalumes)
    - [Casos 3-5: Série Naves Espaciais e Astronauta](#casos-3-5-série-naves-espaciais-e-astronauta)
    - [Caso 6: Transformação do Trem de 1896 (por @emollick)](#caso-6-transformação-do-trem-de-1896-por-emollick)
    - [Caso 7: Remover Pessoa do Vídeo (por @arrakis_ai)](#caso-7-remover-pessoa-do-vídeo-por-arrakis_ai)
    - [Caso 8: Violino Invisível](#caso-8-violino-invisível)
    - [Caso 9: Mudança de Local com Conhecimento de Mundo (por @venturetwins)](#caso-9-mudança-de-local-com-conhecimento-de-mundo-por-venturetwins)
    - [Caso 10: Animação para Ação Real (por @arrakis_ai)](#caso-10-animação-para-ação-real-por-arrakis_ai)
  - [🎬 Cena Base](#-cena-base)
    - [Caso 1: Tomada Base do Violinista](#caso-1-tomada-base-do-violinista)
  - [📷 Direção de Câmera](#-direção-de-câmera)
    - [Caso 1: Ângulo por Cima do Ombro](#caso-1-ângulo-por-cima-do-ombro)
    - [Caso 2: Inclinação da Câmera dos Sapatos ao Plano Médio](#caso-2-inclinação-da-câmera-dos-sapatos-ao-plano-médio)
    - [Caso 3: Hyperlapse de Selfie de Viagem (por @ZaraIrahh)](#caso-3-hyperlapse-de-selfie-de-viagem-por-zarairahh)
    - [Caso 4: Tomada de Drone de Moda (por @ariaxawan)](#caso-4-tomada-de-drone-de-moda-por-ariaxawan)
    - [Caso 5: Vista Superior para Rotação 360 (por @npaka123)](#caso-5-vista-superior-para-rotação-360-por-npaka123)
    - [Caso 6: Omnizoom — Mergulhando em uma Foto (por @alexanderchen)](#caso-6-omnizoom--mergulhando-em-uma-foto-por-alexanderchen)
  - [🎬 Ação e Sincronização](#-ação-e-sincronização)
    - [Caso 1: Som de Brinquedo Animal](#caso-1-som-de-brinquedo-animal)
    - [Caso 2: Sincronização de Luzes dos Apartamentos](#caso-2-sincronização-de-luzes-dos-apartamentos)
    - [Caso 3: Reação em Cadeia com Bolinha de Gude](#caso-3-reação-em-cadeia-com-bolinha-de-gude)
    - [Caso 4: Luzes do Edifício](#caso-4-luzes-do-edifício)
    - [Caso 5: Luta de Boxe Realista (por @RuzainaMeer)](#caso-5-luta-de-boxe-realista-por-ruzainameer)
- [🎨 Multi-Modal Avançado](#-multi-modal-avançado)
  - [🪞 Estilo Artístico](#-estilo-artístico)
    - [Casos 1-3: Série do Espelho](#casos-1-3-série-do-espelho)
    - [Caso 4: Anúncio Animado em Uma Tomada (por @DenneyDara)](#caso-4-anúncio-animado-em-uma-tomada-por-denneydara)
    - [Caso 5: Isolamento de Desenho em Linhas (por @alexanderchen)](#caso-5-isolamento-de-desenho-em-linhas-por-alexanderchen)
  - [✨ Efeitos Visuais](#-efeitos-visuais)
    - [Caso 1: Super Zoom pelo Buraco da Mão](#caso-1-super-zoom-pelo-buraco-da-mão)
    - [Caso 2: Efeitos de Movimento no Skate](#caso-2-efeitos-de-movimento-no-skate)
    - [Caso 3: Sobreposição HUD AR (por @jerrod_lew)](#caso-3-sobreposição-hud-ar-por-jerrod_lew)
  - [🔗 Cross-Modal](#-cross-modal)
    - [Caso 1: Transportar para Novo Ambiente](#caso-1-transportar-para-novo-ambiente)
    - [Caso 2: Forma de Pássaros com Áudio](#caso-2-forma-de-pássaros-com-áudio)
    - [Caso 3: Slide para Movimento (por @yoshifujidesign)](#caso-3-slide-para-movimento-por-yoshifujidesign)
    - [Caso 4: Personagem Isométrico Cozinhando com Imagem de Referência (por @kumiko_shiraki)](#caso-4-personagem-isométrico-cozinhando-com-imagem-de-referência-por-kumiko_shiraki)
    - [Caso 5: Imagem de Instruções do ChatGPT como Entrada (por @Majin_AppSheet)](#caso-5-imagem-de-instruções-do-chatgpt-como-entrada-por-majin_appsheet)
    - [Caso 6: Ilustração ChatGPT para Animação Omni (por @mmmiyama_D)](#caso-6-ilustração-chatgpt-para-animação-omni-por-mmmiyama_d)
  - [📋 Storyboard](#-storyboard)
    - [Caso 1: Comercial de Cosmético de Luxo (por @aiwithaly)](#caso-1-comercial-de-cosmético-de-luxo-por-aiwithaly)
    - [Caso 2: Me Mostre Nesta História](#caso-2-me-mostre-nesta-história)
    - [Caso 3: Tela Dividida 3x3 (por @alexanderchen)](#caso-3-tela-dividida-3x3-por-alexanderchen)
    - [Caso 4: Replay de Ação de Diferentes Ângulos (por @jerrod_lew)](#caso-4-replay-de-ação-de-diferentes-ângulos-por-jerrod_lew)
    - [Caso 5: Vídeo em Tela Dividida (por @jerrod_lew)](#caso-5-vídeo-em-tela-dividida-por-jerrod_lew)
  - [🔤 Renderização de Texto](#-renderização-de-texto)
    - [Caso 1: Sequência de Itens do Alfabeto](#caso-1-sequência-de-itens-do-alfabeto)
    - [Caso 2: Sincronização de Texto Palavra por Palavra](#caso-2-sincronização-de-texto-palavra-por-palavra)
    - [Caso 3: Renderização de Texto com Notícias de IA (por @chrisfirst)](#caso-3-renderização-de-texto-com-notícias-de-ia-por-chrisfirst)
    - [Caso 4: Desfile de Fontes (por @HBCoop_)](#caso-4-desfile-de-fontes-por-hbcoop_)
- [⚖️ Comparação](#️-comparação)
  - [Caso 1: Seedance 2.0 vs Gemini Omni Flash (por @JSFILMZ0412)](#caso-1-seedance-20-vs-gemini-omni-flash-por-jsfilmz0412)
  - [Caso 2: Gemini Omni vs Seedance 2.0 Cenas de Ação (por @CuriousRefuge)](#caso-2-gemini-omni-vs-seedance-20-cenas-de-ação-por-curiousrefuge)
- [🧪 Avaliação](#-avaliação)
  - [Caso 1: Avaliação de Qualidade do Gemini Omni (por @kenichiota0711)](#caso-1-avaliação-de-qualidade-do-gemini-omni-por-kenichiota0711)
- [🌐 Galeria da Comunidade](#-galeria-da-comunidade)
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

> [!TIP]
> **[Preservar Áreas Inalteradas](https://x.com/tanabe_fragm/status/2058103447006896406) (por [@tanabe_fragm](https://x.com/tanabe_fragm)):** Ao editar vídeo, adicione frases como "Não mude mais nada" ou "Mantenha o resto igual" ao seu prompt. Isso reduz significativamente alterações indesejadas em partes que você não pretendia modificar.
>
> https://github.com/user-attachments/assets/285ee7d8-7dfe-4304-a9a4-648026073b80

## ✂️ Edição

### 🔄 Substituição de Elementos

#### Caso 1: Borboleta para Abelha `🎬 Video→Video`

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

---

#### Caso 2: Abelha para Vagalumes `🎬 Video→Video`

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

#### Casos 3-5: Série Naves Espaciais e Astronauta `🎬 Video→Video`

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

#### Caso 3: Naves para Origami Branco

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

#### Caso 4: Astronauta para Anêmona do Mar

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

#### Caso 5: Pequenas Naves para Arraias

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

#### Caso 6: [Transformação do Trem de 1896](https://x.com/emollick/status/2057874739817808223) (por [@emollick](https://x.com/emollick)) `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Prompt:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

---

#### Caso 7: [Remover Pessoa do Vídeo](https://x.com/arrakis_ai/status/2057939231755178439) (por [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Prompt:**

```
Remove the person from this video perfectly.
```

---

#### Caso 8: Violino Invisível `🎬 Video→Video`

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

---

#### Caso 9: [Mudança de Local com Conhecimento de Mundo](https://x.com/venturetwins/status/2058235415883313361) (por [@venturetwins](https://x.com/venturetwins)) `🎬 Video→Video`

https://github.com/user-attachments/assets/daa90750-fc7b-49ea-b85d-364411159663

**Prompt:**

```
Re-shoot this video in [location] based on the screenshot from Google Maps.
```

> Vídeo de uma corrida Waymo carregado, depois pedido ao Omni para regravar em locais diferentes usando screenshots do Google Maps. O modelo aproveita seu conhecimento de mundo para mudar ambientes de forma fluida.

---

#### Caso 10: [Animação para Ação Real](https://x.com/arrakis_ai/status/2058488373057302797) (por [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/3c6be2a9-3e67-4deb-8ccd-fb493b715f65

**Prompt:**

```
Turn this animation into live action.
```

### 🎬 Cena Base

#### Caso 1: Tomada Base do Violinista `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Prompt:**

```
A video of a violinist playing a song.
```

### 📷 Direção de Câmera

#### Caso 1: Ângulo por Cima do Ombro `🎬 Video→Video`

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

---

#### Caso 2: Inclinação da Câmera dos Sapatos ao Plano Médio `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/19dbc1ae-1e9e-4b7b-9069-e979fffe3651

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

#### Caso 3: [Hyperlapse de Selfie de Viagem](https://x.com/ZaraIrahh/status/2057775215749349520) (por [@ZaraIrahh](https://x.com/ZaraIrahh)) `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Prompt:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

---

#### Caso 4: [Tomada de Drone de Moda](https://x.com/ariaxawan/status/2057794715744084042) (por [@ariaxawan](https://x.com/ariaxawan)) `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Prompt:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

---

#### Caso 5: [Vista Superior para Rotação 360](https://x.com/npaka123/status/2058033145845575735) (por [@npaka123](https://x.com/npaka123)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Prompt:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

---

#### Caso 6: [Omnizoom — Mergulhando em uma Foto](https://x.com/alexanderchen/status/2058330610574221672) (por [@alexanderchen](https://x.com/alexanderchen)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/9fd3ad2a-6e4a-4ac0-ab29-48f1c303b95f

**Prompt:**

```
Omnizoom — diving into a photo.
```

### 🎬 Ação e Sincronização

#### Caso 1: Som de Brinquedo Animal `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Prompt:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

#### Caso 2: Sincronização de Luzes dos Apartamentos `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Entrada:**

https://github.com/user-attachments/assets/6fa879c3-5ee8-4ff1-bbe9-6648d750277d

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

#### Caso 3: Reação em Cadeia com Bolinha de Gude `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Prompt:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

#### Caso 4: Luzes do Edifício `🎬+🎵 Video+Audio→Video`

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

#### Caso 5: [Luta de Boxe Realista](https://x.com/RuzainaMeer/status/2057785474446741728) (por [@RuzainaMeer](https://x.com/RuzainaMeer)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Prompt:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

## 🎨 Multi-Modal Avançado

### 🪞 Estilo Artístico

#### Casos 1-3: Série do Espelho `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

#### Caso 1: Espelho com Ondulação de Metal Líquido

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

#### Caso 2: Espelho com Arte em Linhas

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

#### Caso 3: Espelho com Fantoche

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

#### Caso 4: [Anúncio Animado em Uma Tomada](https://x.com/DenneyDara/status/2057844409639551380) (por [@DenneyDara](https://x.com/DenneyDara)) `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Prompt:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

---

#### Caso 5: [Isolamento de Desenho em Linhas](https://x.com/alexanderchen/status/2057925025915666673) (por [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Prompt:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

### ✨ Efeitos Visuais

#### Caso 1: Super Zoom pelo Buraco da Mão `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Prompt:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

#### Caso 2: Efeitos de Movimento no Skate `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Prompt:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

#### Caso 3: [Sobreposição HUD AR](https://x.com/jerrod_lew/status/2058337271947079977) (por [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/04b11cd7-d345-4172-b6e5-38301e73bb77

**Prompt:**

```
Create a virtual HUD and UI overlay for this recorded phone video, like an AR glasses experience with secondary screens.
```

### 🔗 Cross-Modal

#### Caso 1: Transportar para Novo Ambiente `🎬+🖼️ Video+Image→Video`

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

---

#### Caso 2: Forma de Pássaros com Áudio `🎬+🖼️+🎵 Multi-Modal`

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

#### Caso 3: [Slide para Movimento](https://x.com/yoshifujidesign/status/2058032203175731293) (por [@yoshifujidesign](https://x.com/yoshifujidesign)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Prompt:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

---

#### Caso 4: [Personagem Isométrico Cozinhando com Imagem de Referência](https://x.com/kumiko_shiraki/status/2058337185099546885) (por [@kumiko_shiraki](https://x.com/kumiko_shiraki)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/d5e9b97e-cefa-4cd8-bf70-4e633020f092

**Prompt:**

```
Narrow down reference images and add negative prompts to get closer to your ideal output.
```

> Técnica: Quando o vídeo gerado não corresponde à sua visão, (1) restrinja as imagens de referência, e (2) adicione prompts negativos para suprimir elementos indesejados.

---

#### Caso 5: [Imagem de Instruções do ChatGPT como Entrada](https://x.com/Majin_AppSheet/status/2058191091070058846) (por [@Majin_AppSheet](https://x.com/Majin_AppSheet)) `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Entrada (imagens de instrução do ChatGPT):**

<img src="image/049_majin_appsheet_instruction_image_photo_0.jpg" width="280">

</td>
<td width="300">

**Saída:**

https://github.com/user-attachments/assets/578d6968-c6dd-417a-b6fe-100468851f3d

</td>
</tr>
</table>

> Fluxo de trabalho: Gere imagens de instrução/storyboard no ChatGPT, depois alimente-as diretamente ao Gemini Omni como prompts visuais.

---

#### Caso 6: [Ilustração ChatGPT para Animação Omni](https://x.com/mmmiyama_D/status/2058654389326516656) (por [@mmmiyama_D](https://x.com/mmmiyama_D)) `🖼️ Image→Video`

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

> Fluxo de trabalho: Gere diagramas de ilustração com geração de imagem do ChatGPT → anime-os com Gemini Omni. A renderização de texto pode ser aprimorada adicionando prompts específicos para suprimir corrupção de texto.

### 📋 Storyboard

#### Caso 1: [Comercial de Cosmético de Luxo](https://x.com/aiwithaly/status/2057806821138858314) (por [@aiwithaly](https://x.com/aiwithaly)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Prompt:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

---

#### Caso 2: Me Mostre Nesta História `🖼️ Image→Video`

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

#### Caso 3: [Tela Dividida 3x3](https://x.com/alexanderchen/status/2057861567396368841) (por [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Prompt:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

---

#### Caso 4: [Replay de Ação de Diferentes Ângulos](https://x.com/jerrod_lew/status/2057838324140953773) (por [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Prompt:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

---

#### Caso 5: [Vídeo em Tela Dividida](https://x.com/jerrod_lew/status/2057944349846249975) (por [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Prompt:**

```
Use a reference video and ask the agent for a split screen video.
```

### 🔤 Renderização de Texto

#### Caso 1: Sequência de Itens do Alfabeto `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Prompt:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

#### Caso 2: Sincronização de Texto Palavra por Palavra `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Prompt:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

#### Caso 3: [Renderização de Texto com Notícias de IA](https://x.com/chrisfirst/status/2057863432469361098) (por [@chrisfirst](https://x.com/chrisfirst)) `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Prompt:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

---

#### Caso 4: [Desfile de Fontes](https://x.com/HBCoop_/status/2057856570558452142) (por [@HBCoop_](https://x.com/HBCoop_)) `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Prompt:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

## ⚖️ Comparação

#### Caso 1: [Seedance 2.0 vs Gemini Omni Flash](https://x.com/JSFILMZ0412/status/2057926749598736635) (por [@JSFILMZ0412](https://x.com/JSFILMZ0412)) `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — comparação de transferência de estilo, qualidade de movimento e censura.

---

#### Caso 2: [Gemini Omni vs Seedance 2.0 Cenas de Ação](https://x.com/CuriousRefuge/status/2057929340562907451) (por [@CuriousRefuge](https://x.com/CuriousRefuge)) `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Modelo de edição de vídeo Gemini Omni vs Seedance 2.0 — comparação de grandes cenas de ação.

## 🧪 Avaliação

#### Caso 1: [Avaliação de Qualidade do Gemini Omni](https://x.com/kenichiota0711/status/2057820346850660769) (por [@kenichiota0711](https://x.com/kenichiota0711)) `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

## 🌐 Galeria da Comunidade

Experimentos criativos e showcases da comunidade. Estes casos demonstram a amplitude do que é possível com o Gemini Omni.

<table>
<tr>
<td width="50%" valign="top">

**[Vídeo Educacional Baseado em Conceito](https://x.com/VORTEX_Promos/status/2058083405204459621)** — por [@VORTEX_Promos](https://x.com/VORTEX_Promos)

https://github.com/user-attachments/assets/ca450aec-a6c8-455f-973d-087bfb3da742

</td>
<td width="50%" valign="top">

**[Showcase](https://x.com/paji_a/status/2058070248436445600)** — por [@paji_a](https://x.com/paji_a)

https://github.com/user-attachments/assets/8ecfe4b0-6de7-47f0-9b83-3dc736512e54

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Nano Banana para Vídeo — Teste de Consistência](https://x.com/WolfRiccardo/status/2058296266270945483)** — por [@WolfRiccardo](https://x.com/WolfRiccardo)

https://github.com/user-attachments/assets/0cabc195-8a2b-47e6-a649-d95b15003964

</td>
<td width="50%" valign="top">

**[Personagem Isométrico Apresentando](https://x.com/kumiko_shiraki/status/2058699566938194382)** — por [@kumiko_shiraki](https://x.com/kumiko_shiraki)

https://github.com/user-attachments/assets/d38627cd-6f23-4ea3-8a95-7cd831229364

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Uma Frase, Zen Cinematográfico](https://x.com/Dheepanratnam/status/2058372209681342806)** — por [@Dheepanratnam](https://x.com/Dheepanratnam)

https://github.com/user-attachments/assets/d33d9c9d-a68f-4e01-bf1e-c4c8ee60c8ee

</td>
<td width="50%" valign="top">

**[Transformação de Personagem — Glamoroso a Cotidiano](https://x.com/HBCoop_/status/2058221428780970398)** — por [@HBCoop_](https://x.com/HBCoop_)

https://github.com/user-attachments/assets/239ca343-cb71-4254-8478-d8947d6c33aa

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Waymo para a Índia](https://x.com/iHarnoorSingh/status/2058352557819621617)** — por [@iHarnoorSingh](https://x.com/iHarnoorSingh)

https://github.com/user-attachments/assets/7d23ad1f-63bf-4a3c-ab94-09e8f26c570e

</td>
<td width="50%" valign="top">

**[A Carta Nunca Enviada — Curta-Metragem](https://x.com/Strength04_X/status/2058367252299452851)** — por [@Strength04_X](https://x.com/Strength04_X)

https://github.com/user-attachments/assets/df8dcb7c-c918-4fc2-b952-0cb2bcdddfee

</td>
</tr>
</table>

## 🙏 Agradecimentos

Este repositório foi inspirado por excelentes coleções abertas de prompts e exemplos compartilhados pela comunidade.

Agradecemos ao Google DeepMind por publicar demos oficiais e guias de prompts do Gemini Omni que tornaram estes estudos de caso possíveis.

**Contribuidores da Comunidade:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711), [@tanabe_fragm](https://x.com/tanabe_fragm), [@venturetwins](https://x.com/venturetwins), [@kumiko_shiraki](https://x.com/kumiko_shiraki), [@Majin_AppSheet](https://x.com/Majin_AppSheet), [@mmmiyama_D](https://x.com/mmmiyama_D), [@VORTEX_Promos](https://x.com/VORTEX_Promos), [@paji_a](https://x.com/paji_a), [@WolfRiccardo](https://x.com/WolfRiccardo), [@Dheepanratnam](https://x.com/Dheepanratnam), [@iHarnoorSingh](https://x.com/iHarnoorSingh), [@Strength04_X](https://x.com/Strength04_X)

*Se algo precisar ser corrigido, entre em contato conosco e atualizaremos.*

Se você tem mais casos interessantes de prompts para compartilhar, sinta-se à vontade para entrar em contato e nos ajudar a expandir a biblioteca de prompts do Evolink.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

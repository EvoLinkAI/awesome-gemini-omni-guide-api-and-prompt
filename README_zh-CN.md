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

## 🍌 简介
欢迎来到 Gemini Omni API 与提示词仓库！🤗
**我们收集了高质量的提示词和视频示例，涵盖 Google Gemini Omni 的各种创意任务，包括变换、运动、镜头控制、文字序列和多输入工作流。**
本仓库中的大多数案例精选自 DeepMind 官方演示、提示词指南和社区实验。
在 Evolink 上试用：[Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
如果觉得有用，欢迎给个 Star ⭐
> [!NOTE]
> 本仓库专注于可复用的提示词模式和 Gemini Omni 视频生成在 Evolink 上的参考案例。

## 📰 最新动态
- **2026年5月23日：** 新增 10 个来自热门推文的社区展示案例
- **2026年5月22日：** 首次仓库更新，收录 25 个精选 Gemini Omni 提示词

## 📑 目录
- [🎯 提示词要素](#-提示词要素)
- [✂️ 编辑](#️-编辑)
  - [🔄 元素替换](#-元素替换)
  - [🎬 基础场景](#-基础场景)
  - [📷 镜头调度](#-镜头调度)
  - [🎬 动作与同步](#-动作与同步)
- [🎨 高级多模态](#-高级多模态)
  - [🪞 艺术风格](#-艺术风格)
  - [✨ 视觉特效](#-视觉特效)
  - [🔗 跨模态](#-跨模态)
  - [📋 分镜](#-分镜)
  - [🔤 文字渲染](#-文字渲染)
- [⚖️ 对比](#️-对比)
- [🧪 评估](#-评估)
- [🙏 致谢](#-致谢)

## 🎯 提示词要素
Gemini Omni 具有强大的**世界理解能力**——它能调用历史、科学和文化方面的真实世界知识。你不需要过度解释每个细节，只需用自然语言表达你的创意意图，让 Omni 的推理能力来补充其余部分。
从零开始创建新视频时，可以混合以下维度来控制输出：
| 维度 | 需要指定的内容 | 示例 |
| :--- | :--- | :--- |
| **构图与运动** | 广角、中景或特写。镜头轨迹：缓慢滑动、突然推进、静态锁定、推拉变焦等。 | `A close-up tracking shot smoothly pushing in` |
| **风格** | 整体视觉艺术方向 | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **光线** | 场景氛围和灯光设置 | `Warm champagne lighting`, `dim overhead gym lights` |
| **场景** | 环境和背景 | `Small underground gym`, `futuristic neon cityscape` |
| **动作** | 主体行为和运动 | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **迭代编辑：** Omni 支持多轮对话编辑。它会保留有效的部分，只修改你要求更改的内容——无需每次重新描述整个场景。只需说出下一步要改什么。

## ✂️ 编辑

### 🔄 元素替换

**案例 1：蝴蝶变蜜蜂** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**提示词：**

```
Change the butterfly to a bee.
```

---

**案例 2：蜜蜂变萤火虫** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**提示词：**

```
Change the bee into a small swarm of fireflies.
```

---

**案例 3-5：飞船与宇航员系列** `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**输入：**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

**案例 3：飞船变白色折纸**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**案例 4：宇航员变海葵**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**案例 5：小飞船变魔鬼鱼**

</td>
</tr>
</table>

**提示词：**

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

**案例 6：1896年火车变换（作者 [@emollick](https://x.com/emollick)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**提示词：**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> 来源：[原始推文](https://x.com/emollick/status/2057874739817808223)

---

**案例 7：从视频中移除人物（作者 [@arrakis_ai](https://x.com/arrakis_ai)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**提示词：**

```
Remove the person from this video perfectly.
```

> 来源：[原始推文](https://x.com/arrakis_ai/status/2057939231755178439)

---

**案例 8：隐形小提琴** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**提示词：**

```
Make the violin invisible
```

### 🎬 基础场景

**案例 1：小提琴手基础镜头** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**提示词：**

```
A video of a violinist playing a song.
```

### 📷 镜头调度

**案例 1：过肩角度** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**提示词：**

```
Change the camera angle to be over the violinist's shoulder.
```

---

**案例 2：镜头从鞋子上摇到中景** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**提示词：**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**案例 3：旅行自拍延时摄影（作者 [@ZaraIrahh](https://x.com/ZaraIrahh)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**提示词：**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> 来源：[原始推文](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**案例 4：时尚无人机镜头（作者 [@ariaxawan](https://x.com/ariaxawan)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**提示词：**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> 来源：[原始推文](https://x.com/ariaxawan/status/2057794715744084042)

---

**案例 5：俯视图到360度旋转（作者 [@npaka123](https://x.com/npaka123)）** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**提示词：**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> 来源：[原始推文](https://x.com/npaka123/status/2058033145845575735)

### 🎬 动作与同步

**案例 1：动物玩具声音** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**提示词：**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**案例 2：公寓灯光同步** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**提示词：**

```
The lights of the apartments start turning on in sync with the music.
```

---

**案例 3：弹珠链式反应** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**提示词：**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**案例 4：建筑灯光** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**提示词：**

```
The lights of the buildings start turning on in sync with the music.
```

---

**案例 5：拳击对战写实风格（作者 [@RuzainaMeer](https://x.com/RuzainaMeer)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**提示词：**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> 来源：[原始推文](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 高级多模态

### 🪞 艺术风格

**案例 1-3：镜子系列** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**案例 1：镜面液态金属波纹**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**案例 2：镜面线条画**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**案例 3：镜面布偶**

</td>
</tr>
</table>

**提示词：**

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

**案例 4：动画广告一镜到底（作者 [@DenneyDara](https://x.com/DenneyDara)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**提示词：**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> 来源：[原始推文](https://x.com/DenneyDara/status/2057844409639551380)

---

**案例 5：线条画提取（作者 [@alexanderchen](https://x.com/alexanderchen)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**提示词：**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> 来源：[原始推文](https://x.com/alexanderchen/status/2057925025915666673)

---

### ✨ 视觉特效

**案例 1：手洞超级变焦** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**提示词：**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

**案例 2：滑板运动特效** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**提示词：**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

### 🔗 跨模态

**案例 1：转移到新环境** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**输入：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**提示词：**

```
Transport the violinist to the image environment
```

---

**案例 2：鸟群形状配合音频** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**输入视频：**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**输入图片：**

<img src="image/crossmodal-01.webp" width="200">

**输入音频：**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**提示词：**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

**案例 3：幻灯片转动态（作者 [@yoshifujidesign](https://x.com/yoshifujidesign)）** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**提示词：**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> 来源：[原始推文](https://x.com/yoshifujidesign/status/2058032203175731293)

### 📋 分镜

**案例 1：奢华化妆品广告（作者 [@aiwithaly](https://x.com/aiwithaly)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**提示词：**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> 来源：[原始推文](https://x.com/aiwithaly/status/2057806821138858314)

---

**案例 2：让我出现在这个故事中** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**输入：**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**输出：**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**提示词：**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**案例 3：3x3 分屏（作者 [@alexanderchen](https://x.com/alexanderchen)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**提示词：**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> 来源：[原始推文](https://x.com/alexanderchen/status/2057861567396368841)

---

**案例 4：不同角度的动作回放（作者 [@jerrod_lew](https://x.com/jerrod_lew)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**提示词：**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> 来源：[原始推文](https://x.com/jerrod_lew/status/2057838324140953773)

---

**案例 5：分屏视频（作者 [@jerrod_lew](https://x.com/jerrod_lew)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**提示词：**

```
Use a reference video and ask the agent for a split screen video.
```

> 来源：[原始推文](https://x.com/jerrod_lew/status/2057944349846249975)

---

### 🔤 文字渲染

**案例 1：字母表物品序列** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**提示词：**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

**案例 2：逐字文字同步** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**提示词：**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**案例 3：文字渲染 AI 新闻（作者 [@chrisfirst](https://x.com/chrisfirst)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**提示词：**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> 来源：[原始推文](https://x.com/chrisfirst/status/2057863432469361098)

---

**案例 4：字体时装秀（作者 [@HBCoop_](https://x.com/HBCoop_)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**提示词：**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> 来源：[原始推文](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ 对比

**案例 1：Seedance 2.0 vs Gemini Omni Flash（作者 [@JSFILMZ0412](https://x.com/JSFILMZ0412)）** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast 与 Gemini Omni Flash——风格迁移、运动质量和审查对比。

> 来源：[原始推文](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**案例 2：Gemini Omni vs Seedance 2.0 动作场景（作者 [@CuriousRefuge](https://x.com/CuriousRefuge)）** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni 视频编辑模型 vs Seedance 2.0——大型动作场景对比。

> 来源：[原始推文](https://x.com/CuriousRefuge/status/2057929340562907451)

---

## 🧪 评估

**案例 1：Gemini Omni 质量评估（作者 [@kenichiota0711](https://x.com/kenichiota0711)）** `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> 来源：[原始推文](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 致谢

本仓库的灵感来源于优秀的开放提示词合集和社区分享的示例。

感谢 Google DeepMind 发布的官方 Gemini Omni 演示和提示词指南，使这些案例研究成为可能。

**社区贡献者：**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*如有任何需要更正的内容，请联系我们，我们会及时更新。*

如果你有更多有趣的提示词案例想要分享，欢迎联系我们，帮助我们扩展 Evolink 提示词库。

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

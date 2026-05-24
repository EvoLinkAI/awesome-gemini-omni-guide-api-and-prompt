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
## 🍌 簡介
歡迎來到 Gemini Omni API 與提示詞倉庫！🤗
**我們收集了高品質的提示詞和影片範例，涵蓋 Google Gemini Omni 的各種創意任務，包括轉換、動態、鏡頭控制、文字序列以及多輸入工作流程。**
本倉庫中的大多數案例來自 DeepMind 官方展示、提示詞指南以及社群實驗。
在 Evolink 上試用：[Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)
如果覺得有幫助，歡迎給個星標。⭐
> [!NOTE]
> 本倉庫專注於可重複使用的提示詞模式和 Evolink 上 Gemini Omni 影片生成的參考案例。
## 📰 最新消息
- **2026 年 5 月 23 日：** 新增 10 個來自熱門推文的社群展示案例
- **2026 年 5 月 22 日：** 首次倉庫更新，收錄 25 個精選 Gemini Omni 提示詞
## 📑 目錄
- [🎯 提示詞要素](#-提示詞要素)
- [✂️ 編輯](#️-編輯)
  - [🔄 元素替換](#-元素替換)
  - [🎬 基礎場景](#-基礎場景)\n  - [📷 鏡頭運動](#-鏡頭運動)
  - [🎬 動作與同步](#-動作與同步)
- [🎨 進階多模態](#-進階多模態)
  - [🪞 藝術風格](#-藝術風格)
  - [✨ 視覺特效](#-視覺特效)\n  - [🔗 跨模態](#-跨模態)
  - [📋 分鏡](#-分鏡)
  - [🔤 文字渲染](#-文字渲染)
- [⚖️ 比較](#️-比較)
- [🧪 評估](#-評估)
- [🙏 致謝](#-致謝)
## 🎯 提示詞要素
Gemini Omni 具有強大的**世界理解能力**——它能運用歷史、科學和文化方面的真實世界知識。你不需要過度描述每個細節。只需用自然語言表達你的創意意圖，讓 Omni 的推理能力來補充其餘部分。
從零開始建立新影片時，混合以下維度來控制輸出：
| 維度 | 需要指定的內容 | 範例 |
| :--- | :--- | :--- |
| **構圖與運動** | 廣角、中景或特寫。鏡頭軌跡：緩慢滑動、突然推進、靜止鎖定、推拉變焦等。 | `A close-up tracking shot smoothly pushing in` |
| **風格** | 整體視覺藝術方向 | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **光線** | 場景氛圍和燈光設定 | `Warm champagne lighting`, `dim overhead gym lights` |
| **場景** | 環境和背景 | `Small underground gym`, `futuristic neon cityscape` |
| **動作** | 主體行為和動態 | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **迭代編輯：** Omni 支援多輪對話編輯。它會保留有效的部分，只修改你要求的內容——無需每次重新描述整個場景。只需說明下一步要改什麼。
## ✂️ 編輯
### 🔄 元素替換

**案例 1：蝴蝶變蜜蜂** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**提示詞：**

```
Change the butterfly to a bee.
```


**案例 2：蜜蜂變螢火蟲** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**提示詞：**

```
Change the bee into a small swarm of fireflies.
```

---

**案例 3-5：太空船與太空人系列** `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**輸入：**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

**案例 3：太空船變白色摺紙**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**案例 4：太空人變海葵**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**案例 5：小型飛船變魟魚**

</td>
</tr>
</table>

**提示詞：**

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

**案例 6：1896 年火車變形（by [@emollick](https://x.com/emollick)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**提示詞：**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> 來源：[原始推文](https://x.com/emollick/status/2057874739817808223)

---

**案例 7：從影片中移除人物（by [@arrakis_ai](https://x.com/arrakis_ai)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**提示詞：**

```
Remove the person from this video perfectly.
```

> 來源：[原始推文](https://x.com/arrakis_ai/status/2057939231755178439)

---

**案例 8：隱形小提琴** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**提示詞：**

```
Make the violin invisible
```

### 🎬 基礎場景

**案例 1：小提琴手基礎鏡頭** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**提示詞：**

```
A video of a violinist playing a song.
```


### 📷 鏡頭運動

**案例 1：過肩角度** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**提示詞：**

```
Change the camera angle to be over the violinist's shoulder.
```


**案例 2：鏡頭從鞋子上搖到中景** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**提示詞：**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**案例 3：旅行自拍縮時攝影（by [@ZaraIrahh](https://x.com/ZaraIrahh)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**提示詞：**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> 來源：[原始推文](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**案例 4：時尚無人機鏡頭（by [@ariaxawan](https://x.com/ariaxawan)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**提示詞：**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> 來源：[原始推文](https://x.com/ariaxawan/status/2057794715744084042)

---

**案例 5：俯視到 360 度旋轉（by [@npaka123](https://x.com/npaka123)）** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**提示詞：**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> 來源：[原始推文](https://x.com/npaka123/status/2058033145845575735)

### 🎬 動作與同步


**案例 1：動物玩具音效** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**提示詞：**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**案例 2：公寓燈光同步** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**提示詞：**

```
The lights of the apartments start turning on in sync with the music.
```

---

**案例 3：彈珠連鎖反應** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**提示詞：**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**案例 4：建築燈光** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**提示詞：**

```
The lights of the buildings start turning on in sync with the music.
```

---

**案例 5：拳擊對打寫實風格（by [@RuzainaMeer](https://x.com/RuzainaMeer)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**提示詞：**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> 來源：[原始推文](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 進階多模態

### 🪞 藝術風格

**案例 1-3：鏡子系列** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**案例 1：鏡面液態金屬漣漪**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**案例 2：鏡面線條藝術**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**案例 3：鏡面布偶**

</td>
</tr>
</table>

**提示詞：**

```
Case 1: When the person touches the mirror, make the mirror ripple beautifully like liquid, and the person's arm turns into reflective mirror material
```

```
Case 2: When the person touches the mirror, the person transforms into a detailed monochrome line art drawing
```

```
Case 3: When the person touches the mirror, the person suddenly transforms into a cute felted stuffed puppet version with large googley eyes and glasses
```


**案例 4：動畫廣告一鏡到底（by [@DenneyDara](https://x.com/DenneyDara)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**提示詞：**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> 來源：[原始推文](https://x.com/DenneyDara/status/2057844409639551380)

---

**案例 5：線條畫分離（by [@alexanderchen](https://x.com/alexanderchen)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**提示詞：**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> 來源：[原始推文](https://x.com/alexanderchen/status/2057925025915666673)

---

### ✨ 視覺特效

**案例 1：手洞超級變焦** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**提示詞：**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```


**案例 2：滑板動態效果** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**提示詞：**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

### 🔗 跨模態

**案例 1：轉移到新環境** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**輸入：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**提示詞：**

```
Transport the violinist to the image environment
```


**案例 2：鳥群形狀搭配音訊** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**輸入影片：**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**輸入圖片：**

<img src="image/crossmodal-01.webp" width="200">

**輸入音訊：**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**提示詞：**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

**案例 3：幻燈片轉動態（by [@yoshifujidesign](https://x.com/yoshifujidesign)）** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**提示詞：**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> 來源：[原始推文](https://x.com/yoshifujidesign/status/2058032203175731293)

### 📋 分鏡

**案例 1：奢華化妝品廣告（by [@aiwithaly](https://x.com/aiwithaly)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**提示詞：**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> 來源：[原始推文](https://x.com/aiwithaly/status/2057806821138858314)


**案例 2：讓我出現在這個故事中** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**輸入：**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**輸出：**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**提示詞：**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**案例 3：3x3 分割畫面（by [@alexanderchen](https://x.com/alexanderchen)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**提示詞：**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> 來源：[原始推文](https://x.com/alexanderchen/status/2057861567396368841)

---

**案例 4：不同角度動作回放（by [@jerrod_lew](https://x.com/jerrod_lew)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**提示詞：**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> 來源：[原始推文](https://x.com/jerrod_lew/status/2057838324140953773)

---

**案例 5：分割畫面影片（by [@jerrod_lew](https://x.com/jerrod_lew)）** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**提示詞：**

```
Use a reference video and ask the agent for a split screen video.
```

> 來源：[原始推文](https://x.com/jerrod_lew/status/2057944349846249975)

---

### 🔤 文字渲染

**案例 1：字母物品序列** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**提示詞：**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```


**案例 2：逐字文字同步** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**提示詞：**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**案例 3：文字渲染 AI 新聞（by [@chrisfirst](https://x.com/chrisfirst)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**提示詞：**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> 來源：[原始推文](https://x.com/chrisfirst/status/2057863432469361098)

---

**案例 4：字型時裝秀（by [@HBCoop_](https://x.com/HBCoop_)）** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**提示詞：**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> 來源：[原始推文](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ 比較

**案例 1：Seedance 2.0 vs Gemini Omni Flash（by [@JSFILMZ0412](https://x.com/JSFILMZ0412)）** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash——風格轉換、動態品質與審查機制比較。

> 來源：[原始推文](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**案例 2：Gemini Omni vs Seedance 2.0 動作場景（by [@CuriousRefuge](https://x.com/CuriousRefuge)）** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni 影片編輯模型 vs Seedance 2.0——大型動作場景比較。

> 來源：[原始推文](https://x.com/CuriousRefuge/status/2057929340562907451)

---

## 🧪 評估

**案例 1：Gemini Omni 品質評估（by [@kenichiota0711](https://x.com/kenichiota0711)）** `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> 來源：[原始推文](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 致謝

本倉庫的靈感來自優秀的開放提示詞合集和社群分享的範例。

感謝 Google DeepMind 發布官方 Gemini Omni 展示和提示詞指南，使這些案例研究成為可能。

**社群貢獻者：**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*如有任何需要更正的內容，請聯繫我們，我們會進行更新。*

如果你有更多有趣的提示詞案例想要分享，歡迎聯繫我們，幫助我們擴充 Evolink 提示詞庫。

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

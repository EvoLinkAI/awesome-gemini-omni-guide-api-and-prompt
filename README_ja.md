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

## 🍌 はじめに

Gemini Omni APIとプロンプトリポジトリへようこそ！🤗

**変換、モーション、カメラ制御、テキストシーケンス、マルチ入力ワークフローなど、幅広いクリエイティブタスクに対応したGoogle Gemini Omniの高品質プロンプトと動画サンプルを収集しています。**

本リポジトリのケースの多くは、DeepMind公式デモ、プロンプトガイド、コミュニティの実験から厳選されたものです。

Evolinkで試す: [Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)

お役に立てましたら、ぜひスターをお願いします。⭐

> [!NOTE]
> 本リポジトリは、EvolinkでのGemini Omni動画生成に向けた再利用可能なプロンプトパターンとリファレンスケースに焦点を当てています。

## 📰 ニュース

- **2026年5月23日:** トレンドツイートからコミュニティショーケース10件を追加
- **2026年5月22日:** 厳選されたGemini Omniプロンプト25件で初回リポジトリ更新

## 📑 メニュー

- [🎯 プロンプトの構成要素](#-プロンプトの構成要素)
- [✂️ 編集](#️-編集)
  - [🔄 要素の置き換え](#-要素の置き換え)
  - [📷 カメラ演出](#-カメラ演出)
  - [🎬 アクション＆同期](#-アクション同期)
- [🎨 高度なマルチモーダル](#-高度なマルチモーダル)
  - [🪞 アーティスティックスタイル](#-アーティスティックスタイル)
  - [🔗 クロスモーダル](#-クロスモーダル)
  - [📋 ストーリーボード](#-ストーリーボード)
  - [🔤 テキストレンダリング](#-テキストレンダリング)
- [⚖️ 比較](#️-比較)
- [🙏 謝辞](#-謝辞)

## 🎯 プロンプトの構成要素

Gemini Omniは強力な**世界理解**能力を持っています。歴史、科学、文化に関する現実世界の知識を活用します。すべての詳細を過度に説明する必要はありません。自然言語でクリエイティブな意図を表現すれば、Omniの推論が残りを補完します。

ゼロから新しい動画を作成する際は、以下の要素を組み合わせて出力を制御します：

| 要素 | 指定する内容 | 例 |
| :--- | :--- | :--- |
| **ショットフレーミング＆モーション** | 広角、ミディアム、クローズアップ。カメラの軌道：ゆるやかなグライド、突然のラッシュ、静止ロック、ドリーズームなど。 | `A close-up tracking shot smoothly pushing in` |
| **スタイル** | 全体的なビジュアルアートディレクション | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **ライティング** | シーンのムードと照明設定 | `Warm champagne lighting`, `dim overhead gym lights` |
| **ロケーション** | 環境と背景 | `Small underground gym`, `futuristic neon cityscape` |
| **アクション** | 被写体の動作と動き | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |

> [!TIP]
> **反復編集：** Omniはマルチターン会話編集をサポートしています。うまくいっている部分はそのまま保持し、指示された部分のみを変更します。毎回シーン全体を再記述する必要はありません。次に変更したい内容を伝えるだけです。

## ✂️ 編集

### 🔄 要素の置き換え

**ケース1: 蝶からハチへ** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**プロンプト：**

```
Change the butterfly to a bee.
```

---

**ケース2: ハチからホタルへ** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**プロンプト：**

```
Change the bee into a small swarm of fireflies.
```

---

**ケース3-5: 宇宙船＆宇宙飛行士シリーズ** `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**入力：**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

**ケース3: 宇宙船を白い折り紙に**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**ケース4: 宇宙飛行士をイソギンチャクに**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**ケース5: 小型船をエイに**

</td>
</tr>
</table>

**プロンプト：**

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

**ケース6: 1896年の列車変換 (by [@emollick](https://x.com/emollick))** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**プロンプト：**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> 出典： [元のツイート](https://x.com/emollick/status/2057874739817808223)

---

**ケース7: 動画から人物を削除 (by [@arrakis_ai](https://x.com/arrakis_ai))** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**プロンプト：**

```
Remove the person from this video perfectly.
```

> 出典： [元のツイート](https://x.com/arrakis_ai/status/2057939231755178439)

### 📷 カメラ演出

**ケース1: バイオリニスト ベースショット** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**プロンプト：**

```
A video of a violinist playing a song.
```

---

**ケース2: 新しい環境への移動** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**プロンプト：**

```
Transport the violinist to the image environment
```

---

**ケース3: 透明なバイオリン** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**プロンプト：**

```
Make the violin invisible
```

---

**ケース4: 肩越しアングル** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**プロンプト：**

```
Change the camera angle to be over the violinist's shoulder.
```

---

**ケース5: カメラティルト 靴からミディアムショットへ** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**プロンプト：**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**ケース6: トラベルセルフィー ハイパーラプス (by [@ZaraIrahh](https://x.com/ZaraIrahh))** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**プロンプト：**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> 出典： [元のツイート](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**ケース7: ファッション ドローンショット (by [@ariaxawan](https://x.com/ariaxawan))** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**プロンプト：**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> 出典： [元のツイート](https://x.com/ariaxawan/status/2057794715744084042)

---

**ケース8: 3x3 分割画面 (by [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**プロンプト：**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> 出典： [元のツイート](https://x.com/alexanderchen/status/2057861567396368841)

---

**ケース9: 異なるアングルからのアクションリプレイ (by [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**プロンプト：**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> 出典： [元のツイート](https://x.com/jerrod_lew/status/2057838324140953773)

---

**ケース10: 分割画面動画 (by [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**プロンプト：**

```
Use a reference video and ask the agent for a split screen video.
```

> 出典： [元のツイート](https://x.com/jerrod_lew/status/2057944349846249975)

---

**ケース11: 上面図から360度回転 (by [@npaka123](https://x.com/npaka123))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**プロンプト：**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> 出典： [元のツイート](https://x.com/npaka123/status/2058033145845575735)

### 🎬 アクション＆同期

**ケース1: 手の穴スーパーズーム** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**プロンプト：**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

**ケース2: 動物おもちゃの鳴き声** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**プロンプト：**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**ケース3: アパートの照明同期** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**プロンプト：**

```
The lights of the apartments start turning on in sync with the music.
```

---

**ケース4: ビー玉チェーンリアクション** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**プロンプト：**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**ケース5: ビルの照明** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**プロンプト：**

```
The lights of the buildings start turning on in sync with the music.
```

---

**ケース6: スケートボード モーションエフェクト** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**プロンプト：**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

**ケース7: ボクシング リアルファイト (by [@RuzainaMeer](https://x.com/RuzainaMeer))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**プロンプト：**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> 出典： [元のツイート](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 高度なマルチモーダル

### 🪞 アーティスティックスタイル

**ケース1-3: ミラーシリーズ** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**ケース1: ミラー リキッドメタルリップル**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**ケース2: ミラー ラインアート**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**ケース3: ミラー パペット**

</td>
</tr>
</table>

**プロンプト：**

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

**ケース4: アニメーション広告 ワンショット (by [@DenneyDara](https://x.com/DenneyDara))** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**プロンプト：**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> 出典： [元のツイート](https://x.com/DenneyDara/status/2057844409639551380)

---

**ケース5: 線画アイソレーション (by [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**プロンプト：**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> 出典： [元のツイート](https://x.com/alexanderchen/status/2057925025915666673)

### 🔗 クロスモーダル

**ケース1: 鳥の形とオーディオ** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**入力動画：**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**入力画像：**

<img src="image/crossmodal-01.webp" width="200">

**入力オーディオ：**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**プロンプト：**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

### 📋 ストーリーボード

**ケース1: この物語に登場させて** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**入力：**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**プロンプト：**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**ケース2: 高級コスメCM (by [@aiwithaly](https://x.com/aiwithaly))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**プロンプト：**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> 出典： [元のツイート](https://x.com/aiwithaly/status/2057806821138858314)

---

**ケース3: スライドからモーション (by [@yoshifujidesign](https://x.com/yoshifujidesign))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**プロンプト：**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> 出典： [元のツイート](https://x.com/yoshifujidesign/status/2058032203175731293)

### 🔤 テキストレンダリング

**ケース1: アルファベットアイテムシーケンス** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**プロンプト：**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

**ケース2: 単語ごとのテキスト同期** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**プロンプト：**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**ケース3: テキストレンダリング AIニュース (by [@chrisfirst](https://x.com/chrisfirst))** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**プロンプト：**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> 出典： [元のツイート](https://x.com/chrisfirst/status/2057863432469361098)

---

**ケース4: フォント ファッションショー (by [@HBCoop_](https://x.com/HBCoop_))** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**プロンプト：**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> 出典： [元のツイート](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ 比較

**ケース1: Seedance 2.0 vs Gemini Omni Flash (by [@JSFILMZ0412](https://x.com/JSFILMZ0412))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — スタイル転送、モーション品質、検閲の比較。

> 出典： [元のツイート](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**ケース2: Gemini Omni vs Seedance 2.0 アクションシーン (by [@CuriousRefuge](https://x.com/CuriousRefuge))** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni動画編集モデル vs Seedance 2.0 — 大規模アクションシーンの比較。

> 出典： [元のツイート](https://x.com/CuriousRefuge/status/2057929340562907451)

---

**ケース3: Gemini Omni 品質評価 (by [@kenichiota0711](https://x.com/kenichiota0711))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> 出典： [元のツイート](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 謝辞

本リポジトリは、優れたオープンプロンプトコレクションやコミュニティで共有された事例からインスピレーションを受けています。

これらのケーススタディを可能にした公式Gemini Omniデモとプロンプトガイドを公開してくださったGoogle DeepMindに感謝します。

**コミュニティ貢献者：**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*修正が必要な箇所がございましたら、お問い合わせください。速やかに更新いたします。*

さらに興味深いプロンプトケースをお持ちの方は、ぜひご連絡ください。Evolinkプロンプトライブラリの拡充にご協力いただけると幸いです。

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

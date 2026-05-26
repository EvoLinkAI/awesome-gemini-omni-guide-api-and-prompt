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
- **2026年5月25日：** 新しいコミュニティケース16件追加 + コミュニティギャラリーセクション新設
- **2026年5月23日：** トレンドツイートからコミュニティショーケース10件を追加
- **2026年5月22日：** 厳選されたGemini Omniプロンプト25件で初回リポジトリ更新

## 📑 メニュー
- [🎯 プロンプトの構成要素](#-プロンプトの構成要素)
- [✂️ 編集](#️-編集)
  - [🔄 要素の置き換え](#-要素の置き換え)
    - [ケース1: 蝶からハチへ](#ケース1-蝶からハチへ)
    - [ケース2: ハチからホタルへ](#ケース2-ハチからホタルへ)
    - [ケース3-5: 宇宙船＆宇宙飛行士シリーズ](#ケース3-5-宇宙船宇宙飛行士シリーズ)
    - [ケース6: 1896年の列車変換 (by @emollick)](#ケース6-1896年の列車変換-by-emollick)
    - [ケース7: 動画から人物を削除 (by @arrakis_ai)](#ケース7-動画から人物を削除-by-arrakis_ai)
    - [ケース8: 透明なバイオリン](#ケース8-透明なバイオリン)
    - [ケース9: 世界知識を活用したロケーション変更 (by @venturetwins)](#ケース9-世界知識を活用したロケーション変更-by-venturetwins)
    - [ケース10: アニメを実写化 (by @arrakis_ai)](#ケース10-アニメを実写化-by-arrakis_ai)
  - [🎬 ベースシーン](#-ベースシーン)
    - [ケース1: バイオリニスト ベースショット](#ケース1-バイオリニスト-ベースショット)
  - [📷 カメラ演出](#-カメラ演出)
    - [ケース1: 肩越しアングル](#ケース1-肩越しアングル)
    - [ケース2: カメラティルト 靴からミディアムショットへ](#ケース2-カメラティルト-靴からミディアムショットへ)
    - [ケース3: トラベルセルフィー ハイパーラプス (by @ZaraIrahh)](#ケース3-トラベルセルフィー-ハイパーラプス-by-zarairahh)
    - [ケース4: ファッション ドローンショット (by @ariaxawan)](#ケース4-ファッション-ドローンショット-by-ariaxawan)
    - [ケース5: 上面図から360度回転 (by @npaka123)](#ケース5-上面図から360度回転-by-npaka123)
    - [ケース6: Omnizoom — 写真の中へダイブ (by @alexanderchen)](#ケース6-omnizoom--写真の中へダイブ-by-alexanderchen)
  - [🎬 アクション＆同期](#-アクション同期)
    - [ケース1: 動物おもちゃの鳴き声](#ケース1-動物おもちゃの鳴き声)
    - [ケース2: アパートの照明同期](#ケース2-アパートの照明同期)
    - [ケース3: ビー玉チェーンリアクション](#ケース3-ビー玉チェーンリアクション)
    - [ケース4: ビルの照明](#ケース4-ビルの照明)
    - [ケース5: ボクシング リアルファイト (by @RuzainaMeer)](#ケース5-ボクシング-リアルファイト-by-ruzainameer)
- [🎨 高度なマルチモーダル](#-高度なマルチモーダル)
  - [🪞 アーティスティックスタイル](#-アーティスティックスタイル)
    - [ケース1-3: ミラーシリーズ](#ケース1-3-ミラーシリーズ)
    - [ケース4: アニメーション広告 ワンショット (by @DenneyDara)](#ケース4-アニメーション広告-ワンショット-by-denneydara)
    - [ケース5: 線画アイソレーション (by @alexanderchen)](#ケース5-線画アイソレーション-by-alexanderchen)
  - [✨ ビジュアルエフェクト](#-ビジュアルエフェクト)
    - [ケース1: 手の穴スーパーズーム](#ケース1-手の穴スーパーズーム)
    - [ケース2: スケートボード モーションエフェクト](#ケース2-スケートボード-モーションエフェクト)
    - [ケース3: AR HUD オーバーレイ (by @jerrod_lew)](#ケース3-ar-hud-オーバーレイ-by-jerrod_lew)
  - [🔗 クロスモーダル](#-クロスモーダル)
    - [ケース1: 新しい環境への移動](#ケース1-新しい環境への移動)
    - [ケース2: 鳥の形とオーディオ](#ケース2-鳥の形とオーディオ)
    - [ケース3: スライドからモーション (by @yoshifujidesign)](#ケース3-スライドからモーション-by-yoshifujidesign)
    - [ケース4: 料理上手なアイソメ人 + 参考画像 (by @kumiko_shiraki)](#ケース4-料理上手なアイソメ人--参考画像-by-kumiko_shiraki)
    - [ケース5: ChatGPT 指示書画像を入力に (by @Majin_AppSheet)](#ケース5-chatgpt-指示書画像を入力に-by-majin_appsheet)
    - [ケース6: ChatGPT イラスト → Omni でアニメ化 (by @mmmiyama_D)](#ケース6-chatgpt-イラスト--omni-でアニメ化-by-mmmiyama_d)
  - [📋 ストーリーボード](#-ストーリーボード)
    - [ケース1: 高級コスメCM (by @aiwithaly)](#ケース1-高級コスメcm-by-aiwithaly)
    - [ケース2: この物語に登場させて](#ケース2-この物語に登場させて)
    - [ケース3: 3x3 分割画面 (by @alexanderchen)](#ケース3-3x3-分割画面-by-alexanderchen)
    - [ケース4: 異なるアングルからのアクションリプレイ (by @jerrod_lew)](#ケース4-異なるアングルからのアクションリプレイ-by-jerrod_lew)
    - [ケース5: 分割画面動画 (by @jerrod_lew)](#ケース5-分割画面動画-by-jerrod_lew)
  - [🔤 テキストレンダリング](#-テキストレンダリング)
    - [ケース1: アルファベットアイテムシーケンス](#ケース1-アルファベットアイテムシーケンス)
    - [ケース2: 単語ごとのテキスト同期](#ケース2-単語ごとのテキスト同期)
    - [ケース3: テキストレンダリング AIニュース (by @chrisfirst)](#ケース3-テキストレンダリング-aiニュース-by-chrisfirst)
    - [ケース4: フォント ファッションショー (by @HBCoop_)](#ケース4-フォント-ファッションショー-by-hbcoop_)
- [⚖️ 比較](#️-比較)
  - [ケース1: Seedance 2.0 vs Gemini Omni Flash (by @JSFILMZ0412)](#ケース1-seedance-20-vs-gemini-omni-flash-by-jsfilmz0412)
  - [ケース2: Gemini Omni vs Seedance 2.0 アクションシーン (by @CuriousRefuge)](#ケース2-gemini-omni-vs-seedance-20-アクションシーン-by-curiousrefuge)
- [🧪 評価](#-評価)
  - [ケース1: Gemini Omni 品質評価 (by @kenichiota0711)](#ケース1-gemini-omni-品質評価-by-kenichiota0711)
- [🌐 コミュニティギャラリー](#-コミュニティギャラリー)
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

> [!TIP]
> **[変更しない領域を保持する](https://x.com/tanabe_fragm/status/2058103447006896406)（[@tanabe_fragm](https://x.com/tanabe_fragm) さん）：** 動画を編集する際、プロンプトに「この部分以外は変更しないで」「それ以外は何も変えないで」といった表現を加えることで、意図しない部分への変更を大幅に抑えることができます。
>
> https://github.com/user-attachments/assets/285ee7d8-7dfe-4304-a9a4-648026073b80

## ✂️ 編集

### 🔄 要素の置き換え

#### ケース1: 蝶からハチへ `🎬 Video→Video`

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

#### ケース2: ハチからホタルへ `🎬 Video→Video`

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

#### ケース3-5: 宇宙船＆宇宙飛行士シリーズ `🎬 Video→Video`

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

#### ケース3: 宇宙船を白い折り紙に

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

#### ケース4: 宇宙飛行士をイソギンチャクに

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

#### ケース5: 小型船をエイに

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

#### ケース6: [1896年の列車変換](https://x.com/emollick/status/2057874739817808223) (by [@emollick](https://x.com/emollick)) `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**プロンプト：**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

---

#### ケース7: [動画から人物を削除](https://x.com/arrakis_ai/status/2057939231755178439) (by [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**プロンプト：**

```
Remove the person from this video perfectly.
```

---

#### ケース8: 透明なバイオリン `🎬 Video→Video`

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

#### ケース9: [世界知識を活用したロケーション変更](https://x.com/venturetwins/status/2058235415883313361) (by [@venturetwins](https://x.com/venturetwins)) `🎬 Video→Video`

https://github.com/user-attachments/assets/daa90750-fc7b-49ea-b85d-364411159663

**プロンプト：**

```
Re-shoot this video in [location] based on the screenshot from Google Maps.
```

> Waymoの乗車動画をアップロードし、Google Maps のスクリーンショットを使って異なるロケーションで再撮影するよう Omni に指示。モデルは世界知識を活用して環境をシームレスに切り替えます。

---

#### ケース10: [アニメを実写化](https://x.com/arrakis_ai/status/2058488373057302797) (by [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/3c6be2a9-3e67-4deb-8ccd-fb493b715f65

**プロンプト：**

```
Turn this animation into live action.
```

### 🎬 ベースシーン

#### ケース1: バイオリニスト ベースショット `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**プロンプト：**

```
A video of a violinist playing a song.
```

### 📷 カメラ演出

#### ケース1: 肩越しアングル `🎬 Video→Video`

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

#### ケース2: カメラティルト 靴からミディアムショットへ `🎬 Video→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

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

#### ケース3: [トラベルセルフィー ハイパーラプス](https://x.com/ZaraIrahh/status/2057775215749349520) (by [@ZaraIrahh](https://x.com/ZaraIrahh)) `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**プロンプト：**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

---

#### ケース4: [ファッション ドローンショット](https://x.com/ariaxawan/status/2057794715744084042) (by [@ariaxawan](https://x.com/ariaxawan)) `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**プロンプト：**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

---

#### ケース5: [上面図から360度回転](https://x.com/npaka123/status/2058033145845575735) (by [@npaka123](https://x.com/npaka123)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**プロンプト：**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

---

#### ケース6: [Omnizoom — 写真の中へダイブ](https://x.com/alexanderchen/status/2058330610574221672) (by [@alexanderchen](https://x.com/alexanderchen)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/9fd3ad2a-6e4a-4ac0-ab29-48f1c303b95f

**プロンプト：**

```
Omnizoom — diving into a photo.
```

### 🎬 アクション＆同期

#### ケース1: 動物おもちゃの鳴き声 `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**プロンプト：**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

#### ケース2: アパートの照明同期 `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**入力：**

https://github.com/user-attachments/assets/6fa879c3-5ee8-4ff1-bbe9-6648d750277d

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

#### ケース3: ビー玉チェーンリアクション `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**プロンプト：**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

#### ケース4: ビルの照明 `🎬+🎵 Video+Audio→Video`

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

#### ケース5: [ボクシング リアルファイト](https://x.com/RuzainaMeer/status/2057785474446741728) (by [@RuzainaMeer](https://x.com/RuzainaMeer)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**プロンプト：**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

## 🎨 高度なマルチモーダル

### 🪞 アーティスティックスタイル

#### ケース1-3: ミラーシリーズ `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

#### ケース1: ミラー リキッドメタルリップル

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

#### ケース2: ミラー ラインアート

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

#### ケース3: ミラー パペット

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

#### ケース4: [アニメーション広告 ワンショット](https://x.com/DenneyDara/status/2057844409639551380) (by [@DenneyDara](https://x.com/DenneyDara)) `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**プロンプト：**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

---

#### ケース5: [線画アイソレーション](https://x.com/alexanderchen/status/2057925025915666673) (by [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**プロンプト：**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

### ✨ ビジュアルエフェクト

#### ケース1: 手の穴スーパーズーム `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**プロンプト：**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

#### ケース2: スケートボード モーションエフェクト `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**プロンプト：**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

#### ケース3: [AR HUD オーバーレイ](https://x.com/jerrod_lew/status/2058337271947079977) (by [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/04b11cd7-d345-4172-b6e5-38301e73bb77

**プロンプト：**

```
Create a virtual HUD and UI overlay for this recorded phone video, like an AR glasses experience with secondary screens.
```

### 🔗 クロスモーダル

#### ケース1: 新しい環境への移動 `🎬+🖼️ Video+Image→Video`

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

#### ケース2: 鳥の形とオーディオ `🎬+🖼️+🎵 Multi-Modal`

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

---

#### ケース3: [スライドからモーション](https://x.com/yoshifujidesign/status/2058032203175731293) (by [@yoshifujidesign](https://x.com/yoshifujidesign)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**プロンプト：**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

---

#### ケース4: [料理上手なアイソメ人 + 参考画像](https://x.com/kumiko_shiraki/status/2058337185099546885) (by [@kumiko_shiraki](https://x.com/kumiko_shiraki)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/d5e9b97e-cefa-4cd8-bf70-4e633020f092

**プロンプト：**

```
Narrow down reference images and add negative prompts to get closer to your ideal output.
```

> テクニック：生成された動画がイメージと合わないときは、①参照画像を絞り、②ネガティブプロンプトを入れることで理想の出力に近づきます。

---

#### ケース5: [ChatGPT 指示書画像を入力に](https://x.com/Majin_AppSheet/status/2058191091070058846) (by [@Majin_AppSheet](https://x.com/Majin_AppSheet)) `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**入力（ChatGPT で作成した指示書画像）：**

<img src="image/049_majin_appsheet_instruction_image_photo_0.jpg" width="280">

</td>
<td width="300">

**出力：**

https://github.com/user-attachments/assets/578d6968-c6dd-417a-b6fe-100468851f3d

</td>
</tr>
</table>

> ワークフロー：ChatGPT で指示書／絵コンテ画像を生成し、それをそのまま Gemini Omni にビジュアルプロンプトとして渡します。

---

#### ケース6: [ChatGPT イラスト → Omni でアニメ化](https://x.com/mmmiyama_D/status/2058654389326516656) (by [@mmmiyama_D](https://x.com/mmmiyama_D)) `🖼️ Image→Video`

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

> ワークフロー：ChatGPT の画像生成で図解イラストを作成 → Gemini Omni でアニメーション化。文字化けを抑えるプロンプトを加えることで、テキストレンダリングの精度を高められます。

### 📋 ストーリーボード

#### ケース1: [高級コスメCM](https://x.com/aiwithaly/status/2057806821138858314) (by [@aiwithaly](https://x.com/aiwithaly)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**プロンプト：**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

---

#### ケース2: この物語に登場させて `🖼️ Image→Video`

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

#### ケース3: [3x3 分割画面](https://x.com/alexanderchen/status/2057861567396368841) (by [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**プロンプト：**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

---

#### ケース4: [異なるアングルからのアクションリプレイ](https://x.com/jerrod_lew/status/2057838324140953773) (by [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**プロンプト：**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

---

#### ケース5: [分割画面動画](https://x.com/jerrod_lew/status/2057944349846249975) (by [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**プロンプト：**

```
Use a reference video and ask the agent for a split screen video.
```

### 🔤 テキストレンダリング

#### ケース1: アルファベットアイテムシーケンス `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**プロンプト：**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

#### ケース2: 単語ごとのテキスト同期 `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**プロンプト：**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

#### ケース3: [テキストレンダリング AIニュース](https://x.com/chrisfirst/status/2057863432469361098) (by [@chrisfirst](https://x.com/chrisfirst)) `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**プロンプト：**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

---

#### ケース4: [フォント ファッションショー](https://x.com/HBCoop_/status/2057856570558452142) (by [@HBCoop_](https://x.com/HBCoop_)) `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**プロンプト：**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

## ⚖️ 比較

#### ケース1: [Seedance 2.0 vs Gemini Omni Flash](https://x.com/JSFILMZ0412/status/2057926749598736635) (by [@JSFILMZ0412](https://x.com/JSFILMZ0412)) `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — スタイル転送、モーション品質、検閲の比較。

---

#### ケース2: [Gemini Omni vs Seedance 2.0 アクションシーン](https://x.com/CuriousRefuge/status/2057929340562907451) (by [@CuriousRefuge](https://x.com/CuriousRefuge)) `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni動画編集モデル vs Seedance 2.0 — 大規模アクションシーンの比較。

## 🧪 評価

#### ケース1: [Gemini Omni 品質評価](https://x.com/kenichiota0711/status/2057820346850660769) (by [@kenichiota0711](https://x.com/kenichiota0711)) `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

## 🌐 コミュニティギャラリー

コミュニティから集まったクリエイティブな実験とショーケース。これらのケースは Gemini Omni の可能性の広がりを示しています。

<table>
<tr>
<td width="50%" valign="top">

**[コンセプト主導の教育動画](https://x.com/VORTEX_Promos/status/2058083405204459621)** — by [@VORTEX_Promos](https://x.com/VORTEX_Promos)

https://github.com/user-attachments/assets/ca450aec-a6c8-455f-973d-087bfb3da742

</td>
<td width="50%" valign="top">

**[ショーケース](https://x.com/paji_a/status/2058070248436445600)** — by [@paji_a](https://x.com/paji_a)

https://github.com/user-attachments/assets/8ecfe4b0-6de7-47f0-9b83-3dc736512e54

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[動画版 Nano Banana — 一貫性テスト](https://x.com/WolfRiccardo/status/2058296266270945483)** — by [@WolfRiccardo](https://x.com/WolfRiccardo)

https://github.com/user-attachments/assets/0cabc195-8a2b-47e6-a649-d95b15003964

</td>
<td width="50%" valign="top">

**[プレゼンするアイソメ人](https://x.com/kumiko_shiraki/status/2058699566938194382)** — by [@kumiko_shiraki](https://x.com/kumiko_shiraki)

https://github.com/user-attachments/assets/d38627cd-6f23-4ea3-8a95-7cd831229364

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[一文で生まれるシネマティック禅](https://x.com/Dheepanratnam/status/2058372209681342806)** — by [@Dheepanratnam](https://x.com/Dheepanratnam)

https://github.com/user-attachments/assets/d33d9c9d-a68f-4e01-bf1e-c4c8ee60c8ee

</td>
<td width="50%" valign="top">

**[キャラクター変換 — グラマラスから日常へ](https://x.com/HBCoop_/status/2058221428780970398)** — by [@HBCoop_](https://x.com/HBCoop_)

https://github.com/user-attachments/assets/239ca343-cb71-4254-8478-d8947d6c33aa

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Waymo でインドへ](https://x.com/iHarnoorSingh/status/2058352557819621617)** — by [@iHarnoorSingh](https://x.com/iHarnoorSingh)

https://github.com/user-attachments/assets/7d23ad1f-63bf-4a3c-ab94-09e8f26c570e

</td>
<td width="50%" valign="top">

**[届かなかった手紙 — 短編](https://x.com/Strength04_X/status/2058367252299452851)** — by [@Strength04_X](https://x.com/Strength04_X)

https://github.com/user-attachments/assets/df8dcb7c-c918-4fc2-b952-0cb2bcdddfee

</td>
</tr>
</table>

## 🙏 謝辞

本リポジトリは、優れたオープンプロンプトコレクションやコミュニティで共有された事例からインスピレーションを受けています。

これらのケーススタディを可能にした公式Gemini Omniデモとプロンプトガイドを公開してくださったGoogle DeepMindに感謝します。

**コミュニティ貢献者：**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711), [@tanabe_fragm](https://x.com/tanabe_fragm), [@venturetwins](https://x.com/venturetwins), [@kumiko_shiraki](https://x.com/kumiko_shiraki), [@Majin_AppSheet](https://x.com/Majin_AppSheet), [@mmmiyama_D](https://x.com/mmmiyama_D), [@VORTEX_Promos](https://x.com/VORTEX_Promos), [@paji_a](https://x.com/paji_a), [@WolfRiccardo](https://x.com/WolfRiccardo), [@Dheepanratnam](https://x.com/Dheepanratnam), [@iHarnoorSingh](https://x.com/iHarnoorSingh), [@Strength04_X](https://x.com/Strength04_X)

*修正が必要な箇所がございましたら、お問い合わせください。速やかに更新いたします。*

さらに興味深いプロンプトケースをお持ちの方は、ぜひご連絡ください。Evolinkプロンプトライブラリの拡充にご協力いただけると幸いです。

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

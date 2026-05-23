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

## 🍌 소개

Gemini Omni API 및 프롬프트 저장소에 오신 것을 환영합니다! 🤗

**변환, 모션, 카메라 제어, 텍스트 시퀀스, 멀티 입력 워크플로우 등 다양한 창작 작업을 위한 Google Gemini Omni의 고품질 프롬프트와 비디오 예제를 수집합니다.**

이 저장소의 대부분의 사례는 DeepMind 공식 데모, 프롬프트 가이드 및 커뮤니티 실험에서 선별되었습니다.

Evolink에서 체험하기: [Gemini Omni](https://evolink.ai/gemini-omni?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni)

유용하다고 생각하시면 스타를 눌러주세요. ⭐

> [!NOTE]
> 이 저장소는 Evolink에서의 Gemini Omni 비디오 생성을 위한 재사용 가능한 프롬프트 패턴과 참고 사례에 중점을 둡니다.

## 📰 뉴스

- **2026년 5월 23일:** 트렌딩 트윗에서 커뮤니티 쇼케이스 사례 10개 추가
- **2026년 5월 22일:** 엄선된 Gemini Omni 프롬프트 25개로 첫 저장소 업데이트

## 📑 메뉴

- [🎯 프롬프트 구성 요소](#-프롬프트-구성-요소)
- [✂️ 편집](#️-편집)
  - [🔄 요소 교체](#-요소-교체)
  - [📷 카메라 연출](#-카메라-연출)
  - [🎬 액션 & 싱크](#-액션--싱크)
- [🎨 고급 멀티모달](#-고급-멀티모달)
  - [🪞 아티스틱 스타일](#-아티스틱-스타일)
  - [🔗 크로스모달](#-크로스모달)
  - [📋 스토리보드](#-스토리보드)
  - [🔤 텍스트 렌더링](#-텍스트-렌더링)
- [⚖️ 비교](#️-비교)
- [🙏 감사의 말](#-감사의-말)

## 🎯 프롬프트 구성 요소

Gemini Omni는 강력한 **세계 이해력**을 갖추고 있어 역사, 과학, 문화에 대한 실제 지식을 활용합니다. 모든 세부 사항을 과도하게 설명할 필요가 없습니다. 대신 자연어로 창작 의도를 표현하면 Omni의 추론이 나머지를 채워줍니다.

처음부터 새로운 비디오를 만들 때, 다음 차원들을 조합하여 출력을 제어하세요:

| 차원 | 지정할 내용 | 예시 |
| :--- | :--- | :--- |
| **샷 프레이밍 & 모션** | 와이드 앵글, 미디엄, 또는 클로즈업. 카메라 궤적: 부드러운 글라이드, 갑작스러운 러시, 고정 잠금, 돌리 줌 등. | `A close-up tracking shot smoothly pushing in` |
| **스타일** | 전체적인 비주얼 아트 디렉션 | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **조명** | 장면 분위기와 조명 설정 | `Warm champagne lighting`, `dim overhead gym lights` |
| **장소** | 환경과 배경 | `Small underground gym`, `futuristic neon cityscape` |
| **액션** | 피사체의 행동과 움직임 | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |

> [!TIP]
> **반복 편집:** Omni는 멀티턴 대화 편집을 지원합니다. 잘 된 부분은 유지하고 요청한 부분만 수정합니다 — 매번 전체 장면을 다시 설명할 필요가 없습니다. 다음에 변경할 내용만 말하면 됩니다.

## ✂️ 편집

### 🔄 요소 교체

**사례 1: 나비를 벌로** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**프롬프트:**

```
Change the butterfly to a bee.
```

---

**사례 2: 벌을 반딧불이로** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**프롬프트:**

```
Change the bee into a small swarm of fireflies.
```

---

**사례 3-5: 우주선 & 우주비행사 시리즈** `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**입력:**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

**사례 3: 우주선을 흰색 종이접기로**

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

**사례 4: 우주비행사를 말미잘로**

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

**사례 5: 소형 우주선을 가오리로**

</td>
</tr>
</table>

**프롬프트:**

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

**사례 6: 1896년 기차 변환 (by [@emollick](https://x.com/emollick))** `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**프롬프트:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

> 출처: [원본 트윗](https://x.com/emollick/status/2057874739817808223)

---

**사례 7: 비디오에서 사람 제거 (by [@arrakis_ai](https://x.com/arrakis_ai))** `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**프롬프트:**

```
Remove the person from this video perfectly.
```

> 출처: [원본 트윗](https://x.com/arrakis_ai/status/2057939231755178439)

### 📷 카메라 연출

**사례 1: 바이올리니스트 기본 샷** `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**프롬프트:**

```
A video of a violinist playing a song.
```

---

**사례 2: 새로운 환경으로 이동** `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**프롬프트:**

```
Transport the violinist to the image environment
```

---

**사례 3: 투명 바이올린** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**프롬프트:**

```
Make the violin invisible
```

---

**사례 4: 오버더숄더 앵글** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**프롬프트:**

```
Change the camera angle to be over the violinist's shoulder.
```

---

**사례 5: 카메라 틸트 - 신발에서 미디엄 샷으로** `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**프롬프트:**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

**사례 6: 여행 셀피 하이퍼랩스 (by [@ZaraIrahh](https://x.com/ZaraIrahh))** `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**프롬프트:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

> 출처: [원본 트윗](https://x.com/ZaraIrahh/status/2057775215749349520)

---

**사례 7: 패션 드론 샷 (by [@ariaxawan](https://x.com/ariaxawan))** `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**프롬프트:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

> 출처: [원본 트윗](https://x.com/ariaxawan/status/2057794715744084042)

---

**사례 8: 3x3 분할 화면 (by [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**프롬프트:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

> 출처: [원본 트윗](https://x.com/alexanderchen/status/2057861567396368841)

---

**사례 9: 다른 각도에서의 액션 리플레이 (by [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**프롬프트:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

> 출처: [원본 트윗](https://x.com/jerrod_lew/status/2057838324140953773)

---

**사례 10: 분할 화면 비디오 (by [@jerrod_lew](https://x.com/jerrod_lew))** `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**프롬프트:**

```
Use a reference video and ask the agent for a split screen video.
```

> 출처: [원본 트윗](https://x.com/jerrod_lew/status/2057944349846249975)

---

**사례 11: 탑뷰에서 360도 회전으로 (by [@npaka123](https://x.com/npaka123))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**프롬프트:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

> 출처: [원본 트윗](https://x.com/npaka123/status/2058033145845575735)

### 🎬 액션 & 싱크

**사례 1: 손 구멍 슈퍼 줌** `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**프롬프트:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

**사례 2: 동물 장난감 소리** `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**프롬프트:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

**사례 3: 아파트 조명 싱크** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/0669a7be-bc02-4c96-9a5d-fe2268b66c63

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**프롬프트:**

```
The lights of the apartments start turning on in sync with the music.
```

---

**사례 4: 구슬 연쇄 반응** `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**프롬프트:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

**사례 5: 빌딩 조명** `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**프롬프트:**

```
The lights of the buildings start turning on in sync with the music.
```

---

**사례 6: 스케이트보드 모션 이펙트** `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**프롬프트:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

**사례 7: 복싱 경기 리얼리스틱 (by [@RuzainaMeer](https://x.com/RuzainaMeer))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**프롬프트:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

> 출처: [원본 트윗](https://x.com/RuzainaMeer/status/2057785474446741728)

## 🎨 고급 멀티모달

### 🪞 아티스틱 스타일

**사례 1-3: 거울 시리즈** `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

**사례 1: 거울 액체 금속 파동**

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

**사례 2: 거울 라인 아트**

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

**사례 3: 거울 퍼펫**

</td>
</tr>
</table>

**프롬프트:**

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

**사례 4: 애니메이션 광고 원샷 (by [@DenneyDara](https://x.com/DenneyDara))** `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**프롬프트:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

> 출처: [원본 트윗](https://x.com/DenneyDara/status/2057844409639551380)

---

**사례 5: 라인 드로잉 분리 (by [@alexanderchen](https://x.com/alexanderchen))** `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**프롬프트:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

> 출처: [원본 트윗](https://x.com/alexanderchen/status/2057925025915666673)

### 🔗 크로스모달

**사례 1: 오디오와 함께하는 새 형상** `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**입력 비디오:**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**입력 이미지:**

<img src="image/crossmodal-01.webp" width="200">

**입력 오디오:**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**프롬프트:**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

### 📋 스토리보드

**사례 1: 이 이야기 속에 나를 보여줘** `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**입력:**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**프롬프트:**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

**사례 2: 럭셔리 화장품 광고 (by [@aiwithaly](https://x.com/aiwithaly))** `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**프롬프트:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

> 출처: [원본 트윗](https://x.com/aiwithaly/status/2057806821138858314)

---

**사례 3: 슬라이드를 모션으로 (by [@yoshifujidesign](https://x.com/yoshifujidesign))** `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**프롬프트:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

> 출처: [원본 트윗](https://x.com/yoshifujidesign/status/2058032203175731293)

### 🔤 텍스트 렌더링

**사례 1: 알파벳 아이템 시퀀스** `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**프롬프트:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

**사례 2: 단어별 텍스트 싱크** `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**프롬프트:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

**사례 3: 텍스트 렌더링 AI 뉴스 (by [@chrisfirst](https://x.com/chrisfirst))** `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**프롬프트:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

> 출처: [원본 트윗](https://x.com/chrisfirst/status/2057863432469361098)

---

**사례 4: 폰트 패션쇼 (by [@HBCoop_](https://x.com/HBCoop_))** `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**프롬프트:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

> 출처: [원본 트윗](https://x.com/HBCoop_/status/2057856570558452142)

## ⚖️ 비교

**사례 1: Seedance 2.0 vs Gemini Omni Flash (by [@JSFILMZ0412](https://x.com/JSFILMZ0412))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — 스타일 전환, 모션 품질 및 검열 비교.

> 출처: [원본 트윗](https://x.com/JSFILMZ0412/status/2057926749598736635)

---

**사례 2: Gemini Omni vs Seedance 2.0 액션 장면 (by [@CuriousRefuge](https://x.com/CuriousRefuge))** `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni 비디오 편집 모델 vs Seedance 2.0 — 대형 액션 장면 비교.

> 출처: [원본 트윗](https://x.com/CuriousRefuge/status/2057929340562907451)

---

**사례 3: Gemini Omni 품질 평가 (by [@kenichiota0711](https://x.com/kenichiota0711))** `⚖️ Comparison`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

> 출처: [원본 트윗](https://x.com/kenichiota0711/status/2057820346850660769)

## 🙏 감사의 말

이 저장소는 우수한 오픈 프롬프트 컬렉션과 커뮤니티 공유 예제에서 영감을 받았습니다.

이러한 사례 연구를 가능하게 한 공식 Gemini Omni 데모와 프롬프트 가이드를 공개해 주신 Google DeepMind에 감사드립니다.

**커뮤니티 기여자:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711)

*수정이 필요한 사항이 있으면 연락해 주시면 업데이트하겠습니다.*

더 흥미로운 프롬프트 사례를 공유하고 싶으시다면, 연락해 주셔서 Evolink 프롬프트 라이브러리 확장에 도움을 주세요.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-api-and-prompt&Date)

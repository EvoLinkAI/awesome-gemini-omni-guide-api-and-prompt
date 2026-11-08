<div align="center">

<a href="https://evolink.ai/gemini-omni?utm_source=github&utm_medium=banner&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=readme_banner"><img src="image/guide-banner.png" width="760" alt="Gemini Omni 가이드 및 프롬프트 라이브러리"></a>

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Try Gemini Omni 1.2 Flash](https://img.shields.io/badge/Try_Gemini_Omni_1.2_Flash-EvoLink-black)](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=badge&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=model_try)

[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Default_Source-111111)](README.md) [![🇪🇸 Español](https://img.shields.io/badge/🇪🇸_Español-Ver-ffb703)](README_es.md) [![🇵🇹 Português](https://img.shields.io/badge/🇵🇹_Português-Ver-2a9d8f)](README_pt.md) [![🇯🇵 日本語](https://img.shields.io/badge/🇯🇵_日本語-表示-52b788)](README_ja.md) [![🇰🇷 한국어](https://img.shields.io/badge/🇰🇷_한국어-보기-4ea8de)](README_ko.md) [![🇩🇪 Deutsch](https://img.shields.io/badge/🇩🇪_Deutsch-Ansehen-f4a261)](README_de.md) [![🇫🇷 Français](https://img.shields.io/badge/🇫🇷_Français-Voir-e76f51)](README_fr.md) [![🇹🇷 Türkçe](https://img.shields.io/badge/🇹🇷_Türkçe-Görüntüle-d62828)](README_tr.md) [![🇹🇼 繁體中文](https://img.shields.io/badge/🇹🇼_繁體中文-查看-8338ec)](README_zh-TW.md) [![🇨🇳 简体中文](https://img.shields.io/badge/🇨🇳_简体中文-查看-ef476f)](README_zh-CN.md) [![🇷🇺 Русский](https://img.shields.io/badge/🇷🇺_Русский-Смотреть-577590)](README_ru.md)

</div>

# Gemini Omni 1.2 Flash 가이드 및 프롬프트 라이브러리

## 🍌 소개
**Gemini Omni 1.2 Flash 가이드와 함께, Gemini Omni 제품군의 프롬프트, 편집 데모, 비교, 커뮤니티 영상을 보존한 라이브러리입니다.** 크리에이터와 개발자가 작업을 선택하고 입력 및 출력 제한을 이해할 수 있도록 정리했습니다.

> [!NOTE]
> 기존 프롬프트 사례, 비교, 커뮤니티 갤러리는 과거 Gemini Omni 제품군에 관한 자료입니다. 원본 프롬프트, 출처, 미디어를 그대로 보존하며, 이를 Gemini Omni 1.2 Flash의 생성 결과나 벤치마크로 제시하지 않습니다.

<a id="omni-1-2-guide"></a>
## 🆕 Gemini Omni 1.2 Flash

Google은 Gemini Omni 1.2 Flash를 **2026년 11월 5일** 출시한 GA 모델로 명시합니다. 1.1 대비 주요 변경 사항은 해당 경로에서 최대 **15초**까지 생성할 수 있다는 점과 **독립적인 영상 업스케일**입니다. [Google 모델 사양 읽기](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-1-2-flash), [EvoLink의 11월 5일 발표 읽기](https://evolink.ai/changelog?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=release_source#2026-11-05-gemini-omni-1-2-flash).

- 텍스트, 이미지, 영상을 입력하고, 말소리·음악·효과음이 동기화된 영상을 출력합니다. 오디오 파일 입력과 소리 편집은 지원하지 않습니다.
- 네이티브 출력은 **360p / 720p**입니다. **1080p / 4K는 업스케일 출력**이며 네이티브 4K가 아닙니다. 문서에 명시된 출력은 24 fps이며 화면비는 16:9 또는 9:16입니다.
- EvoLink에서 **15초** 영상을 생성하려면 텍스트로 영상 생성, 첫 프레임 이미지 1장으로 영상 생성, 또는 참조 이미지와 참조 영상 최대 1개를 사용하는 생성을 선택하세요. 첫 프레임과 마지막 프레임을 함께 지정하거나 참조 영상을 2~3개 사용하면 **3~10초**로 설정하세요.
- 영상 연장은 **3~10초**를 덧붙입니다. 이 값은 추가할 길이이며 완성된 영상 전체 길이가 아닙니다.

### EvoLink 작업 선택

각 작업 링크에서 해당 작업의 요청 사양을 확인할 수 있습니다. 경로를 변경하기 전에 [전체 매개변수 개요 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=parameter_overview).

| 작업 | 용도 | 경로별 제한 |
| :--- | :--- | :--- |
| [텍스트 기반 영상 생성 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-text-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_text) | 텍스트 프롬프트로 장면을 생성합니다. | 3~15초. |
| [이미지 기반 영상 생성 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-image-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_image) | 첫 프레임 1장에 움직임을 주거나 첫 프레임과 마지막 프레임을 연결합니다. | 이미지 1장: 3~15초. 이미지 2장: 3~10초. |
| [참조 기반 영상 생성 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-reference-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_reference) | 이미지와 영상 참조 자료를 사용해 새 장면을 생성합니다. | 이미지 최대 10장과 참조 영상 최대 3개. 출력이 10초를 초과하면 참조 영상은 최대 1개. |
| [영상 편집 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-edit?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_edit) | 프롬프트로 기존 클립을 변경합니다. | 최대 15초의 입력 영상 1개. 참조 이미지는 선택 사항. 화질 기본값은 `auto`. |
| [영상 연장 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-extend?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_extend) | 클립 끝부분에서 이어지는 영상을 생성합니다. | 최대 30초의 입력 영상 1개. 3~10초 추가. |
| [영상 업스케일 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-upscale?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_upscale) | 선택한 완성 클립의 해상도를 높입니다. | 지원되는 표준 크기의 입력 영상, 최대 15초. 프롬프트 불필요. 아래의 플랫폼 간 차이를 확인하세요. |

### 플랫폼 및 버전의 차이

- **참조 자료:** [AI Studio 사용 가이드 읽기](https://aistudio.google.com/docs/omni). AI Studio는 이미지를 최대 6장까지 허용하지만 Google Cloud와 EvoLink 문서는 최대 10장으로 명시합니다. 참조 영상의 제한도 출력 길이에 따라 달라지므로 선택한 플랫폼의 사양을 따르세요.
- **업스케일:** Google Cloud는 360p→720p/1080p와 720p→1080p/4K를 명시하며, 1080p→4K는 제외합니다. EvoLink 문서에는 1080p→4K도 기재되어 있습니다. 이 추가 조합은 선택한 플랫폼에서 확인하세요. 모든 플랫폼이 공통으로 보장하는 기능은 아닙니다. [Google 업스케일 제한 읽기](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/video/upscale-videos).
- **대화 상태:** Google의 Interactions API는 대화형 편집을 지원합니다. EvoLink의 비동기 영상 작업은 별도의 요청 사양을 사용하므로 `previous_interaction_id` 등 Google 전용 매개변수를 그대로 전달하지 마세요.
- **마이그레이션:** [Google 모델 페이지 읽기](https://aistudio.google.com/docs/models/gemini-omni-flash). Gemini API의 1.1 stable ID는 2026년 12월 3일부터 1.2로 연결될 예정입니다. 이것이 EvoLink의 1.1 경로도 마이그레이션된다는 뜻은 아닙니다. 기존의 일반 ID를 별칭으로 취급하지 말고 명시적인 1.2 작업을 선택하세요.
- **비용:** EvoLink 모델 페이지는 토큰 기반 요금을 표시합니다. 토큰 단가는 초당 또는 완성 클립 1개당 고정 가격이 아닙니다. 작업 비용을 추산하기 전에 현재 경로, 해상도, 실제 사용량을 확인하세요.

출처 확인일: **2026년 11월 6일**.

<a id="quick-start"></a>
## ⚡ 빠른 시작

[브라우저에서 Gemini Omni 1.2 Flash 체험하기](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=browser_try) 또는 [최신 작업 문서 읽기](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=task_docs).

위 작업 표에서 텍스트 기반 영상 생성, 이미지 기반 영상 생성, 참조 기반 생성, 편집, 연장 또는 업스케일을 선택하세요. 입력, 제한 사항, 결과 처리 흐름은 선택한 작업의 최신 문서를 따르세요.

## 📑 메뉴
- [Gemini Omni 1.2 Flash 가이드](#omni-1-2-guide)
- [빠른 시작](#quick-start)
- [Gemini Omni 1.2 공식 데모](#omni12-demos)
- [Gemini Omni 1.2 커뮤니티 데모 모음](#omni12-community-demos)
- [🎯 프롬프트 구성 요소](#-프롬프트-구성-요소)
- [✂️ 편집](#️-편집)
  - [🔄 요소 교체](#-요소-교체)
    - [사례 1: 나비를 벌로](#사례-1-나비를-벌로)
    - [사례 2: 벌을 반딧불이로](#사례-2-벌을-반딧불이로)
    - [사례 3-5: 우주선 & 우주비행사 시리즈](#사례-3-5-우주선--우주비행사-시리즈)
    - [사례 6: 1896년 기차 변환 (작성자 @emollick)](#사례-6-1896년-기차-변환-작성자-emollick)
    - [사례 7: 비디오에서 사람 제거 (작성자 @arrakis_ai)](#사례-7-비디오에서-사람-제거-작성자-arrakis_ai)
    - [사례 8: 투명 바이올린](#사례-8-투명-바이올린)
    - [사례 9: 세계 지식을 활용한 위치 변경 (작성자 @venturetwins)](#사례-9-세계-지식을-활용한-위치-변경-작성자-venturetwins)
    - [사례 10: 애니메이션을 실사로 (작성자 @arrakis_ai)](#사례-10-애니메이션을-실사로-작성자-arrakis_ai)
  - [🎬 베이스 장면](#-베이스-장면)
    - [사례 1: 바이올리니스트 기본 샷](#사례-1-바이올리니스트-기본-샷)
  - [📷 카메라 연출](#-카메라-연출)
    - [사례 1: 오버더숄더 앵글](#사례-1-오버더숄더-앵글)
    - [사례 2: 카메라 틸트 - 신발에서 미디엄 샷으로](#사례-2-카메라-틸트---신발에서-미디엄-샷으로)
    - [사례 3: 여행 셀피 하이퍼랩스 (작성자 @ZaraIrahh)](#사례-3-여행-셀피-하이퍼랩스-작성자-zarairahh)
    - [사례 4: 패션 드론 샷 (작성자 @ariaxawan)](#사례-4-패션-드론-샷-작성자-ariaxawan)
    - [사례 5: 탑뷰에서 360도 회전으로 (작성자 @npaka123)](#사례-5-탑뷰에서-360도-회전으로-작성자-npaka123)
    - [사례 6: Omnizoom — 사진 속으로 다이브 (작성자 @alexanderchen)](#사례-6-omnizoom--사진-속으로-다이브-작성자-alexanderchen)
  - [🎬 액션 & 싱크](#-액션--싱크)
    - [사례 1: 동물 장난감 소리](#사례-1-동물-장난감-소리)
    - [사례 2: 아파트 조명 싱크](#사례-2-아파트-조명-싱크)
    - [사례 3: 구슬 연쇄 반응](#사례-3-구슬-연쇄-반응)
    - [사례 4: 빌딩 조명](#사례-4-빌딩-조명)
    - [사례 5: 복싱 경기 리얼리스틱 (작성자 @RuzainaMeer)](#사례-5-복싱-경기-리얼리스틱-작성자-ruzainameer)
- [🎨 고급 멀티모달](#-고급-멀티모달)
  - [🪞 아티스틱 스타일](#-아티스틱-스타일)
    - [사례 1-3: 거울 시리즈](#사례-1-3-거울-시리즈)
    - [사례 4: 애니메이션 광고 원샷 (작성자 @DenneyDara)](#사례-4-애니메이션-광고-원샷-작성자-denneydara)
    - [사례 5: 라인 드로잉 분리 (작성자 @alexanderchen)](#사례-5-라인-드로잉-분리-작성자-alexanderchen)
  - [✨ 비주얼 이펙트](#-비주얼-이펙트)
    - [사례 1: 손 구멍 슈퍼 줌](#사례-1-손-구멍-슈퍼-줌)
    - [사례 2: 스케이트보드 모션 이펙트](#사례-2-스케이트보드-모션-이펙트)
    - [사례 3: AR HUD 오버레이 (작성자 @jerrod_lew)](#사례-3-ar-hud-오버레이-작성자-jerrod_lew)
  - [🔗 크로스모달](#-크로스모달)
    - [사례 1: 새로운 환경으로 이동](#사례-1-새로운-환경으로-이동)
    - [사례 2: 오디오와 함께하는 새 형상](#사례-2-오디오와-함께하는-새-형상)
    - [사례 3: 슬라이드를 모션으로 (작성자 @yoshifujidesign)](#사례-3-슬라이드를-모션으로-작성자-yoshifujidesign)
    - [사례 4: 참조 이미지를 활용한 아이소메트릭 요리 캐릭터 (작성자 @kumiko_shiraki)](#사례-4-참조-이미지를-활용한-아이소메트릭-요리-캐릭터-작성자-kumiko_shiraki)
    - [사례 5: ChatGPT 지시서 이미지를 입력으로 (작성자 @Majin_AppSheet)](#사례-5-chatgpt-지시서-이미지를-입력으로-작성자-majin_appsheet)
    - [사례 6: ChatGPT 일러스트를 Omni 애니메이션으로 (작성자 @mmmiyama_D)](#사례-6-chatgpt-일러스트를-omni-애니메이션으로-작성자-mmmiyama_d)
  - [📋 스토리보드](#-스토리보드)
    - [사례 1: 럭셔리 화장품 광고 (작성자 @aiwithaly)](#사례-1-럭셔리-화장품-광고-작성자-aiwithaly)
    - [사례 2: 이 이야기 속에 나를 보여줘](#사례-2-이-이야기-속에-나를-보여줘)
    - [사례 3: 3x3 분할 화면 (작성자 @alexanderchen)](#사례-3-3x3-분할-화면-작성자-alexanderchen)
    - [사례 4: 다른 각도에서의 액션 리플레이 (작성자 @jerrod_lew)](#사례-4-다른-각도에서의-액션-리플레이-작성자-jerrod_lew)
    - [사례 5: 분할 화면 비디오 (작성자 @jerrod_lew)](#사례-5-분할-화면-비디오-작성자-jerrod_lew)
  - [🔤 텍스트 렌더링](#-텍스트-렌더링)
    - [사례 1: 알파벳 아이템 시퀀스](#사례-1-알파벳-아이템-시퀀스)
    - [사례 2: 단어별 텍스트 싱크](#사례-2-단어별-텍스트-싱크)
    - [사례 3: 텍스트 렌더링 AI 뉴스 (작성자 @chrisfirst)](#사례-3-텍스트-렌더링-ai-뉴스-작성자-chrisfirst)
    - [사례 4: 폰트 패션쇼 (작성자 @HBCoop_)](#사례-4-폰트-패션쇼-작성자-hbcoop_)
- [⚖️ 비교](#️-비교)
  - [사례 1: Seedance 2.0 vs Gemini Omni Flash (작성자 @JSFILMZ0412)](#사례-1-seedance-20-vs-gemini-omni-flash-작성자-jsfilmz0412)
  - [사례 2: Gemini Omni vs Seedance 2.0 액션 장면 (작성자 @CuriousRefuge)](#사례-2-gemini-omni-vs-seedance-20-액션-장면-작성자-curiousrefuge)
- [🧪 평가](#-평가)
  - [사례 1: Gemini Omni 품질 평가 (작성자 @kenichiota0711)](#사례-1-gemini-omni-품질-평가-작성자-kenichiota0711)
- [🌐 커뮤니티 갤러리](#-커뮤니티-갤러리)
- [관련 저장소](#related-repositories)
- [🙏 감사의 말](#-감사의-말)

<a id="omni12-demos"></a>
## 🎬 Gemini Omni 1.2 데모

Google이 **2026년 11월 5일** 공개한 공식 데모 8개입니다. [원본 출시 글](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/)을 읽고, 포스터를 선택해 Google의 원본 영상을 시청하세요.

<table>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-1"></a>
**[15초 가상 피팅](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)**

[![15초 가상 피팅](image/omni-1.2/15-second-virtual-try-on.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)

모델 사진 한 장과 의상 세 벌을 바탕으로 15초 가상 피팅 몽타주를 구성합니다.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-2"></a>
**[레이어별 타이포그래피 애니메이션](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)**

[![레이어별 타이포그래피 애니메이션](image/omni-1.2/layered-typography-animation.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)

애니메이션 포스터가 소재와 글자를 조합합니다. Google은 1.1과 1.2의 출력을 함께 보여 줍니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-3"></a>
**[대화형 배경 변경](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)**

[![대화형 배경 변경](image/omni-1.2/conversational-background-changes.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)

대화를 거듭하며 갑옷을 입은 두 인물은 유지한 채 클립의 배경을 바꿉니다.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-4"></a>
**[판테온을 통과하는 연속 비행](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)**

[![판테온을 통과하는 연속 비행](image/omni-1.2/continuous-pantheon-flythrough.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)

건축 사진 두 장을 참조해 판테온의 돔을 통과하는 연속 카메라 비행을 구성합니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-5"></a>
**[15초 벌집 설명 영상](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)**

[![15초 벌집 설명 영상](image/omni-1.2/15-second-beehive-explainer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)

스타일 프레임 한 장이 네 개의 샷으로 구성된 15초짜리 벌집 설명 일러스트 영상이 됩니다.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-6"></a>
**[문어에서 무용수로의 동작 전이](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)**

[![문어에서 무용수로의 동작 전이](image/omni-1.2/octopus-to-dancer-motion-transfer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)

후속 편집으로 문어의 유연한 움직임을 무용수의 드레스에 옮깁니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-7"></a>
**[첫 프레임과 마지막 프레임으로 연결한 라멘 가게](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)**

[![첫 프레임과 마지막 프레임으로 연결한 라멘 가게](image/omni-1.2/first-to-last-frame-ramen-shop.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)

첫 프레임과 마지막 프레임으로 라멘 가게의 외부와 내부를 연결합니다. Google의 비교 영상에는 눈에 띄는 불일치도 포함됩니다.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-8"></a>
**[섬에서 연속 줌아웃](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)**

[![섬에서 연속 줌아웃](image/omni-1.2/continuous-island-zoom-out.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)

10초짜리 한 샷에서 해안의 클로즈업으로부터 섬의 넓은 전경까지 멀어집니다.

</td>
</tr>
</table>

<a id="omni12-community-demos"></a>
## 🎥 Gemini Omni 1.2 커뮤니티 데모 모음

크리에이터와 도구 개발팀이 공개한 Gemini Omni 1.2 Flash 영상 6편을 모았습니다. 미리보기를 선택하면 원본 영상을 재생할 수 있습니다. 제목은 제작자의 게시물이나 글로 연결되며, 공개된 프롬프트는 해당 출처에서 확인할 수 있습니다.

<table>
<tr>
<td width="50%" valign="top">

<a id="omni12-community-1"></a>
**[박자에 맞춰 바뀌는 스트리트웨어](https://x.com/HarshithLucky3/status/2118401265273360530)** · HarshithLucky3

[![박자에 맞춰 바뀌는 스트리트웨어](image/omni-1.2/community/streetwear-beat-cuts.jpg)](https://video-s.twimg.com/amplify_video/2118400792348770305/vid/avc1/640x360/y-KZwoASoz81lFXx.mp4?tag=29)

스트리트 스타일로 걷는 장면에서 손뼉 소리를 신호로 의상이 빠르게 바뀝니다. 제작자가 프롬프트를 공개했습니다.

</td>
<td width="50%" valign="top">

<a id="omni12-community-2"></a>
**[여러 스타일이 어우러진 생일 파티](https://x.com/ash_twtz/status/2118393918794707053)** · ash_twtz

[![여러 스타일이 어우러진 생일 파티](image/omni-1.2/community/mixed-style-party.jpg)](https://video-s.twimg.com/amplify_video/2118393860493905920/vid/avc1/640x360/W2r1uWl7T7aS8Bms.mp4?tag=29)

스톱모션, 3D, 만화, 애니메이션 스타일의 캐릭터가 한 생일 파티 장면에 등장합니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-community-3"></a>
**[타임코드로 구성한 물병 광고](https://weel.co.jp/media/tech/gemini-omni-1-2-flash/)** · WEEL

[![타임코드로 구성한 물병 광고](image/omni-1.2/community/timecoded-bottle-ad.jpg)](https://www.youtube.com/watch?v=u6P7rxZlSQI)

WEEL이 세 구간의 타이밍을 지정한 15초짜리 제품 광고를 실험합니다. 글에 프롬프트가 포함되어 있습니다.

</td>
<td width="50%" valign="top">

<a id="omni12-community-4"></a>
**[첫 프레임과 마지막 프레임으로 연출한 향수 공개](https://blog.segmind.com/gemini-omni-1-2-flash-is-here-generate-and-edit-15-second-videos/)** · Segmind

[![첫 프레임과 마지막 프레임으로 연출한 향수 공개](image/omni-1.2/community/perfume-first-last-frames.jpg)](https://segmind-resources.s3.amazonaws.com/blog/gemini-omni-12-flash/i2v-fl10.mp4)

참조 프레임 두 장으로 어두운 스튜디오에서 햇빛을 받는 꽃으로 이어지는 10초짜리 향수 영상을 연출합니다. 글에 프롬프트가 포함되어 있습니다.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-community-5"></a>
**[도예가와 참조 이미지 속 꽃병](https://blog.segmind.com/gemini-omni-1-2-flash-is-here-generate-and-edit-15-second-videos/)** · Segmind

[![도예가와 참조 이미지 속 꽃병](image/omni-1.2/community/ceramic-artist-vase.jpg)](https://segmind-resources.s3.amazonaws.com/blog/gemini-omni-12-flash/ref10.mp4)

도예가와 꽃병에 각각 다른 참조 자료를 사용해 음성이 들어간 제품 소개 장면을 연출합니다. 글에 프롬프트가 포함되어 있습니다.

</td>
<td width="50%" valign="top">

<a id="omni12-community-6"></a>
**[폴란드 식탁에서 나누는 세 사람의 대화](https://promptif.fr/gemini-omni-1-2-flash-test/)** · Promptif

[![폴란드 식탁에서 나누는 세 사람의 대화](image/omni-1.2/community/polish-dinner-dialogue.webp)](https://promptif.fr/wp-content/uploads/2026/11/omni12-cc251d82201c7f7e2cbd2d57b6e9715b.mp4)

폴란드의 명절 저녁 식사를 배경으로 세 사람이 번갈아 말하는 흐름과 입 모양의 동기화를 시험합니다.

</td>
</tr>
</table>

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

> [!TIP]
> **[변경되지 않을 영역 유지](https://x.com/tanabe_fragm/status/2058103447006896406) (작성자 [@tanabe_fragm](https://x.com/tanabe_fragm)):** 비디오 편집 시 "다른 부분은 바꾸지 마세요" 또는 "나머지는 그대로 유지하세요" 같은 문구를 프롬프트에 추가하세요. 이렇게 하면 의도하지 않은 부분의 변경이 크게 줄어듭니다.
>
> https://github.com/user-attachments/assets/285ee7d8-7dfe-4304-a9a4-648026073b80

## ✂️ 편집

### 🔄 요소 교체

<a id="사례-1-나비를-벌로"></a>
### 사례 1: 나비를 벌로 `🎬 Video→Video`

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

<a id="사례-2-벌을-반딧불이로"></a>
### 사례 2: 벌을 반딧불이로 `🎬 Video→Video`

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

<a id="사례-3-5-우주선--우주비행사-시리즈"></a>
### 사례 3-5: 우주선 & 우주비행사 시리즈 `🎬 Video→Video`

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

### 사례 3: 우주선을 흰색 종이접기로

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

### 사례 4: 우주비행사를 말미잘로

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

### 사례 5: 소형 우주선을 가오리로

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

<a id="사례-6-1896년-기차-변환-작성자-emollick"></a>
### 사례 6: [1896년 기차 변환](https://x.com/emollick/status/2057874739817808223) (작성자 [@emollick](https://x.com/emollick)) `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**프롬프트:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

---

<a id="사례-7-비디오에서-사람-제거-작성자-arrakis_ai"></a>
### 사례 7: [비디오에서 사람 제거](https://x.com/arrakis_ai/status/2057939231755178439) (작성자 [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**프롬프트:**

```
Remove the person from this video perfectly.
```

---

<a id="사례-8-투명-바이올린"></a>
### 사례 8: 투명 바이올린 `🎬 Video→Video`

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

<a id="사례-9-세계-지식을-활용한-위치-변경-작성자-venturetwins"></a>
### 사례 9: [세계 지식을 활용한 위치 변경](https://x.com/venturetwins/status/2058235415883313361) (작성자 [@venturetwins](https://x.com/venturetwins)) `🎬 Video→Video`

https://github.com/user-attachments/assets/daa90750-fc7b-49ea-b85d-364411159663

**프롬프트:**

```
Re-shoot this video in [location] based on the screenshot from Google Maps.
```

> Waymo 차량 탑승 영상을 업로드한 후 Google Maps 스크린샷을 사용하여 다른 위치에서 다시 촬영하도록 Omni에 요청했습니다. 모델은 세계 지식을 활용하여 환경을 매끄럽게 변경합니다.

---

<a id="사례-10-애니메이션을-실사로-작성자-arrakis_ai"></a>
### 사례 10: [애니메이션을 실사로](https://x.com/arrakis_ai/status/2058488373057302797) (작성자 [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/3c6be2a9-3e67-4deb-8ccd-fb493b715f65

**프롬프트:**

```
Turn this animation into live action.
```

### 🎬 베이스 장면

<a id="사례-1-바이올리니스트-기본-샷"></a>
### 사례 1: 바이올리니스트 기본 샷 `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**프롬프트:**

```
A video of a violinist playing a song.
```

### 📷 카메라 연출

<a id="사례-1-오버더숄더-앵글"></a>
### 사례 1: 오버더숄더 앵글 `🎬 Video→Video`

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

<a id="사례-2-카메라-틸트---신발에서-미디엄-샷으로"></a>
### 사례 2: 카메라 틸트 - 신발에서 미디엄 샷으로 `🎬 Video→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/19dbc1ae-1e9e-4b7b-9069-e979fffe3651

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

<a id="사례-3-여행-셀피-하이퍼랩스-작성자-zarairahh"></a>
### 사례 3: [여행 셀피 하이퍼랩스](https://x.com/ZaraIrahh/status/2057775215749349520) (작성자 [@ZaraIrahh](https://x.com/ZaraIrahh)) `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**프롬프트:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

---

<a id="사례-4-패션-드론-샷-작성자-ariaxawan"></a>
### 사례 4: [패션 드론 샷](https://x.com/ariaxawan/status/2057794715744084042) (작성자 [@ariaxawan](https://x.com/ariaxawan)) `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**프롬프트:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

---

<a id="사례-5-탑뷰에서-360도-회전으로-작성자-npaka123"></a>
### 사례 5: [탑뷰에서 360도 회전으로](https://x.com/npaka123/status/2058033145845575735) (작성자 [@npaka123](https://x.com/npaka123)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**프롬프트:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

---

<a id="사례-6-omnizoom--사진-속으로-다이브-작성자-alexanderchen"></a>
### 사례 6: [Omnizoom — 사진 속으로 다이브](https://x.com/alexanderchen/status/2058330610574221672) (작성자 [@alexanderchen](https://x.com/alexanderchen)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/9fd3ad2a-6e4a-4ac0-ab29-48f1c303b95f

**프롬프트:**

```
Omnizoom — diving into a photo.
```

### 🎬 액션 & 싱크

<a id="사례-1-동물-장난감-소리"></a>
### 사례 1: 동물 장난감 소리 `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**프롬프트:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

<a id="사례-2-아파트-조명-싱크"></a>
### 사례 2: 아파트 조명 싱크 `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**입력:**

https://github.com/user-attachments/assets/6fa879c3-5ee8-4ff1-bbe9-6648d750277d

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

<a id="사례-3-구슬-연쇄-반응"></a>
### 사례 3: 구슬 연쇄 반응 `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**프롬프트:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

<a id="사례-4-빌딩-조명"></a>
### 사례 4: 빌딩 조명 `🎬+🎵 Video+Audio→Video`

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

<a id="사례-5-복싱-경기-리얼리스틱-작성자-ruzainameer"></a>
### 사례 5: [복싱 경기 리얼리스틱](https://x.com/RuzainaMeer/status/2057785474446741728) (작성자 [@RuzainaMeer](https://x.com/RuzainaMeer)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**프롬프트:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

## 🎨 고급 멀티모달

### 🪞 아티스틱 스타일

<a id="사례-1-3-거울-시리즈"></a>
### 사례 1-3: 거울 시리즈 `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

### 사례 1: 거울 액체 금속 파동

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

### 사례 2: 거울 라인 아트

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

### 사례 3: 거울 퍼펫

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

<a id="사례-4-애니메이션-광고-원샷-작성자-denneydara"></a>
### 사례 4: [애니메이션 광고 원샷](https://x.com/DenneyDara/status/2057844409639551380) (작성자 [@DenneyDara](https://x.com/DenneyDara)) `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**프롬프트:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

---

<a id="사례-5-라인-드로잉-분리-작성자-alexanderchen"></a>
### 사례 5: [라인 드로잉 분리](https://x.com/alexanderchen/status/2057925025915666673) (작성자 [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**프롬프트:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

### ✨ 비주얼 이펙트

<a id="사례-1-손-구멍-슈퍼-줌"></a>
### 사례 1: 손 구멍 슈퍼 줌 `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**프롬프트:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

<a id="사례-2-스케이트보드-모션-이펙트"></a>
### 사례 2: 스케이트보드 모션 이펙트 `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**프롬프트:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

<a id="사례-3-ar-hud-오버레이-작성자-jerrod_lew"></a>
### 사례 3: [AR HUD 오버레이](https://x.com/jerrod_lew/status/2058337271947079977) (작성자 [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/04b11cd7-d345-4172-b6e5-38301e73bb77

**프롬프트:**

```
Create a virtual HUD and UI overlay for this recorded phone video, like an AR glasses experience with secondary screens.
```

### 🔗 크로스모달

<a id="사례-1-새로운-환경으로-이동"></a>
### 사례 1: 새로운 환경으로 이동 `🎬+🖼️ Video+Image→Video`

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

<a id="사례-2-오디오와-함께하는-새-형상"></a>
### 사례 2: 오디오와 함께하는 새 형상 `🎬+🖼️+🎵 Multi-Modal`

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

---

<a id="사례-3-슬라이드를-모션으로-작성자-yoshifujidesign"></a>
### 사례 3: [슬라이드를 모션으로](https://x.com/yoshifujidesign/status/2058032203175731293) (작성자 [@yoshifujidesign](https://x.com/yoshifujidesign)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**프롬프트:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

---

<a id="사례-4-참조-이미지를-활용한-아이소메트릭-요리-캐릭터-작성자-kumiko_shiraki"></a>
### 사례 4: [참조 이미지를 활용한 아이소메트릭 요리 캐릭터](https://x.com/kumiko_shiraki/status/2058337185099546885) (작성자 [@kumiko_shiraki](https://x.com/kumiko_shiraki)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/d5e9b97e-cefa-4cd8-bf70-4e633020f092

**프롬프트:**

```
Narrow down reference images and add negative prompts to get closer to your ideal output.
```

> 기법: 생성된 비디오가 의도와 일치하지 않을 때, (1) 참조 이미지를 좁히고, (2) 원하지 않는 요소를 억제하기 위해 네거티브 프롬프트를 추가합니다.

---

<a id="사례-5-chatgpt-지시서-이미지를-입력으로-작성자-majin_appsheet"></a>
### 사례 5: [ChatGPT 지시서 이미지를 입력으로](https://x.com/Majin_AppSheet/status/2058191091070058846) (작성자 [@Majin_AppSheet](https://x.com/Majin_AppSheet)) `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**입력 (ChatGPT의 지시 이미지):**

<img src="image/049_majin_appsheet_instruction_image_photo_0.jpg" width="280">

</td>
<td width="300">

**출력:**

https://github.com/user-attachments/assets/578d6968-c6dd-417a-b6fe-100468851f3d

</td>
</tr>
</table>

> 워크플로우: ChatGPT에서 지시/스토리보드 이미지를 생성한 후, 비주얼 프롬프트로서 Gemini Omni에 직접 입력합니다.

---

<a id="사례-6-chatgpt-일러스트를-omni-애니메이션으로-작성자-mmmiyama_d"></a>
### 사례 6: [ChatGPT 일러스트를 Omni 애니메이션으로](https://x.com/mmmiyama_D/status/2058654389326516656) (작성자 [@mmmiyama_D](https://x.com/mmmiyama_D)) `🖼️ Image→Video`

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

> 워크플로우: ChatGPT 이미지 생성으로 일러스트 다이어그램을 생성 → Gemini Omni로 애니메이션화합니다. 텍스트 깨짐을 억제하기 위한 특정 프롬프트를 추가하여 텍스트 렌더링을 개선할 수 있습니다.

### 📋 스토리보드

<a id="사례-1-럭셔리-화장품-광고-작성자-aiwithaly"></a>
### 사례 1: [럭셔리 화장품 광고](https://x.com/aiwithaly/status/2057806821138858314) (작성자 [@aiwithaly](https://x.com/aiwithaly)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**프롬프트:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

---

<a id="사례-2-이-이야기-속에-나를-보여줘"></a>
### 사례 2: 이 이야기 속에 나를 보여줘 `🖼️ Image→Video`

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

<a id="사례-3-3x3-분할-화면-작성자-alexanderchen"></a>
### 사례 3: [3x3 분할 화면](https://x.com/alexanderchen/status/2057861567396368841) (작성자 [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**프롬프트:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

---

<a id="사례-4-다른-각도에서의-액션-리플레이-작성자-jerrod_lew"></a>
### 사례 4: [다른 각도에서의 액션 리플레이](https://x.com/jerrod_lew/status/2057838324140953773) (작성자 [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**프롬프트:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

---

<a id="사례-5-분할-화면-비디오-작성자-jerrod_lew"></a>
### 사례 5: [분할 화면 비디오](https://x.com/jerrod_lew/status/2057944349846249975) (작성자 [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**프롬프트:**

```
Use a reference video and ask the agent for a split screen video.
```

### 🔤 텍스트 렌더링

<a id="사례-1-알파벳-아이템-시퀀스"></a>
### 사례 1: 알파벳 아이템 시퀀스 `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**프롬프트:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

<a id="사례-2-단어별-텍스트-싱크"></a>
### 사례 2: 단어별 텍스트 싱크 `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**프롬프트:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

<a id="사례-3-텍스트-렌더링-ai-뉴스-작성자-chrisfirst"></a>
### 사례 3: [텍스트 렌더링 AI 뉴스](https://x.com/chrisfirst/status/2057863432469361098) (작성자 [@chrisfirst](https://x.com/chrisfirst)) `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**프롬프트:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

---

<a id="사례-4-폰트-패션쇼-작성자-hbcoop_"></a>
### 사례 4: [폰트 패션쇼](https://x.com/HBCoop_/status/2057856570558452142) (작성자 [@HBCoop_](https://x.com/HBCoop_)) `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**프롬프트:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

## ⚖️ 비교

<a id="사례-1-seedance-20-vs-gemini-omni-flash-작성자-jsfilmz0412"></a>
### 사례 1: [Seedance 2.0 vs Gemini Omni Flash](https://x.com/JSFILMZ0412/status/2057926749598736635) (작성자 [@JSFILMZ0412](https://x.com/JSFILMZ0412)) `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — 스타일 전환, 모션 품질 및 검열 비교.

---

<a id="사례-2-gemini-omni-vs-seedance-20-액션-장면-작성자-curiousrefuge"></a>
### 사례 2: [Gemini Omni vs Seedance 2.0 액션 장면](https://x.com/CuriousRefuge/status/2057929340562907451) (작성자 [@CuriousRefuge](https://x.com/CuriousRefuge)) `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni 비디오 편집 모델 vs Seedance 2.0 — 대형 액션 장면 비교.

## 🧪 평가

<a id="사례-1-gemini-omni-품질-평가-작성자-kenichiota0711"></a>
### 사례 1: [Gemini Omni 품질 평가](https://x.com/kenichiota0711/status/2057820346850660769) (작성자 [@kenichiota0711](https://x.com/kenichiota0711)) `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

## 🌐 커뮤니티 갤러리

커뮤니티의 창의적인 실험과 쇼케이스. 이 사례들은 Gemini Omni로 가능한 것의 폭을 보여줍니다.

<table>
<tr>
<td width="50%" valign="top">

**[컨셉 기반 교육 비디오](https://x.com/VORTEX_Promos/status/2058083405204459621)** — 작성자 [@VORTEX_Promos](https://x.com/VORTEX_Promos)

https://github.com/user-attachments/assets/ca450aec-a6c8-455f-973d-087bfb3da742

</td>
<td width="50%" valign="top">

**[Showcase](https://x.com/paji_a/status/2058070248436445600)** — 작성자 [@paji_a](https://x.com/paji_a)

https://github.com/user-attachments/assets/8ecfe4b0-6de7-47f0-9b83-3dc736512e54

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[비디오용 Nano Banana — 일관성 테스트](https://x.com/WolfRiccardo/status/2058296266270945483)** — 작성자 [@WolfRiccardo](https://x.com/WolfRiccardo)

https://github.com/user-attachments/assets/0cabc195-8a2b-47e6-a649-d95b15003964

</td>
<td width="50%" valign="top">

**[발표하는 아이소메트릭 캐릭터](https://x.com/kumiko_shiraki/status/2058699566938194382)** — 작성자 [@kumiko_shiraki](https://x.com/kumiko_shiraki)

https://github.com/user-attachments/assets/d38627cd-6f23-4ea3-8a95-7cd831229364

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[한 문장으로 만든 시네마틱 선(禪)](https://x.com/Dheepanratnam/status/2058372209681342806)** — 작성자 [@Dheepanratnam](https://x.com/Dheepanratnam)

https://github.com/user-attachments/assets/d33d9c9d-a68f-4e01-bf1e-c4c8ee60c8ee

</td>
<td width="50%" valign="top">

**[캐릭터 변환 — 화려함에서 일상으로](https://x.com/HBCoop_/status/2058221428780970398)** — 작성자 [@HBCoop_](https://x.com/HBCoop_)

https://github.com/user-attachments/assets/239ca343-cb71-4254-8478-d8947d6c33aa

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Waymo로 인도 가기](https://x.com/iHarnoorSingh/status/2058352557819621617)** — 작성자 [@iHarnoorSingh](https://x.com/iHarnoorSingh)

https://github.com/user-attachments/assets/7d23ad1f-63bf-4a3c-ab94-09e8f26c570e

</td>
<td width="50%" valign="top">

**[부쳐지지 않은 편지 — 단편](https://x.com/Strength04_X/status/2058367252299452851)** — 작성자 [@Strength04_X](https://x.com/Strength04_X)

https://github.com/user-attachments/assets/df8dcb7c-c918-4fc2-b952-0cb2bcdddfee

</td>
</tr>
</table>

<a id="related-repositories"></a>
## 🔗 관련 저장소

- [EvoLink 영상 모델 API 가이드 살펴보기](https://github.com/EvoLinkAI/awesome-ai-video-models-api-guide).
- [EvoLink Media MCP 저장소 사용하기](https://github.com/EvoLinkAI/evolink-media-mcp).
- [EvoLink의 Seedance 2.5 소개 읽기](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=related_seedance).

## 🙏 감사의 말

이 저장소는 우수한 오픈 프롬프트 컬렉션과 커뮤니티 공유 예제에서 영감을 받았습니다.

이러한 사례 연구를 가능하게 한 공식 Gemini Omni 데모와 프롬프트 가이드를 공개해 주신 Google DeepMind에 감사드립니다.

**커뮤니티 기여자:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711), [@tanabe_fragm](https://x.com/tanabe_fragm), [@venturetwins](https://x.com/venturetwins), [@kumiko_shiraki](https://x.com/kumiko_shiraki), [@Majin_AppSheet](https://x.com/Majin_AppSheet), [@mmmiyama_D](https://x.com/mmmiyama_D), [@VORTEX_Promos](https://x.com/VORTEX_Promos), [@paji_a](https://x.com/paji_a), [@WolfRiccardo](https://x.com/WolfRiccardo), [@Dheepanratnam](https://x.com/Dheepanratnam), [@iHarnoorSingh](https://x.com/iHarnoorSingh), [@Strength04_X](https://x.com/Strength04_X)

*수정이 필요한 사항이 있으면 연락해 주시면 업데이트하겠습니다.*

더 흥미로운 프롬프트 사례를 공유하고 싶으시다면, 연락해 주셔서 Evolink 프롬프트 라이브러리 확장에 도움을 주세요.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&Date)

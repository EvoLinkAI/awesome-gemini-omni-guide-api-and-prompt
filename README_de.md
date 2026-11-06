<div align="center">

<a href="https://evolink.ai/gemini-omni?utm_source=github&utm_medium=banner&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=readme_banner"><img src="image/guide-banner.png" width="760" alt="Gemini Omni Leitfaden und Prompt-Sammlung"></a>

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![Gemini Omni 1.2 Flash ausprobieren](https://img.shields.io/badge/Try_Gemini_Omni_1.2_Flash-EvoLink-black)](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=badge&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=model_try)

[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Default_Source-111111)](README.md) [![🇪🇸 Español](https://img.shields.io/badge/🇪🇸_Español-Ver-ffb703)](README_es.md) [![🇵🇹 Português](https://img.shields.io/badge/🇵🇹_Português-Ver-2a9d8f)](README_pt.md) [![🇯🇵 日本語](https://img.shields.io/badge/🇯🇵_日本語-表示-52b788)](README_ja.md) [![🇰🇷 한국어](https://img.shields.io/badge/🇰🇷_한국어-보기-4ea8de)](README_ko.md) [![🇩🇪 Deutsch](https://img.shields.io/badge/🇩🇪_Deutsch-Ansehen-f4a261)](README_de.md) [![🇫🇷 Français](https://img.shields.io/badge/🇫🇷_Français-Voir-e76f51)](README_fr.md) [![🇹🇷 Türkçe](https://img.shields.io/badge/🇹🇷_Türkçe-Görüntüle-d62828)](README_tr.md) [![🇹🇼 繁體中文](https://img.shields.io/badge/🇹🇼_繁體中文-查看-8338ec)](README_zh-TW.md) [![🇨🇳 简体中文](https://img.shields.io/badge/🇨🇳_简体中文-查看-ef476f)](README_zh-CN.md) [![🇷🇺 Русский](https://img.shields.io/badge/🇷🇺_Русский-Смотреть-577590)](README_ru.md)

</div>

# Gemini Omni 1.2 Flash: Leitfaden und Prompt-Sammlung

## 🍌 Einführung
**Ein Leitfaden zu Gemini Omni 1.2 Flash mit einer erhaltenen Sammlung von Prompts der Gemini-Omni-Familie, Bearbeitungsdemos, Vergleichen und Community-Videos.** Er hilft Kreativen und Entwicklern, eine passende Aufgabe auszuwählen und deren Ein- und Ausgabegrenzen zu verstehen.

> [!NOTE]
> Die bisherigen Prompt-Fälle, Vergleiche und die Community-Galerie sind historisches Material zur Gemini-Omni-Familie. Ihre ursprünglichen Prompts, Quellen und Medien bleiben erhalten; sie werden nicht als Ergebnisse oder Benchmarks von Gemini Omni 1.2 Flash dargestellt.

<a id="omni-1-2-guide"></a>
## 🆕 Gemini Omni 1.2 Flash

Google führt Gemini Omni 1.2 Flash als allgemein verfügbar (GA), mit Veröffentlichung am **5. November 2026**. Die wichtigsten Änderungen gegenüber 1.1 sind die Generierung von bis zu **15 Sekunden** auf den entsprechenden Routen und die **eigenständige Video-Hochskalierung**. Lies die [Google-Modellspezifikation](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-1-2-flash) und die [EvoLink-Ankündigung vom 5. November](https://evolink.ai/changelog?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=release_source#2026-11-05-gemini-omni-1-2-flash).

- Text-, Bild- und Videoeingaben; Videoausgabe mit synchronisierter Sprache, Musik und Geräuschen. Audiodateien als Eingabe und Tonbearbeitung werden nicht unterstützt.
- Native Ausgabe in **360p / 720p**; **1080p / 4K wird hochskaliert** und ist kein natives 4K. Dokumentiert sind 24 Bilder pro Sekunde sowie 16:9 oder 9:16.
- Text-zu-Video und ein einzelnes Bild als Startbild unterstützen **3–15 Sekunden**. Die Interpolation zwischen erstem und letztem Bild bleibt auf **3–10 Sekunden** begrenzt.
- Die Videoverlängerung fügt **3–10 Sekunden** hinzu; dieser Wert bezeichnet die zusätzliche Dauer, nicht die Gesamtlänge des fertigen Videos.

### Eine EvoLink-Aufgabe auswählen

Jede Aufgabe verlinkt auf ihre eigene Anfragespezifikation. Lies die [vollständige Parameterübersicht](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=parameter_overview), bevor du die Route wechselst.

| Aufgabe | Geeignet für | Routenspezifische Grenzen |
| :--- | :--- | :--- |
| [Text-zu-Video-Dokumentation lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-text-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_text) | Eine Aufnahme aus einem Text-Prompt erstellen. | 3–15 Sekunden. |
| [Bild-zu-Video-Dokumentation lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-image-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_image) | Ein Startbild animieren oder ein erstes und letztes Bild verbinden. | Ein Bild: 3–15 Sekunden; zwei Bilder: 3–10 Sekunden. |
| [Referenz-zu-Video-Dokumentation lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-reference-to-video?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_reference) | Eine neue Aufnahme anhand von Bild- oder Videoreferenzen gestalten. | Bis zu 10 Bilder und 3 Referenzvideos; bei mehr als 10 Sekunden Ausgabedauer höchstens 1 Referenzvideo. |
| [Dokumentation zur Videobearbeitung lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-edit?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_edit) | Einen vorhandenen Clip mithilfe eines Prompts verändern. | Ein Eingabevideo bis zu 15 Sekunden; optionale Referenzbilder; die Qualität ist standardmäßig `auto`. |
| [Dokumentation zur Videoverlängerung lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-extend?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_extend) | Das Ende eines Clips fortsetzen. | Ein Eingabevideo bis zu 30 Sekunden; 3–10 Sekunden werden angefügt. |
| [Dokumentation zur Video-Hochskalierung lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-video-upscale?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=route_upscale) | Die Auflösung eines ausgewählten fertigen Clips erhöhen. | Eingabe bis zu 15 Sekunden in einer unterstützten Standardgröße; kein Prompt. Beachte die folgenden Plattformunterschiede. |

### Unterschiede zwischen Plattformen und Versionen

- **Referenzen:** Die [AI-Studio-Nutzungsanleitung](https://aistudio.google.com/docs/omni) erlaubt bis zu 6 Bilder, während Google Cloud und EvoLink bis zu 10 dokumentieren. Die Grenzen für Referenzvideos hängen auch von der Ausgabedauer ab; verwende die Spezifikation der gewählten Plattform.
- **Hochskalierung:** Google Cloud dokumentiert 360p→720p/1080p und 720p→1080p/4K und schließt 1080p→4K aus. Die EvoLink-Dokumentation führt zusätzlich 1080p→4K auf. Kläre diese zusätzliche Kombination mit der gewählten Plattform; sie ist keine plattformübergreifende Zusicherung. Lies die [Google-Einschränkungen zur Hochskalierung](https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/video/upscale-videos).
- **Gesprächszustand:** Die Interactions API von Google unterstützt dialogbasierte Bearbeitung. Asynchrone Videoaufgaben von EvoLink verwenden ihre eigene Anfragespezifikation; übertrage `previous_interaction_id` oder andere ausschließlich für Google vorgesehene Parameter nicht darauf.
- **Migration:** Die [Google-Modellseite](https://aistudio.google.com/docs/models/gemini-omni-flash) kündigt an, dass die stabile 1.1-Modell-ID der Gemini API ab dem 3. Dezember 2026 auf 1.2 weitergeleitet wird. Daraus folgt keine Migration der 1.1-Routen von EvoLink. Wähle die ausdrückliche 1.2-Aufgabe, statt die alte generische ID als Alias zu behandeln.
- **Kosten:** Die EvoLink-Modellseite zeigt tokenbasierte Preise; ein Tokenpreis ist kein fester Preis pro Sekunde oder fertigem Clip. Prüfe vor einer Kostenschätzung die aktuelle Route, die Auflösung und den tatsächlichen Verbrauch.

Quellen geprüft am **6. November 2026**.

<a id="quick-start"></a>
## ⚡ Schnellstart

[Gemini Omni 1.2 Flash im Browser ausprobieren](https://evolink.ai/gemini-omni-1-2-flash?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=browser_try) oder [die aktuelle Aufgabendokumentation lesen](https://evolink.ai/docs/en/api-manual/video-series/gemini-omni-1.2-flash/gemini-omni-1.2-flash-overview?utm_source=github&utm_medium=quickstart&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=task_docs).

Wähle in der obigen Aufgabentabelle Text-zu-Video, Bild-zu-Video, Referenzen, Bearbeitung, Verlängerung oder Hochskalierung. Die aktuelle Dokumentation der gewählten Aufgabe beschreibt ihre Eingaben, Grenzen und den Ablauf bis zum Ergebnis.

## 📑 Menü
- [Leitfaden zu Gemini Omni 1.2 Flash](#omni-1-2-guide)
- [Schnellstart](#quick-start)
- [Offizielle Demos zu Gemini Omni 1.2](#omni12-demos)
- [🎯 Prompt-Zutaten](#-prompt-zutaten)
- [✂️ Bearbeitung](#️-bearbeitung)
  - [🔄 Element-Ersetzung](#-element-ersetzung)
    - [Fall 1: Schmetterling zu Biene](#fall-1-schmetterling-zu-biene)
    - [Fall 2: Biene zu Glühwürmchen](#fall-2-biene-zu-glühwürmchen)
    - [Fall 3-5: Raumschiffe & Astronauten-Serie](#fall-3-5-raumschiffe--astronauten-serie)
    - [Fall 6: Zug 1896 Transformation (von @emollick)](#fall-6-zug-1896-transformation-von-emollick)
    - [Fall 7: Person aus Video entfernen (von @arrakis_ai)](#fall-7-person-aus-video-entfernen-von-arrakis_ai)
    - [Fall 8: Unsichtbare Geige](#fall-8-unsichtbare-geige)
    - [Fall 9: Standortwechsel durch Weltwissen (von @venturetwins)](#fall-9-standortwechsel-durch-weltwissen-von-venturetwins)
    - [Fall 10: Animation zu Realfilm (von @arrakis_ai)](#fall-10-animation-zu-realfilm-von-arrakis_ai)
  - [🎬 Basisszene](#-basisszene)
    - [Fall 1: Geiger Basisaufnahme](#fall-1-geiger-basisaufnahme)
  - [📷 Kameraführung](#-kameraführung)
    - [Fall 1: Über-die-Schulter-Perspektive](#fall-1-über-die-schulter-perspektive)
    - [Fall 2: Kameraneigung Schuhe zur Halbtotale](#fall-2-kameraneigung-schuhe-zur-halbtotale)
    - [Fall 3: Reise-Selfie-Hyperlapse (von @ZaraIrahh)](#fall-3-reise-selfie-hyperlapse-von-zarairahh)
    - [Fall 4: Mode-Drohnenaufnahme (von @ariaxawan)](#fall-4-mode-drohnenaufnahme-von-ariaxawan)
    - [Fall 5: Draufsicht zu 360-Grad-Rotation (von @npaka123)](#fall-5-draufsicht-zu-360-grad-rotation-von-npaka123)
    - [Fall 6: Omnizoom — Eintauchen in ein Foto (von @alexanderchen)](#fall-6-omnizoom--eintauchen-in-ein-foto-von-alexanderchen)
  - [🎬 Aktion & Synchronisation](#-aktion--synchronisation)
    - [Fall 1: Tierspielzeug-Geräusch](#fall-1-tierspielzeug-geräusch)
    - [Fall 2: Wohnungslichter-Synchronisation](#fall-2-wohnungslichter-synchronisation)
    - [Fall 3: Murmel-Kettenreaktion](#fall-3-murmel-kettenreaktion)
    - [Fall 4: Gebäudelichter](#fall-4-gebäudelichter)
    - [Fall 5: Boxkampf Realistisch (von @RuzainaMeer)](#fall-5-boxkampf-realistisch-von-ruzainameer)
- [🎨 Erweitert Multi-Modal](#-erweitert-multi-modal)
  - [🪞 Künstlerischer Stil](#-künstlerischer-stil)
    - [Fall 1-3: Spiegel-Serie](#fall-1-3-spiegel-serie)
    - [Fall 4: Animations-Werbung One Shot (von @DenneyDara)](#fall-4-animations-werbung-one-shot-von-denneydara)
    - [Fall 5: Strichzeichnung-Isolation (von @alexanderchen)](#fall-5-strichzeichnung-isolation-von-alexanderchen)
  - [✨ Visuelle Effekte](#-visuelle-effekte)
    - [Fall 1: Hand-Loch Super-Zoom](#fall-1-hand-loch-super-zoom)
    - [Fall 2: Skateboard-Bewegungseffekte](#fall-2-skateboard-bewegungseffekte)
    - [Fall 3: AR HUD Overlay (von @jerrod_lew)](#fall-3-ar-hud-overlay-von-jerrod_lew)
  - [🔗 Cross-Modal](#-cross-modal)
    - [Fall 1: Transport in neue Umgebung](#fall-1-transport-in-neue-umgebung)
    - [Fall 2: Vogelformation mit Audio](#fall-2-vogelformation-mit-audio)
    - [Fall 3: Folie zu Bewegung (von @yoshifujidesign)](#fall-3-folie-zu-bewegung-von-yoshifujidesign)
    - [Fall 4: Isometrischer Koch-Charakter mit Referenzbild (von @kumiko_shiraki)](#fall-4-isometrischer-koch-charakter-mit-referenzbild-von-kumiko_shiraki)
    - [Fall 5: ChatGPT-Anweisungsbild als Eingabe (von @Majin_AppSheet)](#fall-5-chatgpt-anweisungsbild-als-eingabe-von-majin_appsheet)
    - [Fall 6: ChatGPT-Illustration zu Omni-Animation (von @mmmiyama_D)](#fall-6-chatgpt-illustration-zu-omni-animation-von-mmmiyama_d)
  - [📋 Storyboard](#-storyboard)
    - [Fall 1: Luxus-Kosmetik-Werbespot (von @aiwithaly)](#fall-1-luxus-kosmetik-werbespot-von-aiwithaly)
    - [Fall 2: Zeig mich in dieser Geschichte](#fall-2-zeig-mich-in-dieser-geschichte)
    - [Fall 3: 3x3 Splitscreen (von @alexanderchen)](#fall-3-3x3-splitscreen-von-alexanderchen)
    - [Fall 4: Action-Replay aus verschiedenen Winkeln (von @jerrod_lew)](#fall-4-action-replay-aus-verschiedenen-winkeln-von-jerrod_lew)
    - [Fall 5: Splitscreen-Video (von @jerrod_lew)](#fall-5-splitscreen-video-von-jerrod_lew)
  - [🔤 Textdarstellung](#-textdarstellung)
    - [Fall 1: Alphabet-Gegenstände-Sequenz](#fall-1-alphabet-gegenstände-sequenz)
    - [Fall 2: Wort-für-Wort Text-Synchronisation](#fall-2-wort-für-wort-text-synchronisation)
    - [Fall 3: Textdarstellung KI-Nachrichten (von @chrisfirst)](#fall-3-textdarstellung-ki-nachrichten-von-chrisfirst)
    - [Fall 4: Schriftarten-Modenschau (von @HBCoop_)](#fall-4-schriftarten-modenschau-von-hbcoop_)
- [⚖️ Vergleich](#️-vergleich)
  - [Fall 1: Seedance 2.0 vs Gemini Omni Flash (von @JSFILMZ0412)](#fall-1-seedance-20-vs-gemini-omni-flash-von-jsfilmz0412)
  - [Fall 2: Gemini Omni vs Seedance 2.0 Actionszenen (von @CuriousRefuge)](#fall-2-gemini-omni-vs-seedance-20-actionszenen-von-curiousrefuge)
- [🧪 Bewertung](#-bewertung)
  - [Fall 1: Gemini Omni Qualitätsbewertung (von @kenichiota0711)](#fall-1-gemini-omni-qualitätsbewertung-von-kenichiota0711)
- [🌐 Community-Galerie](#-community-galerie)
- [Verwandte Repositories](#related-repositories)
- [🙏 Danksagung](#-danksagung)

<a id="omni12-demos"></a>
## 🎬 Gemini Omni 1.2: Demos

Acht offizielle Demonstrationen, die Google am **5. November 2026** veröffentlicht hat. Lies den [ursprünglichen Ankündigungsartikel](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemini-omni-1-2-flash/); wähle ein Vorschaubild aus, um das Originalvideo von Google anzusehen.

<table>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-1"></a>
**[Virtuelle Anprobe in 15 Sekunden](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)**

[![Virtuelle Anprobe in 15 Sekunden](image/omni-1.2/15-second-virtual-try-on.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/ECom_Try_On_Demo.mp4)

Ein Model-Foto und drei Outfits dienen als Vorgabe für eine 15-sekündige Anprobemontage.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-2"></a>
**[Typografie-Animation in mehreren Ebenen](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)**

[![Typografie-Animation in mehreren Ebenen](image/omni-1.2/layered-typography-animation.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Typographic_Motion_Graphics_Demo.mp4)

Ein animiertes Plakat setzt Materialien und Schriftzüge zusammen; Google zeigt Ergebnisse von 1.1 und 1.2.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-3"></a>
**[Hintergrundwechsel per Dialog](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)**

[![Hintergrundwechsel per Dialog](image/omni-1.2/conversational-background-changes.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Video_Background_Editing_Demo.mp4)

Mehrere aufeinanderfolgende Dialoge ersetzen den Hintergrund eines Clips und erhalten dabei seine beiden Figuren in Rüstung.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-4"></a>
**[Durchgehender Kameraflug durch das Pantheon](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)**

[![Durchgehender Kameraflug durch das Pantheon](image/omni-1.2/continuous-pantheon-flythrough.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Pantheon_Tour_Demo_FuU0KUh.mp4)

Zwei Architekturfotos dienen als Vorgabe für einen durchgehenden Kameraflug durch die Kuppel des Pantheons.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-5"></a>
**[Bienenstock-Erklärvideo in 15 Sekunden](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)**

[![Bienenstock-Erklärvideo in 15 Sekunden](image/omni-1.2/15-second-beehive-explainer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Bee_Hive_Live_Infographic_Demo_ninuxtc.mp4)

Aus einem Stilreferenzbild entsteht ein illustriertes Erklärvideo über einen Bienenstock mit vier Einstellungen und 15 Sekunden Länge.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-6"></a>
**[Bewegungsübertragung vom Oktopus auf eine Tänzerin](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)**

[![Bewegungsübertragung vom Oktopus auf eine Tänzerin](image/omni-1.2/octopus-to-dancer-motion-transfer.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Unexpected_Motion_Tracking_Demo_QRzpS2T.mp4)

Eine anschließende Bearbeitung überträgt die fließende Bewegung eines Oktopus auf das Kleid einer Tänzerin.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a id="omni12-demo-7"></a>
**[Ramen-Lokal zwischen erstem und letztem Bild](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)**

[![Ramen-Lokal zwischen erstem und letztem Bild](image/omni-1.2/first-to-last-frame-ramen-shop.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Ramen_Bar_Demo_jeWGtqx.mp4)

Das erste und letzte Bild verbinden Außen- und Innenansicht eines Ramen-Lokals; Googles Vergleich enthält sichtbare Unstimmigkeiten.

</td>
<td width="50%" valign="top">

<a id="omni12-demo-8"></a>
**[Durchgehendes Herauszoomen von einer Insel](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)**

[![Durchgehendes Herauszoomen von einer Insel](image/omni-1.2/continuous-island-zoom-out.webp)](https://storage.googleapis.com/gweb-uniblog-publish-prod/original_videos/Castaway_Crash_Zoom_Out_Demo.mp4)

Eine zehnsekündige Aufnahme zieht sich von einer Nahansicht der Küste bis zu einer weiten Inselansicht zurück.

</td>
</tr>
</table>

## 🎯 Prompt-Zutaten
Gemini Omni verfügt über ein starkes **Weltverständnis** — es greift auf reales Wissen über Geschichte, Wissenschaft und Kultur zurück. Du musst nicht jedes Detail übermäßig erklären. Drücke stattdessen deine kreative Absicht in natürlicher Sprache aus und lass Omnis Reasoning den Rest ergänzen.
Wenn du ein neues Video von Grund auf erstellst, kombiniere diese Dimensionen, um die Ausgabe zu steuern:
| Dimension | Was angegeben werden sollte | Beispiel |
| :--- | :--- | :--- |
| **Bildausschnitt & Bewegung** | Weitwinkel, Halbtotale oder Nahaufnahme. Kameratrajektorie: sanftes Gleiten, plötzlicher Schwenk, statische Fixierung, Dolly-Zoom usw. | `A close-up tracking shot smoothly pushing in` |
| **Stil** | Gesamte visuelle Art Direction | `Vintage monochrome hologram`, `3D voxel art`, `colored crayon aesthetic` |
| **Beleuchtung** | Szenen-Stimmung und Lichtaufbau | `Warm champagne lighting`, `dim overhead gym lights` |
| **Ort** | Umgebung und Hintergrund | `Small underground gym`, `futuristic neon cityscape` |
| **Aktion** | Verhalten und Bewegung des Subjekts | `The person touches the mirror`, `a marble rolling fast on a chain reaction track` |
> [!TIP]
> **Iteratives Bearbeiten:** Omni unterstützt Multi-Turn-Konversationsbearbeitung. Es bewahrt, was funktioniert, und ändert nur das, was du verlangst — du musst nicht jedes Mal die gesamte Szene neu beschreiben. Sage einfach, was als Nächstes geändert werden soll.

> [!TIP]
> **[Unveränderte Bereiche bewahren](https://x.com/tanabe_fragm/status/2058103447006896406) (von [@tanabe_fragm](https://x.com/tanabe_fragm)):** Beim Bearbeiten von Videos füge Sätze wie "Ändere nichts anderes" oder "Behalte alles andere unverändert" zu deinem Prompt hinzu. Dies reduziert deutlich ungewollte Änderungen an Teilen, die du nicht modifizieren wolltest.
>
> https://github.com/user-attachments/assets/285ee7d8-7dfe-4304-a9a4-648026073b80

## ✂️ Bearbeitung

### 🔄 Element-Ersetzung

<a id="fall-1-schmetterling-zu-biene"></a>
### Fall 1: Schmetterling zu Biene `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/8feb4d7b-825d-4a4a-bd9d-900754cf5d38

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
</tr>
</table>

**Prompt:**

```
Change the butterfly to a bee.
```

---

<a id="fall-2-biene-zu-glühwürmchen"></a>
### Fall 2: Biene zu Glühwürmchen `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/60f31f6d-895e-4048-b477-9a46a5d20b90

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/76fc8e97-c7d1-40bc-9e79-bd6705aa8267

</td>
</tr>
</table>

**Prompt:**

```
Change the bee into a small swarm of fireflies.
```

---

<a id="fall-3-5-raumschiffe--astronauten-serie"></a>
### Fall 3-5: Raumschiffe & Astronauten-Serie `🎬 Video→Video`

<table>
<tr>
<td colspan="3">

**Eingabe:**

https://github.com/user-attachments/assets/26ea7e43-9787-4096-82f9-e10543229bec

</td>
</tr>
<tr>
<td width="300">

https://github.com/user-attachments/assets/dd9ae5b1-0205-45ac-a651-258af1c4f12c

### Fall 3: Raumschiffe zu weißem Origami

</td>
<td width="300">

https://github.com/user-attachments/assets/78ef5301-b759-4dda-9995-3ee0d259a7b1

### Fall 4: Astronaut zu Seeanemone

</td>
<td width="300">

https://github.com/user-attachments/assets/0cbadb19-8a5b-4a2c-9093-e3a84f3dd988

### Fall 5: Kleine Schiffe zu Rochen

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

<a id="fall-6-zug-1896-transformation-von-emollick"></a>
### Fall 6: [Zug 1896 Transformation](https://x.com/emollick/status/2057874739817808223) (von [@emollick](https://x.com/emollick)) `🎬 Video→Video`

https://github.com/user-attachments/assets/275cc90e-adaa-48ff-9ff8-1e96ea29d44f

**Prompt:**

```
I took the famous "train" movie from 1896 & made it a bullet train, LEGO, added a time traveler, a centipede, muppets...
```

---

<a id="fall-7-person-aus-video-entfernen-von-arrakis_ai"></a>
### Fall 7: [Person aus Video entfernen](https://x.com/arrakis_ai/status/2057939231755178439) (von [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/72379fb2-ac30-4d1e-a6b4-143052f8f061

**Prompt:**

```
Remove the person from this video perfectly.
```

---

<a id="fall-8-unsichtbare-geige"></a>
### Fall 8: Unsichtbare Geige `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
</tr>
</table>

**Prompt:**

```
Make the violin invisible
```

---

<a id="fall-9-standortwechsel-durch-weltwissen-von-venturetwins"></a>
### Fall 9: [Standortwechsel durch Weltwissen](https://x.com/venturetwins/status/2058235415883313361) (von [@venturetwins](https://x.com/venturetwins)) `🎬 Video→Video`

https://github.com/user-attachments/assets/daa90750-fc7b-49ea-b85d-364411159663

**Prompt:**

```
Re-shoot this video in [location] based on the screenshot from Google Maps.
```

---

<a id="fall-10-animation-zu-realfilm-von-arrakis_ai"></a>
### Fall 10: [Animation zu Realfilm](https://x.com/arrakis_ai/status/2058488373057302797) (von [@arrakis_ai](https://x.com/arrakis_ai)) `🎬 Video→Video`

https://github.com/user-attachments/assets/3c6be2a9-3e67-4deb-8ccd-fb493b715f65

**Prompt:**

```
Turn this animation into live action.
```

### 🎬 Basisszene

<a id="fall-1-geiger-basisaufnahme"></a>
### Fall 1: Geiger Basisaufnahme `🔤 Text→Video`

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

**Prompt:**

```
A video of a violinist playing a song.
```

### 📷 Kameraführung

<a id="fall-1-über-die-schulter-perspektive"></a>
### Fall 1: Über-die-Schulter-Perspektive `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/ac6457aa-158c-4a0b-852f-ce1f3367bc3f

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/71aa1c8d-0287-4591-b239-68322919293d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle to be over the violinist's shoulder.
```

---

<a id="fall-2-kameraneigung-schuhe-zur-halbtotale"></a>
### Fall 2: Kameraneigung Schuhe zur Halbtotale `🎬 Video→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/19dbc1ae-1e9e-4b7b-9069-e979fffe3651

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/c0ccbda0-4fd0-42be-8620-db7a67a5347d

</td>
</tr>
</table>

**Prompt:**

```
Change the camera angle, a close-up on his shoes, quickly tilting up to medium shot, then widening.
```

---

<a id="fall-3-reise-selfie-hyperlapse-von-zarairahh"></a>
### Fall 3: [Reise-Selfie-Hyperlapse](https://x.com/ZaraIrahh/status/2057775215749349520) (von [@ZaraIrahh](https://x.com/ZaraIrahh)) `🔤 Text→Video`

https://github.com/user-attachments/assets/31fa5a56-6113-4376-873b-5e40d26803f1

**Prompt:**

```
Create a 10-second cinematic hyper-lapse selfie travel video of the uploaded female character across 20 world-famous destinations in 2026. Hard cuts every 0.5 seconds synced to the beat. Handheld selfie-stick camera, wide-angle lens, close selfie framing, energetic travel-vlogger style, vibrant cinematic colors, realistic lighting, dynamic motion blur, natural crowds, and clear landmarks in every shot.
```

---

<a id="fall-4-mode-drohnenaufnahme-von-ariaxawan"></a>
### Fall 4: [Mode-Drohnenaufnahme](https://x.com/ariaxawan/status/2057794715744084042) (von [@ariaxawan](https://x.com/ariaxawan)) `🔤 Text→Video`

https://github.com/user-attachments/assets/b199a5ab-e008-4a72-aa03-094bc6d573e6

**Prompt:**

```
A 10 second ultra cinematic hyper realistic FPV fashion drone shot filmed in a single continuous take inside a futuristic luxury tunnel. Single continuous take, aggressive FPV motion, ultra smooth cinematic flight path, luxury high-fashion editorial atmosphere.
```

---

<a id="fall-5-draufsicht-zu-360-grad-rotation-von-npaka123"></a>
### Fall 5: [Draufsicht zu 360-Grad-Rotation](https://x.com/npaka123/status/2058033145845575735) (von [@npaka123](https://x.com/npaka123)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/1ad202cb-a485-4b7a-9c8c-d4fea4a3b6d5

**Prompt:**

```
この教室の中央から黒板を見ているファーストパーソンなゲーム視点。360度カメラを回転。教室の黒板右側の窓の外は廊下、黒板左側の窓の外は校庭。
```

---

<a id="fall-6-omnizoom--eintauchen-in-ein-foto-von-alexanderchen"></a>
### Fall 6: [Omnizoom — Eintauchen in ein Foto](https://x.com/alexanderchen/status/2058330610574221672) (von [@alexanderchen](https://x.com/alexanderchen)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/9fd3ad2a-6e4a-4ac0-ab29-48f1c303b95f

**Prompt:**

```
Omnizoom — diving into a photo.
```

### 🎬 Aktion & Synchronisation

<a id="fall-1-tierspielzeug-geräusch"></a>
### Fall 1: Tierspielzeug-Geräusch `🎬 Video→Video`

https://github.com/user-attachments/assets/fbf377d7-1b39-43af-92e6-665792d05de0

**Prompt:**

```
When the finger in <video> touches the animal toy play the sound the animal makes
```

---

<a id="fall-2-wohnungslichter-synchronisation"></a>
### Fall 2: Wohnungslichter-Synchronisation `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/6fa879c3-5ee8-4ff1-bbe9-6648d750277d

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/3f010e2a-a471-4b0d-8782-c4c5547cd2a5

</td>
</tr>
</table>

**Prompt:**

```
The lights of the apartments start turning on in sync with the music.
```

---

<a id="fall-3-murmel-kettenreaktion"></a>
### Fall 3: Murmel-Kettenreaktion `🔤 Text→Video`

https://github.com/user-attachments/assets/1ece8df7-f29a-4ebd-ad68-9c910f811590

**Prompt:**

```
A marble rolling fast on a chain reaction style track, continuous smooth shot
```

---

<a id="fall-4-gebäudelichter"></a>
### Fall 4: Gebäudelichter `🎬+🎵 Video+Audio→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/efbc0d8d-b64a-4ef9-afe6-fed4a8b66102

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/51727436-1fc2-426b-afaa-86bb63cfba0f

</td>
</tr>
</table>

**Prompt:**

```
The lights of the buildings start turning on in sync with the music.
```

---

<a id="fall-5-boxkampf-realistisch-von-ruzainameer"></a>
### Fall 5: [Boxkampf Realistisch](https://x.com/RuzainaMeer/status/2057785474446741728) (von [@RuzainaMeer](https://x.com/RuzainaMeer)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6796bf78-8bad-441c-889d-30621ee62cd7

**Prompt:**

```
Ultra-realistic 10-second boxing fight between two women inside a small underground gym. Both fighters look naturally athletic with realistic skin texture, sweat, bruises, and detailed facial expressions. The fight feels raw and authentic, like real professional sparring footage. The camera moves handheld around the ring at close range, capturing fast punches, defensive movement, realistic footwork, and heavy breathing.
```

## 🎨 Erweitert Multi-Modal

### 🪞 Künstlerischer Stil

<a id="fall-1-3-spiegel-serie"></a>
### Fall 1-3: Spiegel-Serie `🎬 Video→Video`

<table>
<tr>
<td width="300">

https://github.com/user-attachments/assets/747cdc6b-f5fa-4482-b745-2839551e9ba2

### Fall 1: Spiegel Flüssigmetall-Welle

</td>
<td width="300">

https://github.com/user-attachments/assets/36ea02a2-3716-44aa-9bc2-a5cc1480d0bf

### Fall 2: Spiegel Strichzeichnung

</td>
<td width="300">

https://github.com/user-attachments/assets/dbca6772-dd7a-4418-a0e6-a39796a91c97

### Fall 3: Spiegel Puppe

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

<a id="fall-4-animations-werbung-one-shot-von-denneydara"></a>
### Fall 4: [Animations-Werbung One Shot](https://x.com/DenneyDara/status/2057844409639551380) (von [@DenneyDara](https://x.com/DenneyDara)) `🔤 Text→Video`

https://github.com/user-attachments/assets/edacf1c5-94db-4687-8eaa-f87ebf5fabee

**Prompt:**

```
Make a Pixar-style video of an aloe leaf that is walking through the forest that talks about how good nature makes it feel. Have it say, "Organic and healthy ingredients make me feel so good."
```

---

<a id="fall-5-strichzeichnung-isolation-von-alexanderchen"></a>
### Fall 5: [Strichzeichnung-Isolation](https://x.com/alexanderchen/status/2057925025915666673) (von [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/787813c0-2e20-4999-8383-fd76a9b21f91

**Prompt:**

```
Extract the key object in this video. Render a video showing that object as a black diagram-style line art drawing on solid 100% white background, nothing else in background. Keep the motion and sound exactly as is.
```

### ✨ Visuelle Effekte

<a id="fall-1-hand-loch-super-zoom"></a>
### Fall 1: Hand-Loch Super-Zoom `🎬 Video→Video`

https://github.com/user-attachments/assets/06683ef4-16e0-47b0-93ec-c6222560ee13

**Prompt:**

```
Make it look like the weird shape of my hand hole super zooms and magnifies the ground it's looking at in sharper quality.
```

---

<a id="fall-2-skateboard-bewegungseffekte"></a>
### Fall 2: Skateboard-Bewegungseffekte `🎬 Video→Video`

https://github.com/user-attachments/assets/44c120a2-38a7-43d7-89fa-a23d0842078c

**Prompt:**

```
Edit this keeping everything the same. Add animated motion effects coming out of the skateboard.
```

---

<a id="fall-3-ar-hud-overlay-von-jerrod_lew"></a>
### Fall 3: [AR HUD Overlay](https://x.com/jerrod_lew/status/2058337271947079977) (von [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/04b11cd7-d345-4172-b6e5-38301e73bb77

**Prompt:**

```
Create a virtual HUD and UI overlay for this recorded phone video, like an AR glasses experience with secondary screens.
```

### 🔗 Cross-Modal

<a id="fall-1-transport-in-neue-umgebung"></a>
### Fall 1: Transport in neue Umgebung `🎬+🖼️ Video+Image→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

https://github.com/user-attachments/assets/93de5898-88ee-4bfc-a36f-19d8aa99dfc1

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/88176743-d17e-48fe-89f3-528fe60df7fd

</td>
</tr>
</table>

**Prompt:**

```
Transport the violinist to the image environment
```

---

<a id="fall-2-vogelformation-mit-audio"></a>
### Fall 2: Vogelformation mit Audio `🎬+🖼️+🎵 Multi-Modal`

<table>
<tr>
<td width="300">

**Eingabe-Video:**

https://github.com/user-attachments/assets/66946870-b366-4981-90b3-c9a35aca69b1

**Eingabe-Bild:**

<img src="image/crossmodal-01.webp" width="200">

**Eingabe-Audio:**

https://github.com/user-attachments/assets/6d79cd06-7805-493c-9f27-6985a3da1866

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/a94efea9-14ac-47c2-ab5f-9492400fdc3a

</td>
</tr>
</table>

**Prompt:**

```
The birds from <video> loosely form the imperfect shape of a bird based on <image>. They move to the music from <audio> and dissipate as they fly
```

---

<a id="fall-3-folie-zu-bewegung-von-yoshifujidesign"></a>
### Fall 3: [Folie zu Bewegung](https://x.com/yoshifujidesign/status/2058032203175731293) (von [@yoshifujidesign](https://x.com/yoshifujidesign)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/f07a861b-cd0d-4894-8ef1-b74520c7cbd7

**Prompt:**

```
GPT image2でスライド作成 → Gemini Omniでモーション。画面遷移もさせられるし、イラストの動かし方も自然。
```

---

<a id="fall-4-isometrischer-koch-charakter-mit-referenzbild-von-kumiko_shiraki"></a>
### Fall 4: [Isometrischer Koch-Charakter mit Referenzbild](https://x.com/kumiko_shiraki/status/2058337185099546885) (von [@kumiko_shiraki](https://x.com/kumiko_shiraki)) `🖼️ Image→Video`

https://github.com/user-attachments/assets/d5e9b97e-cefa-4cd8-bf70-4e633020f092

**Prompt:**

```
Narrow down reference images and add negative prompts to get closer to your ideal output.
```

---

<a id="fall-5-chatgpt-anweisungsbild-als-eingabe-von-majin_appsheet"></a>
### Fall 5: [ChatGPT-Anweisungsbild als Eingabe](https://x.com/Majin_AppSheet/status/2058191091070058846) (von [@Majin_AppSheet](https://x.com/Majin_AppSheet)) `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Eingabe (Anweisungsbilder von ChatGPT):**

<img src="image/049_majin_appsheet_instruction_image_photo_0.jpg" width="280">

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/578d6968-c6dd-417a-b6fe-100468851f3d

</td>
</tr>
</table>

---

<a id="fall-6-chatgpt-illustration-zu-omni-animation-von-mmmiyama_d"></a>
### Fall 6: [ChatGPT-Illustration zu Omni-Animation](https://x.com/mmmiyama_D/status/2058654389326516656) (von [@mmmiyama_D](https://x.com/mmmiyama_D)) `🖼️ Image→Video`

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

### 📋 Storyboard

<a id="fall-1-luxus-kosmetik-werbespot-von-aiwithaly"></a>
### Fall 1: [Luxus-Kosmetik-Werbespot](https://x.com/aiwithaly/status/2057806821138858314) (von [@aiwithaly](https://x.com/aiwithaly)) `🔤 Text→Video`

https://github.com/user-attachments/assets/6d003859-eb77-4466-9f70-5a76a2269667

**Prompt:**

```
Create a cinematic 10-second ultra-realistic luxury cosmetic commercial in a high-end skincare advertisement style. Use warm champagne lighting, glossy beauty-film aesthetic, shallow depth of field, macro beauty cinematography, smooth cinematic camera movement. 10 scenes from macro serum droplets to final payoff shot.
```

---

<a id="fall-2-zeig-mich-in-dieser-geschichte"></a>
### Fall 2: Zeig mich in dieser Geschichte `🖼️ Image→Video`

<table>
<tr>
<td width="300">

**Eingabe:**

<img src="image/storyboard-01.webp" width="280">
<img src="image/storyboard-01-02.webp" width="280">

</td>
<td width="300">

**Ausgabe:**

https://github.com/user-attachments/assets/8429423d-9b72-4cb6-9e8c-985818f160a7

</td>
</tr>
</table>

**Prompt:**

```
Show me in this story. Follow the story exactly in order starting top left. Entire story in 10 seconds. Cinematic
```

---

<a id="fall-3-3x3-splitscreen-von-alexanderchen"></a>
### Fall 3: [3x3 Splitscreen](https://x.com/alexanderchen/status/2057861567396368841) (von [@alexanderchen](https://x.com/alexanderchen)) `🎬 Video→Video`

https://github.com/user-attachments/assets/587fc95e-526f-4d8d-94c8-feefe34edba9

**Prompt:**

```
Generate a 3x3 split screen video based on different details you see here. Make each cell different, varying the perspective, composition, zoom, angle, camera movement (some static, some moving). Make some of the cells extreme close-ups with detailed textures. Keep it photorealistic, handheld, raw. Only natural sounds.
```

---

<a id="fall-4-action-replay-aus-verschiedenen-winkeln-von-jerrod_lew"></a>
### Fall 4: [Action-Replay aus verschiedenen Winkeln](https://x.com/jerrod_lew/status/2057838324140953773) (von [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/a1179492-74bd-488c-b594-6bc023269c10

**Prompt:**

```
Gemini Omni can create action replays from different angles. I referenced a video clip with agent instructions to generate replays.
```

---

<a id="fall-5-splitscreen-video-von-jerrod_lew"></a>
### Fall 5: [Splitscreen-Video](https://x.com/jerrod_lew/status/2057944349846249975) (von [@jerrod_lew](https://x.com/jerrod_lew)) `🎬 Video→Video`

https://github.com/user-attachments/assets/8755d95d-a9b2-4f7c-a56d-bfbbcc47f80e

**Prompt:**

```
Use a reference video and ask the agent for a split screen video.
```

### 🔤 Textdarstellung

<a id="fall-1-alphabet-gegenstände-sequenz"></a>
### Fall 1: Alphabet-Gegenstände-Sequenz `🔤 Text→Video`

https://github.com/user-attachments/assets/f7693ec2-ac70-4ac8-813f-8fcb46d90d3d

**Prompt:**

```
The video shows items of the alphabet. An unusual item starting with each letter is shown sitting on a table. All 26 letters must be represented by 26 items with matching lower thirds displaying the letter. Only one item and lower third at a time. Rapid fire, roughly 9 frames per item at 24FPS. Last frame is a slip of paper "THE END".
```

---

<a id="fall-2-wort-für-wort-text-synchronisation"></a>
### Fall 2: Wort-für-Wort Text-Synchronisation `🔤 Text→Video`

https://github.com/user-attachments/assets/03620abc-bcb2-4011-a52b-ce13409853c4

**Prompt:**

```
word by word, one word on the screen at a time: did, you, know, that, this, model, can, do, pretty, good, text!? each word appears with a different animated style, perfect pacing to a rhythm, sizzle reel.
```

---

<a id="fall-3-textdarstellung-ki-nachrichten-von-chrisfirst"></a>
### Fall 3: [Textdarstellung KI-Nachrichten](https://x.com/chrisfirst/status/2057863432469361098) (von [@chrisfirst](https://x.com/chrisfirst)) `🔤 Text→Video`

https://github.com/user-attachments/assets/e7d23502-1ca0-4f47-be76-47ff05390508

**Prompt:**

```
Static shot we see them turn the page 3 times. Every flip we see content on both left and right side of book pages. Each contains a big news story around AI for the year of 2025. Include images and crystal clear text.
```

---

<a id="fall-4-schriftarten-modenschau-von-hbcoop_"></a>
### Fall 4: [Schriftarten-Modenschau](https://x.com/HBCoop_/status/2057856570558452142) (von [@HBCoop_](https://x.com/HBCoop_)) `🔤 Text→Video`

https://github.com/user-attachments/assets/395d767c-7d8e-4367-941b-0190da9a0284

**Prompt:**

```
Create a 10-second avant-garde fashion editorial where every outfit is inspired by a specific Google Font personality. Each second introduces a new model styled around fonts like Playfair Display, Bebas Neue, Orbitron, Pacifico, Rubik Mono One, and Cormorant Garamond. Font names appear integrated into the environment using their exact typography style. High-fashion runway cinematography with bold lighting, mirrored sets, and surreal motion.
```

## ⚖️ Vergleich

<a id="fall-1-seedance-20-vs-gemini-omni-flash-von-jsfilmz0412"></a>
### Fall 1: [Seedance 2.0 vs Gemini Omni Flash](https://x.com/JSFILMZ0412/status/2057926749598736635) (von [@JSFILMZ0412](https://x.com/JSFILMZ0412)) `⚖️ Comparison`

https://github.com/user-attachments/assets/a03e70b5-99c0-4ad8-b26b-9aed6e037f02

> Seedance 2.0 Fast vs Gemini Omni Flash — Stiltransfer, Bewegungsqualität und Zensurvergleich.

---

<a id="fall-2-gemini-omni-vs-seedance-20-actionszenen-von-curiousrefuge"></a>
### Fall 2: [Gemini Omni vs Seedance 2.0 Actionszenen](https://x.com/CuriousRefuge/status/2057929340562907451) (von [@CuriousRefuge](https://x.com/CuriousRefuge)) `⚖️ Comparison`

https://github.com/user-attachments/assets/33e09b7d-2357-481d-8536-dab39e75524b

> Gemini Omni Videobearbeitungsmodell vs Seedance 2.0 — Vergleich großer Actionszenen.

## 🧪 Bewertung

<a id="fall-1-gemini-omni-qualitätsbewertung-von-kenichiota0711"></a>
### Fall 1: [Gemini Omni Qualitätsbewertung](https://x.com/kenichiota0711/status/2057820346850660769) (von [@kenichiota0711](https://x.com/kenichiota0711)) `🧪 Evaluation`

https://github.com/user-attachments/assets/a9adf476-fac9-4ea2-b5ea-90a50192ccfb

> ほぼ理想的なアウトプットで感動。わずかに揺れる花と髪、まばたきの表現、ノートに書く動作の滑らかさ。

## 🌐 Community-Galerie

Kreative Experimente und Showcases aus der Community. Diese Fälle demonstrieren die Bandbreite dessen, was mit Gemini Omni möglich ist.

<table>
<tr>
<td width="50%" valign="top">

**[Konzeptbasiertes Lehrvideo](https://x.com/VORTEX_Promos/status/2058083405204459621)** — von [@VORTEX_Promos](https://x.com/VORTEX_Promos)

https://github.com/user-attachments/assets/ca450aec-a6c8-455f-973d-087bfb3da742

</td>
<td width="50%" valign="top">

**[Showcase](https://x.com/paji_a/status/2058070248436445600)** — von [@paji_a](https://x.com/paji_a)

https://github.com/user-attachments/assets/8ecfe4b0-6de7-47f0-9b83-3dc736512e54

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Nano Banana für Video — Konsistenztest](https://x.com/WolfRiccardo/status/2058296266270945483)** — von [@WolfRiccardo](https://x.com/WolfRiccardo)

https://github.com/user-attachments/assets/0cabc195-8a2b-47e6-a649-d95b15003964

</td>
<td width="50%" valign="top">

**[Präsentierender isometrischer Charakter](https://x.com/kumiko_shiraki/status/2058699566938194382)** — von [@kumiko_shiraki](https://x.com/kumiko_shiraki)

https://github.com/user-attachments/assets/d38627cd-6f23-4ea3-8a95-7cd831229364

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Ein Satz, kinoreife Zen](https://x.com/Dheepanratnam/status/2058372209681342806)** — von [@Dheepanratnam](https://x.com/Dheepanratnam)

https://github.com/user-attachments/assets/d33d9c9d-a68f-4e01-bf1e-c4c8ee60c8ee

</td>
<td width="50%" valign="top">

**[Charakterverwandlung — Von Glamourös zu Alltäglich](https://x.com/HBCoop_/status/2058221428780970398)** — von [@HBCoop_](https://x.com/HBCoop_)

https://github.com/user-attachments/assets/239ca343-cb71-4254-8478-d8947d6c33aa

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Waymo nach Indien](https://x.com/iHarnoorSingh/status/2058352557819621617)** — von [@iHarnoorSingh](https://x.com/iHarnoorSingh)

https://github.com/user-attachments/assets/7d23ad1f-63bf-4a3c-ab94-09e8f26c570e

</td>
<td width="50%" valign="top">

**[Der nie gesendete Brief — Kurzfilm](https://x.com/Strength04_X/status/2058367252299452851)** — von [@Strength04_X](https://x.com/Strength04_X)

https://github.com/user-attachments/assets/df8dcb7c-c918-4fc2-b952-0cb2bcdddfee

</td>
</tr>
</table>

<a id="related-repositories"></a>
## 🔗 Verwandte Repositories

- [Den EvoLink-API-Leitfaden für Videomodelle erkunden](https://github.com/EvoLinkAI/awesome-ai-video-models-api-guide).
- [Das EvoLink-Media-MCP-Repository verwenden](https://github.com/EvoLinkAI/evolink-media-mcp).
- [Seedance 2.5 auf EvoLink erkunden](https://evolink.ai/launch/seedance-2-5?utm_source=github&utm_medium=readme&utm_campaign=awesome-gemini-omni-guide-api-and-prompt&utm_content=related_seedance).

## 🙏 Danksagung

Dieses Repository wurde von hervorragenden offenen Prompt-Sammlungen und von der Community geteilten Beispielen inspiriert.

Vielen Dank an Google DeepMind für die Veröffentlichung offizieller Gemini Omni Demos und Prompt-Anleitungen, die diese Fallstudien ermöglicht haben.

**Community-Mitwirkende:**

[@emollick](https://x.com/emollick), [@jerrod_lew](https://x.com/jerrod_lew), [@arrakis_ai](https://x.com/arrakis_ai), [@npaka123](https://x.com/npaka123), [@yoshifujidesign](https://x.com/yoshifujidesign), [@chrisfirst](https://x.com/chrisfirst), [@DenneyDara](https://x.com/DenneyDara), [@ZaraIrahh](https://x.com/ZaraIrahh), [@alexanderchen](https://x.com/alexanderchen), [@ariaxawan](https://x.com/ariaxawan), [@RuzainaMeer](https://x.com/RuzainaMeer), [@aiwithaly](https://x.com/aiwithaly), [@HBCoop_](https://x.com/HBCoop_), [@JSFILMZ0412](https://x.com/JSFILMZ0412), [@CuriousRefuge](https://x.com/CuriousRefuge), [@kenichiota0711](https://x.com/kenichiota0711), [@tanabe_fragm](https://x.com/tanabe_fragm), [@venturetwins](https://x.com/venturetwins), [@kumiko_shiraki](https://x.com/kumiko_shiraki), [@Majin_AppSheet](https://x.com/Majin_AppSheet), [@mmmiyama_D](https://x.com/mmmiyama_D), [@VORTEX_Promos](https://x.com/VORTEX_Promos), [@paji_a](https://x.com/paji_a), [@WolfRiccardo](https://x.com/WolfRiccardo), [@Dheepanratnam](https://x.com/Dheepanratnam), [@iHarnoorSingh](https://x.com/iHarnoorSingh), [@Strength04_X](https://x.com/Strength04_X)

*Falls etwas korrigiert werden muss, kontaktiere uns bitte und wir werden es aktualisieren.*

Wenn du weitere interessante Prompt-Fälle teilen möchtest, melde dich gerne und hilf uns, die Evolink Prompt-Bibliothek zu erweitern.

[![Star History Chart](https://api.star-history.com/svg?repos=EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&type=Date)](https://www.star-history.com/#EvoLinkAI/awesome-gemini-omni-guide-api-and-prompt&Date)

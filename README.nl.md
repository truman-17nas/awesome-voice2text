# Awesome Voice Input

> Een verzameling van open-source spraakinvoer-/dicteersoftware — volledig open, uitbreidbaar en licht. Afgestemd op Typeless, Lazytype en Shandianshuo (闪电说), die allemaal closed-source zijn.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Als deze lijst nuttig is, geef dan ⭐ aan de repo — het helpt anderen om deze te vinden.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · **Nederlands** · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Inhoud

- [Benchmarks (closed source)](#benchmarks-closed-source)
- [Waarom deze lijst](#waarom-deze-lijst)
- [Selectiecriteria](#selectiecriteria)
- [Topkeuzes](#topkeuzes)
- [Alle projecten](#alle-projecten)
- [Categorieoverzicht](#categorieoverzicht)
  - [Cross-platform desktop realtime dicteer](#cross-platform-desktop-realtime-dicteer)
  - [Native macOS-dicteer](#native-macos-dicteer)
  - [AI-spraakschoonmaak / LLM-nabewerking](#ai-spraakschoonmaak-llm-nabewerking)
  - [Lokale/offline STT-engines en toolkits](#lokaleoffline-stt-engines-en-toolkits)
  - [Systeemniveau spraakinvoer / IME](#systeemniveau-spraakinvoer-ime)
  - [Chinese spraakinvoer / IME](#chinese-spraakinvoer-ime)
  - [Browser en web spraakinvoer](#browser-en-web-spraakinvoer)
  - [Mobiele spraakinvoer (non-IME)](#mobiele-spraakinvoer-non-ime)
  - [Lichte scripts, CLI en spraakbesturing](#lichte-scripts-cli-en-spraakbesturing)
  - [Overige](#overige)
- [Open source versus benchmarks](#open-source-versus-benchmarks)
- [Hoe kiezen](#hoe-kiezen)
- [Bijdragen](#bijdragen)
- [Star-Geschiedenis](#star-geschiedenis)
- [Licentie](#licentie)

## Benchmarks (closed source)

| Product | Prijs | Platforms | Model/Engine | Open Source |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: gratis 8K wk/wk; Pro $12/mo jaarlijks ($30/mo maandelijks) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Persoonlijk €25 eenmalig (BYOK Groq); Pro €5/mo gehost | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Gratis (lokaal/BYOK); Pro ¥29/mo of ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Waarom deze lijst

Typeless, Lazytype en Shandianshuo (闪电说) zijn krachtig maar closed-source. Deze lijst verzamelt open-source alternatieven die aan drie criteria voldoen: de code is volledig openbaar, het gereedschap is uitbreidbaar en het blijft licht genoeg om op een persoonlijke machine te draaien. Hij omvat momenteel **75 projecten in 9 categorieën**, allemaal geverifieerd als volledig open source.

## Selectiecriteria

- ✅ **Volledig open source** — alle code op een openbare forge (GitHub, GitLab, Codeberg).
- 🔌 **Uitbreidbaar** — je kunt de functies, modellen of integraties toevoegen die je wilt.
- ⚡ **Lichtgewicht** — minimale bloat, snelle opstart, kleine footprint.

## Topkeuzes

🏆 **[Handy](https://github.com/cjpais/Handy)** — Cross-platform offline spraak-naar-teksttool met Whisper of Parakeet, met globale sneltoetsen en klembordplakken. *Gemeenschapsvlaggenschip — 25,281 sterren, de meest gepolijste keuze.*

**Fit-5 keuzes** (voldoen aan alle drie criteria):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — High-performance C/C++ port van OpenAI Whisper met CPU/GPU-inferentie, quantisatie en cross-platform ondersteuning.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linux offline spraak-naar-teksttool met Vosk die toetsenbordinvoer in elke applicatie simuleert.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux en Wayland push-to-talk spraak-naar-tekst met zeven lokale ASR-engines, GPU-ondersteuning en vergaderingsmodus.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash-script voor offline spraakdictee via Whisper voor TTY, X11, Wayland en WSL met optionele LLM-bewerking.

## Alle projecten

| Naam | ⭐ Sterren | Licentie | Taal | Fit | Open | Ext | LW | Chinees |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 51,163 | MIT | C/C++, CMake, Python/Java/C# bindings | 5 | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | 1,882 | GPL-3.0 | Python | 5 | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | 909 | MIT | Rust | 5 | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | 155 | GPL-2.0 | Bash | 5 | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | 25,281 | MIT | Rust, Tauri, React, TypeScript, Tailwind | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | 19,906 | MIT | Python, PyQt6, Whisper, PyTorch, ONNX Runtime | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [FunASR](https://github.com/modelscope/FunASR) | 18,745 | MIT | Python (PyTorch) | 4 | ⚠️ | ✅ | ⚠️ | ✅ |
| [vosk-api](https://github.com/alphacep/vosk-api) | 14,889 | Apache-2.0 | C++ with Python, Java, C#, Node.js, Rust, Go | 4 | ⚠️ | ✅ | ✅ | ✅ |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | 13,280 | Apache-2.0 | C++, Python, Go, Java, Rust, C#, Swift, JS, Dart | 4 | ✅ | ✅ | ⚠️ | ✅ |
| [Vibe](https://github.com/thewh1teagle/vibe) | 6,635 | MIT | Rust, Tauri, TypeScript, React, whisper.cpp | 4 | ✅ | ✅ | ✅ | ✅ |
| [Epicenter](https://github.com/EpicenterHQ/epicenter) | 4,663 | MIT + AGPL-3.0-or-later | — | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) | 2,821 | Apache-2.0 | Python, PyTorch, Gradio, FFmpeg | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) | 1,541 | GPL-3.0 | Swift | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) | 1,474 | MIT | Swift, Shell, CMake, C, Ruby | 4 | ✅ | ⚠️ | ⚠️ | ✅ |
| [Amical](https://github.com/amicalhq/amical) | 1,388 | MIT | TypeScript, Electron, Next.js, React | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr) | 1,074 | MIT | Python, C/C++, GTK4, Astro | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [whisper-writer](https://github.com/savbell/whisper-writer) | 1,071 | GPL-3.0 | Python | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Transcribro](https://github.com/soupslurpr/Transcribro) | 723 | ISC | Kotlin, Android, C++, Jetpack Compose | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [Whisper IME](https://github.com/woheller69/whisperIME) | 603 | MIT | Java, Android, TensorFlow Lite | 4 | ✅ | ✅ | ✅ | ◐ |
| [Vocalinux](https://github.com/jatinkrmalik/vocalinux) | 404 | GPL-3.0 | Python, GTK, whisper.cpp, VOSK | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [VoiceTypr](https://github.com/moinulmoin/voicetypr) | 389 | AGPL-3.0 | Rust, Tauri, TypeScript, React, Vite, Whisper | 4 | ✅ | ✅ | ✅ | ◐ |
| [HoldSpeak](https://github.com/karolswdev/HoldSpeak) | 277 | Apache-2.0 | Python, FastAPI, Astro, Swift, SQLite | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Chirp](https://github.com/Whamp/chirp-stt) | 191 | MIT | Python | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) | 163 | GPL-3.0 | Python, C++, Shell | 4 | ✅ | ✅ | ✅ | ✅ |
| [Dabri](https://github.com/AshBuk/dabri) | 110 | MIT | Go, whisper.cpp (CGO), YAML | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [hns](https://github.com/primaprashant/hns) | 107 | MIT | Python 3.10+ | 4 | ✅ | ✅ | ✅ | ◐ |
| [Elograf](https://github.com/papoteur-mga/elograf) | 82 | GPL-3.0 | Python 3.7+, PyQt6, Vosk, ujson | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) | 1 | MIT | Swift | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [Voicisst](https://github.com/lucyfromnaarm/voicisst) | 0 | MIT | Python | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [dsnote (Speech Note)](https://github.com/mkiol/dsnote) | 1,525 | MPL-2.0 | C++17, Qt5/QML, CMake, Python | 3.5 | ✅ | ⚠️ | ⚠️ | ✅ |
| [VoiceFlow](https://github.com/infiniV/VoiceFlow) | 393 | MIT | Python, React, Vite, faster-whisper | 3.5 | ✅ | ⚠️ | ✅ | ◐ |
| [voice-input-method](https://github.com/pofice/voice-input-method) | 38 | GPL-3.0-or-later | Python 3.10+ | 3.5 | ✅ | ✅ | ✅ | ✅ |
| [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) | 0 | MIT | JavaScript (Manifest V3), Python | 3.5 | ⚠️ | ✅ | ✅ | ⚠️ |
| [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) | 12,636 | Apache-2.0 | Python, C++ | 3 | ✅ | ✅ | ⚠️ | ✅ |
| [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) | 8,731 | MIT | Python, C/C++ | 3 | ⚠️ | ✅ | ✅ | ✅ |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) | 5,387 | GPL-3.0 | Swift, whisper.cpp | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) | 5,013 | GPL-3.0 | Swift | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) | 4,143 | MIT | TypeScript, React, Electron, Vite, Tailwind CSS | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [Ghost Pepper](https://github.com/matthartman/ghost-pepper) | 2,800 | MIT | Swift | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [WhisperBoard](https://github.com/Saik0s/Whisperboard) | 1,040 | GPL-3.0 | Swift, SwiftUI, TCA, whisper.cpp, Tuist | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [Voquill](https://github.com/voquill/voquill) | 977 | AGPL-3.0 | TypeScript, Rust, React, Vite | 3 | ⚠️ | ✅ | ⚠️ | ⚠️ |
| [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) | 695 | Apache-2.0 | Kotlin, Android SDK 36, Compose | 3 | ⚠️ | ✅ | ⚠️ | ✅ |
| [Pindrop](https://github.com/watzon/pindrop) | 546 | MIT | Swift, SwiftUI, WhisperKit, SwiftData, Sparkle | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [vosk-browser](https://github.com/ccoreilly/vosk-browser) | 520 | Apache-2.0 | TypeScript, JavaScript, WebAssembly | 3 | ✅ | ✅ | ✅ | ◐ |
| [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) | 366 | AGPL-3.0 | Rust, TypeScript, React, Python | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [OpenTypeless](https://github.com/tover0314-w/opentypeless) | 308 | MIT | TypeScript, Rust, React, Tauri | 3 | ✅ | ⚠️ | ✅ | ✅ |
| [voxd](https://github.com/jakovius/voxd) | 266 | MIT | Python | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [whisper-dictation](https://github.com/foges/whisper-dictation) | 219 | MIT | Python | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [Speed of Sound](https://github.com/zugaldia/speedofsound) | 171 | MIT | Kotlin, JVM, GTK, Sherpa ONNX | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [blurt](https://github.com/QuantiusBenignus/blurt) | 107 | GPL-3.0 | JavaScript, Shell, CSS | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) | 77 | MIT | Python 3.10-3.12, tkinter, LiteLLM | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [Aria](https://github.com/Xingxun7777/Aria) | 71 | Apache-2.0 | Python 3.12, PyTorch, CUDA, PySide6 | 3 | ✅ | ✅ | ⚠️ | ✅ |
| [Vosk Android Service](https://github.com/alphacep/vosk-android-service) | 64 | Apache-2.0 | Java, Android SDK, Gradle, Vosk, JNA, RxJava2 | 3 | ✅ | ✅ | ✅ | ◐ |
| [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) | 59 | MIT | Python, PyTorch, customtkinter | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [TalkType](https://github.com/lmacan1/talktype) | 54 | MIT | Python | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [FnKey](https://github.com/evoleinik/fnkey) | 45 | GPL-3.0 | Rust | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) | 29 | MIT | Python, faster-whisper, CTranslate2, pyaudio | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [Speechfire](https://github.com/Jejkobb/Speechfire) | 27 | None | JavaScript, Python | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
| [Osprey](https://github.com/osprey-voice/osprey) | 26 | MIT | Python | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [whisper-dictation](https://github.com/jacopone/whisper-dictation) | 18 | MIT | Python, Nix | 3 | ✅ | ✅ | ✅ | — |
| [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) | 15 | MIT | Electron, React, TypeScript | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) | 13 | MIT | JavaScript (React) | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [Dictus](https://github.com/getdictus/dictus-ios) | 12 | MIT | Swift, SwiftUI, WhisperKit, CoreML | 3 | ✅ | ✅ | ✅ | ⚠️ |
| [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) | 11 | MIT | Python | 3 | ⚠️ | ✅ | ⚠️ | ⚠️ |
| [hush](https://github.com/djmunro/hush) | 6 | MIT | Rust | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [freespeak](https://github.com/Zetaphor/freespeak) | 6 | MIT | Python, PyQt6, JavaScript, HTML, CSS | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [WhisperDictation](https://github.com/sam-pop/WhisperDictation) | 1 | MIT | Swift, C/C++ | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
| [voico](https://github.com/Kirera-Wainaina/voico) | 1 | MIT | TypeScript, JavaScript, Node.js, Chrome MV3 | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [localflow](https://github.com/sidharth-n/localflow) | 0 | Apache-2.0 | Python | 3 | ⚠️ | ✅ | ✅ | ◐ |
| [yammer](https://github.com/andynu/yammer) | 0 | MIT | Rust, Tauri, TypeScript, Node.js | 3 | ✅ | ✅ | ⚠️ | ⚠️ |
| [whisper_dictation](https://github.com/themanyone/whisper_dictation) | 291 | GPL-2.0 | Python, C/C++, GStreamer | 2 | ✅ | ✅ | ⚠️ | ◐ |
| [OmniDictate](https://github.com/gurjar1/OmniDictate) | 141 | CC BY-NC 4.0 | Python, PySide6, faster-whisper | 2 | ⚠️ | ⚠️ | ⚠️ | ◐ |
| [seamless](https://github.com/woheller69/seamless) | 84 | MIT | Java, Kotlin, Android | 2 | ⚠️ | ⚠️ | ⚠️ | ⚠️ |
| [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) | 25 | MIT | Python | 2 | ✅ | ⚠️ | ⚠️ | ⚠️ |
| [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) | 9 | GPL-3.0 | Python | 2 | ✅ | ⚠️ | ⚠️ | ◐ |

## Categorieoverzicht

### Cross-platform desktop realtime dicteer

Whisper-gebaseerde desktop-dicteerapps voor Linux, Windows of cross-platform, met push-to-talk, lokale transcriptie en auto-invoer.

- [Handy](https://github.com/cjpais/Handy) — Cross-platform offline spraak-naar-teksttool met Whisper of Parakeet, met globale sneltoetsen en klembordplakken.
- [Buzz](https://github.com/chidiwilliams/buzz) — Cross-platform desktop-GUI voor offline Whisper-transcriptie en -vertaling met GPU-acceleratie en live microfoon.
- [Vibe](https://github.com/thewh1teagle/vibe) — Cross-platform desktop-app voor offline audio- en videotranscriptie met Whisper, met GPU-acceleratie.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Local-first app-toolkit met Markdown/SQLite-opslag, Yjs CRDT-synchronisatie en een desktop spraak-naar-tekst-hulpprogramma.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux-native spraak-naar-tekst met lokale Whisper en ONNX-modellen, cloud-API's, Waybar-integratie en visualizer.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Desktop-dicteerapp die Whisper lokaal of via API gebruikt, geactiveerd door globale sneltoets om in het actieve venster te typen.
- [Chirp](https://github.com/Whamp/chirp-stt) — Windows CPU-only dicteerapp met ParakeetV3, met sneltoetsschakelaar, klembordplakken en woordoverschrijvingen.
- [Dabri](https://github.com/AshBuk/dabri) — Linux offline STT-app met whisper.cpp in daemon-, CLI- en WebSocket-modi voor X11/Wayland-desktops.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux en Sailfish OS offline notitie-app met lokale STT, TTS en vertaling met meerdere engines.
- [voxd](https://github.com/jakovius/voxd) — Linux desktop-spraakdictee met whisper.cpp voor offline ASR met ydotool-typen en AI-nabewerking.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linux offline spraakdictee via Whisper, Parakeet of Canary ONNX, met X11/Wayland-ondersteuning en LLM-polish.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windows spraakdictee-assistent met Caps Lock-sneltoets, met multi-provider STT en optionele LLM-verfijning.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Cross-platform offline dicteerapp met distil-whisper, sneltoetsbesturing en optionele lokale LLM-assistent.
- [TalkType](https://github.com/lmacan1/talktype) — Cross-platform push-to-talk spraakdictee met faster-whisper, met globale sneltoetsen en slim plakken.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Offline meertalige dicteerapp met Faster-Whisper, geactiveerd door sneltoets om in het actieve veld te transcriberen.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — NixOS/Wayland lokale spraakdictee met whisper.cpp met GTK4-feedback en ondersteuning voor 99 talen.
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux Wayland spraakdictee-app met STT, grammaticacorrectie via LanguageTool en ydotool-tekstinvoer.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Lokale AI desktop-agent die spraakdictee, LLM-chat, afbeeldingsgeneratie en spraakgestuurde automatisering combineert.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows desktop spraak-naar-tekst met faster-whisper met toetsenbordsimulatie, VAD, PTT en interpunctie.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Whisper spraakdictee voor KDE Wayland met achtergrond-daemon, systemd-service en klembordplakken.

### Native macOS-dicteer

Native macOS-dicteerapps gebouwd met Swift en WhisperKit, met ondersteuning voor globale sneltoetsen, menubalk en Neural Engine-acceleratie.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Een macOS-spraaktranscriptie-app met Whisper- en Parakeet-engines, globale sneltoetsen en batchverwerking.
- [Pindrop](https://github.com/watzon/pindrop) — Native macOS menubalk-dicteerapp met WhisperKit voor offline STT, met sneltoetsen en optionele AI-schoonmaak.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Offline meertalige dicteertool met Whisper, geactiveerd door sneltoets om in elk invoerveld te transcriberen.
- [FnKey](https://github.com/evoleinik/fnkey) — Een macOS menubalk-app die spraak transcript via Deepgram Nova-3 terwijl Fn wordt ingedrukt en het resultaat plakt.
- [hush](https://github.com/djmunro/hush) — Een macOS push-to-talk dicteerapp met lokale Whisper/Parakeet ONNX en automatisch plakken via sneltoets.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Een macOS menubalk-dicteerapp met offline Whisper met Metal GPU-acceleratie en cursor-tekstinjectie.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS menubalk-app neemt op bij loslaten van Globe/Fn, transcribeert via faster-whisper en plakt bij de cursor.

### AI-spraakschoonmaak / LLM-nabewerking

Dicteertools die lokale of cloud-LLM's gebruiken om spraakherkenningsuitvoer te polijsten, op te maken, samen te vatten en te herstijlen tot schone, formele tekst.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Een macOS-dicteerapp met on-device en cloud-STT, globale sneltoetsen, AI-workflows, plugin, REST API en CLI.
- [Amical](https://github.com/amicalhq/amical) — Local-first AI-dicteerapp met Whisper voor offline transcriptie en Ollama voor slimme notitieverwerking.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Offline spraakdictee-tool voor macOS/Windows met Whisper, met globale sneltoetsen en optionele AI-verbetering.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Local-first spraakassistent voor macOS en Linux met push-to-talk, transcriptie en plugin-extractie.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Een macOS push-to-talk dicteerapp met Whisper en LLM-schoonmaak, die gepolijste tekst plakt via Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Lokaal spraakdictee met Whisper en LLM-polish, push-to-talk, woordenboek en client-server-opdeling.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Lokaal spraakdictee en vergaderingsrecorder met faster-whisper, LLM-samenvattingen en dual-track audiorecord.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Native macOS spraak-naar-tekst-app met lokale whisper.cpp-modellen, met globale snelkoppelingen en contextbewuste modi.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Een macOS-dicteerapp met on-device spraakherkenning en optionele AI-nabewerking voor opmaak.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Desktop spraaktranscriptie-app met sneltoetsen, AI-assistent, vergaderingsdiarisatie en semantisch zoeken.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Een macOS menubalk-app voor offline spraak-naar-tekst en vergaderingssamenvattingen met Whisper en Qwen op Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Cross-platform Tauri spraakdictee-app met lokale Whisper of Groq, AI-schoonmaak, woordenlijst en spraakassistent.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Cross-platform spraakdictee-assistent met LLM-opmaak, met ondersteuning voor lokale Whisper, Ollama of cloud-API's.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Cross-platform Tauri-app voor AI-spraakdictee, tekst herschrijven en spraak-Q&A met globale sneltoetsen.
- [Aria](https://github.com/Xingxun7777/Aria) — Windows AI-spraakinvoer met offline Qwen3-ASR met OCR-context, hotword-correctie en spraakcommando's.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windows spraakdictee met whisper.cpp, Groq of llama.cpp, meerdere stijlen, automatisch plakken in actief venster.
- [localflow](https://github.com/sidharth-n/localflow) — Lokale cross-platform spraakdictee met Moonshine STT, Qwen3-4B-polish, push-to-talk en skip-gate.
- [yammer](https://github.com/andynu/yammer) — Linux lokaal spraak-naar-tekst met Whisper en LLM-schoonmaak, plus Tauri-overlay-UI en xdotool-invoerinjectie.

### Lokale/offline STT-engines en toolkits

Offline ASR-engines en spraak-toolkits voor app-integratie: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech en SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — High-performance C/C++ port van OpenAI Whisper met CPU/GPU-inferentie, quantisatie en cross-platform ondersteuning.
- [FunASR](https://github.com/modelscope/FunASR) — Industriële ASR-toolkit met Paraformer, SenseVoice, VAD, diarisatie, streaming en OpenAI-compatibele API.
- [vosk-api](https://github.com/alphacep/vosk-api) — Offline spraakherkenningstoolkit met kleine CPU-only modellen voor 20+ talen en multitalige bindings.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Offline spraak-toolkit met next-gen Kaldi en ONNX Runtime voor STT, TTS, spreker-ID, VAD en meer.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Uitgebreide spraak-toolkit met ASR, TTS, voiceprint, diarisatie, vertaling en streamingdiensten.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Spraakmodel met ASR voor 50+ talen, emotie, audio-evenementen en snelle niet-autoregressieve inferentie.

### Systeemniveau spraakinvoer / IME

Spraakinvoeroplossingen geïntegreerd op systeemniveau, inclusief invoermethoden, IBus-/Fcitx-extensies, Android-IME en iOS-toetsenborden.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android-IME en spraakinvoerservice met Whisper voor offline spraakherkenning en Engelse vertaling.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Offline Linux spraakdictee-app met whisper.cpp, Whisper en VOSK-engines, Vulkan GPU en GTK GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — GNOME Shell-extensie voor offline spraakinvoer via whisper.cpp met sneltoetstrigger, met ondersteuning voor X11 en Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Android offline spraakherkenningsservice met Vosk met standaard RecognitionService API-ondersteuning.
- [Dictus](https://github.com/getdictus/dictus-ios) — Open-source iOS-toetsenbord voor on-device spraakdictee met WhisperKit en CoreML, werkt in elke app.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linux IBus spraak-naar-tekst-invoermethode met streaming STT, optionele Whisper-verfijning en GPU-acceleratie.

### Chinese spraakinvoer / IME

Projecten geoptimaliseerd voor Chinese spraakherkenning en -invoer, inclusief op FunASR, Paraformer en SenseVoice gebaseerde Chinese IME's en toetsenborden.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Offline Linux Chinese spraakinvoer met FunASR Paraformer, IBus/Fcitx5, PTT-sneltoets en zinnenpolish.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Cross-platform offline spraakinvoermethode met FunASR, met hotword-correctie, automatisch plakken en GUI/CLI-modi.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android spraakinvoertoetsenbord met 11 ASR-engines, LLM-nabewerking, zwevende bal en Material3-UI.

### Browser en web spraakinvoer

Browsergebaseerde spraakinvoer via extensies, WebAssembly-wrappers of web-UI's, die doorgaans een lokale of cloud-STT-backend vereisen.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI voor ondertitels uit bestanden, YouTube of microfoon, met VAD, BGM-scheiding en diarisatie.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Browserextensie voor realtime offline spraak-naar-tekst via Vosk, met Arabische en Engelse spraakcommando's.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Browsergebaseerde offline spraakherkenningsbibliotheek die Vosk verpakt als WebAssembly draaiend in een WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Browserextensie en lokale Whisper-server voor offline spraak-naar-tekst in Firefox en Chrome via Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Chrome-extensie die spraak opneemt via sneltoets, transcribeert met OpenAI Whisper API en tekst automatisch plakt.
- [voico](https://github.com/Kirera-Wainaina/voico) — Chrome-extensie voor spraak-naar-tekst-invoer in webvelden, met een Node.js-backend met Google en OpenAI STT.

### Mobiele spraakinvoer (non-IME)

Zelfstandige spraaktranscriptie-apps op Android of iOS, in plaats van invoermethodetoetsenborden.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Privé on-device spraakherkenningstoetsenbord voor Android met Whisper via whisper.cpp en Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Open-source iOS-app voor offline spraaktranscriptie met Whisper.cpp, met opname en audio-export.
- [seamless](https://github.com/woheller69/seamless) — Android offline spraak-naar-tekst-vertaalapp met Meta Seamless M4T Lite voor 5 talen met TTS-uitvoer.

### Lichte scripts, CLI en spraakbesturing

Lichte scripts, CLI-tools, tray-triggers of hulpprogramma's geschikt voor ontwikkelaarsintegratie of als aanvulling op bestaande toolchains.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linux offline spraak-naar-teksttool met Vosk die toetsenbordinvoer in elke applicatie simuleert.
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash-script voor offline spraakdictee via Whisper voor TTY, X11, Wayland en WSL met optionele LLM-bewerking.
- [hns](https://github.com/primaprashant/hns) — CLI-tool voor lokale microfoon spraak-naar-tekst met faster-whisper, met klembordkopiëren en stdout-piping.
- [Elograf](https://github.com/papoteur-mga/elograf) — PyQt6 GUI-manager voor nerd-dictation met systeemvak, Vosk-modellen, invoersimulatie en KDE-sneltoetsen.
- [Osprey](https://github.com/osprey-voice/osprey) — Command-gebaseerde spraakbesturings- en typtool met Kaldi en Dragonfly voor volledig lokale spraakherkenning.

### Overige

Projecten die nog niet aan een categorie zijn toegewezen.

- [VoxType](https://github.com/peteonrails/voxtype) — Linux en Wayland push-to-talk spraak-naar-tekst met zeven lokale ASR-engines, GPU-ondersteuning en vergaderingsmodus.

## Open source versus benchmarks

| Project | Prijs | Open Source | Uitbreidbaar | Offline | Chinees |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Gratis (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Gratis (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: gratis 8K wk/wk; Pro $12/mo jaarlijks ($30/mo maandelijks) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Persoonlijk €25 eenmalig (BYOK Groq); Pro €5/mo gehost | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Gratis (lokaal/BYOK); Pro ¥29/mo of ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Hoe kiezen

- **Gepolijste cross-platform desktop-app** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 sterren, Whisper/Parakeet offline.
- **Minimale Linux offline, scriptbaar** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simuleert toetsenbordinvoer in elke app.
- **STT inbedden in je eigen app** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, embeddable.
- **Chinese-eerste invoer** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; offline Linux Chinese spraakinvoer met FunASR Paraformer, IBus/Fcitx5, PTT-sneltoets en zinnenpolish.
- **Zelf een transcriptie-API/server hosten** → [FunASR](https://github.com/modelscope/FunASR) — industriële ASR-toolkit met Paraformer, SenseVoice, VAD, diarisatie, streaming en OpenAI-compatibele API.

## Bijdragen

Bijdragen zijn welkom — zie [CONTRIBUTING.md](CONTRIBUTING.md). Projecten moeten volledig open source, uitbreidbaar en lichtgewicht zijn; volg de stijlgids voor beschrijvingen (in het Engels, één regel, feitelijk, geen marketingflauwekul).

## Star-Geschiedenis

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

Star-groei over tijd voor de meest-gesternde projecten in deze lijst. De repository zelf is privé tijdens het reviewen; zijn eigen star-geschiedenis wordt hier toegevoegd zodra deze publiek wordt.

## Licentie

[MIT](LICENSE).

# Awesome Voice Input

> 오픈 소스 음성 입력 / 받아쓰기 소프트웨어의 선별된 목록 — 완전히 개방적이고, 확장 가능하며, 가벼운. Typeless, Lazytype, Shandianshuo(闪电说)와 비교 기준으로 삼았으며, 모두 클로즈드 소스입니다.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*이 목록이 유용하다면 ⭐를 눌러주세요 — 더 많은 사람이 발견하는 데 도움이 됩니다.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · **한국어** · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## 목차

- [벤치마크 (클로즈드 소스)](#벤치마크-클로즈드-소스)
- [왜 이 목록인가](#왜-이-목록인가)
- [포함 기준](#포함-기준)
- [추천 프로젝트](#추천-프로젝트)
- [모든 프로젝트](#모든-프로젝트)
- [분류 목록](#분류-목록)
  - [크로스 플랫폼 데스크톱 실시간 받아쓰기](#크로스-플랫폼-데스크톱-실시간-받아쓰기)
  - [macOS 전용 받아쓰기](#macos-전용-받아쓰기)
  - [AI 음성 정리 / LLM 후처리](#ai-음성-정리-llm-후처리)
  - [로컬/오프라인 STT 엔진 및 툴킷](#로컬오프라인-stt-엔진-및-툴킷)
  - [시스템 수준 음성 입력 / IME](#시스템-수준-음성-입력-ime)
  - [중국어 음성 입력 / IME](#중국어-음성-입력-ime)
  - [브라우저 및 웹 음성 입력](#브라우저-및-웹-음성-입력)
  - [모바일 음성 입력 (IME 아님)](#모바일-음성-입력-ime-아님)
  - [경량 스크립트, CLI 및 음성 제어](#경량-스크립트-cli-및-음성-제어)
  - [기타](#기타)
- [오픈 소스 대 벤치마크](#오픈-소스-대-벤치마크)
- [선택 방법](#선택-방법)
- [기여 贡献](#기여-贡献)
- [Star History](#star-history)
- [라이선스](#라이선스)

## 벤치마크 (클로즈드 소스)

| 제품 | 가격 | 플랫폼 | 모델/엔진 | 오픈 소스 |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## 왜 이 목록인가

Typeless, Lazytype, Shandianshuo(闪电说)는 강력하지만 클로즈드 소스입니다. 이 목록은 세 가지 기준을 충족하는 오픈 소스 대안을 모응니다: 코드가 완전히 공개되어 있고, 도구를 확장할 수 있으며, 개인 컴퓨터에서 실행할 수 있을 만큼 가벼운. 현재 **9개 카테고리의 75개 프로젝트**를 다루며, 모두 완전한 오픈 소스임을 검증하였습니다.

## 포함 기준

- ✅ **완전한 오픈 소스** — 모든 코드가 공개 포지(GitHub, GitLab, Codeberg)에 있음.
- 🔌 **확장 가능** — 원하는 기능, 모델, 통합을 추가할 수 있음.
- ⚡ **경량** — 불필요한 부풀림 최소화, 빠른 시작, 작은 공간.

## 추천 프로젝트

🏆 **[Handy](https://github.com/cjpais/Handy)** — Whisper 또는 Parakeet을 사용하는 크로스 플랫폼 오프라인 음성-텍스트 도구, 전역 핫키와 클립보드 붙여넣기 지원. *커뮤니티 플래그십 — 25,281개 스타, 가장 다듬어진 솔루션.*

**Fit-5 선정** (세 가지 기준 모두 충족):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — OpenAI Whisper의 고성능 C/C++ 포트, CPU/GPU 추론, 양자화, 크로스 플랫폼 지원.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Vosk를 사용하는 Linux 오프라인 음성-텍스트 도구, 모든 애플리케이션에 키보드 입력을 시뮬레이션.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux 및 Wayland용 푸시-토-토크 음성-텍스트, 7개 로컬 ASR 엔진, GPU 지원, 회의 모드.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — TTY, X11, Wayland, WSL용 오프라인 음성 입력 Bash 스크립트, 선택적 LLM 편집.

## 모든 프로젝트

| 이름 | ⭐ 스타 | 라이선스 | 언어 | 적합 | 오픈 | 확장 | 경량 | 중국어 |
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

## 분류 목록

### 크로스 플랫폼 데스크톱 실시간 받아쓰기

Linux, Windows, 크로스 플랫폼용 Whisper 기반 데스크톱 받아쓰기 앱, 푸시-토-토크, 로컬 전사, 자동 입력 기능 제공.

- [Handy](https://github.com/cjpais/Handy) — Whisper 또는 Parakeet을 사용하는 크로스 플랫폼 오프라인 음성-텍스트 도구, 전역 핫키와 클립보드 붙여넣기 지원.
- [Buzz](https://github.com/chidiwilliams/buzz) — 오프라인 Whisper 전사 및 번역을 위한 크로스 플랫폼 데스크톱 GUI, GPU 가속, 실시간 마이크.
- [Vibe](https://github.com/thewh1teagle/vibe) — Whisper를 사용한 오프라인 오디오 및 비디오 전사 크로스 플랫폼 데스크톱 앱, GPU 가속.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Markdown/SQLite 저장소, Yjs CRDT 동기화, 데스크톱 음성-텍스트 유틸리티를 갖춘 로컬 우선 앱 툴킷.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — 로컬 Whisper 및 ONNX 모델, 클라우드 API, Waybar 통합, 시각화를 갖춘 Linux 네이티브 음성-텍스트.
- [whisper-writer](https://github.com/savbell/whisper-writer) — 로컬 또는 API를 통해 Whisper를 사용하는 데스크톱 받아쓰기 앱, 전역 핫키로 활성 창에 입력.
- [Chirp](https://github.com/Whamp/chirp-stt) — ParakeetV3를 사용하는 Windows CPU 전용 받아쓰기 앱, 핫키 전환, 클립보드 붙여넣기, 단어 재정의.
- [Dabri](https://github.com/AshBuk/dabri) — X11/Wayland 데스크톱용 whisper.cpp 기반 Linux 오프라인 STT 앱, 데몬, CLI, WebSocket 모드.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — 여러 엔진을 사용한 로컬 STT, TTS, 번역 기능을 갖춘 Linux 및 Sailfish OS 오프라인 메모 앱.
- [voxd](https://github.com/jakovius/voxd) — ydotool 입력과 AI 후처리를 갖춘 whisper.cpp 기반 Linux 데스크톱 음성 받아쓰기.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Whisper, Parakeet, Canary ONNX를 통한 Linux 오프라인 음성 입력, X11/Wayland 지원 및 LLM 다듬기.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Caps Lock 핫키, 다중 공급자 STT, 선택적 LLM 정제를 사용하는 Windows 음성 입력 보조 도구.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — distil-whisper, 핫키 제어, 선택적 로컬 LLM 어시스턴트를 갖춘 크로스 플랫폼 오프라인 받아쓰기 앱.
- [TalkType](https://github.com/lmacan1/talktype) — faster-whisper를 사용하는 크로스 플랫폼 푸시-토-토크 음성 입력, 전역 핫키 및 스마트 붙여넣기.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Faster-Whisper를 사용하는 오프라인 다국어 받아쓰기 앱, 핫키로 활성 필드에 전사.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — GTK4 피드백과 99개 언어 지원을 갖춘 NixOS/Wayland 로컬 음성 받아쓰기, whisper.cpp 사용.
- [freespeak](https://github.com/Zetaphor/freespeak) — STT, LanguageTool을 통한 문법 교정, ydotool 텍스트 입력을 갖춘 Linux Wayland 음성 받아쓰기 앱.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — 음성 받아쓰기, LLM 챗, 이미지 생성, 음성 기반 자동화를 결합한 로컬 AI 데스크톱 에이전트.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — faster-whisper를 사용하는 Windows 데스크톱 음성-텍스트, 키보드 시뮬레이션, VAD, PTT, 문장부호.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — 백그라운드 데몬, systemd 서비스, 클립보드 붙여넣기를 갖춘 KDE Wayland용 Whisper 음성 받아쓰기.

### macOS 전용 받아쓰기

Swift 및 WhisperKit으로 빌드된 macOS 전용 받아쓰기 앱, 전역 핫키, 메뉴 바, Neural Engine 가속 지원.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Whisper 및 Parakeet 엔진, 전역 핫키, 배치 처리를 갖춘 macOS 음성 전사 앱.
- [Pindrop](https://github.com/watzon/pindrop) — 오프라인 STT를 위해 WhisperKit을 사용하는 macOS 네이티브 메뉴 바 받아쓰기 앱, 핫키 및 선택적 AI 정리.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — 핫키로 트리거되어 모든 입력 필드에 전사되는 오프라인 다국어 받아쓰기 도구, Whisper 사용.
- [FnKey](https://github.com/evoleinik/fnkey) — Fn을 누르는 동안 Deepgram Nova-3을 통해 음성을 전사하고 결과를 붙여넣는 macOS 메뉴 바 앱.
- [hush](https://github.com/djmunro/hush) — 로컬 Whisper/Parakeet ONNX를 사용하고 핫키로 자동 붙여넣기하는 macOS 푸시-토-토크 받아쓰기 앱.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — 오프라인 Whisper를 사용하는 macOS 메뉴 바 받아쓰기 앱, Metal GPU 가속 및 커서 텍스트 삽입.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS 메뉴 바 앱은 Globe/Fn 해제 시 녹음하고 faster-whisper로 전사하여 커서에 붙여넣기.

### AI 음성 정리 / LLM 후처리

로컬 또는 클라우드 LLM을 사용하여 음성 인식 결과를 깔끔하고 공식적인 텍스트로 다듬거나, 형식화하거나, 요약하거나, 스타일을 변경하는 받아쓰기 도구.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — 온디바이스 및 클라우드 STT, 전역 핫키, AI 워크플로우, 플러그인, REST API, CLI를 갖춘 macOS 받아쓰기 앱.
- [Amical](https://github.com/amicalhq/amical) — 오프라인 전사에 Whisper, 스마트 메모 처리에 Ollama를 사용하는 로컬 우선 AI 받아쓰기 앱.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — macOS/Windows용 오프라인 음성 받아쓰기 도구, Whisper 사용, 전역 핫키 및 선택적 AI 향상.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — macOS 및 Linux용 로컬 우선 음성 어시스턴트, 푸시-토-토크, 전사, 플러그인 추출.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Whisper 및 LLM 정리를 사용하는 macOS 푸시-토-토크 받아쓰기 앱, Cmd-V로 깔끔한 텍스트 붙여넣기.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Whisper 및 LLM 다듬기, 푸시-토-토크, 사전, 클라이언트-서버 분할을 갖춘 로컬 음성 받아쓰기.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — faster-whisper, LLM 요약, 듀얼 트랙 오디오 캡처를 갖춘 로컬 음성 받아쓰기 및 회의 녹음 도구.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — 로컬 whisper.cpp 모델, 전역 단축키, 맥락 인식 모드를 갖춘 macOS 네이티브 음성-텍스트 앱.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — 온디바이스 음성 인식과 형식화를 위한 선택적 AI 후처리를 갖춘 macOS 받아쓰기 앱.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — 핫키, AI 어시스턴트, 회의 화자 분리, 의미 검색을 갖춘 데스크톱 음성 전사 앱.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — 오프라인 음성-텍스트와 Whisper, Apple Silicon에서의 Qwen을 사용한 회의 요약을 위한 macOS 메뉴 바 앱.
- [Voquill](https://github.com/voquill/voquill) — 로컬 Whisper 또는 Groq, AI 정리, 용어집, 음성 어시스턴트를 갖춘 크로스 플랫폼 Tauri 음성 입력 앱.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — LLM 형식화, 로컬 Whisper, Ollama 또는 클라우드 API를 지원하는 크로스 플랫폼 음성 받아쓰기 어시스턴트.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — AI 음성 입력, 텍스트 재작성, 음성 Q&A, 전역 핫키를 갖춘 크로스 플랫폼 Tauri 앱.
- [Aria](https://github.com/Xingxun7777/Aria) — 오프라인 Qwen3-ASR, OCR 맥락, 핫워드 수정, 음성 명령을 사용하는 Windows AI 음성 입력.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — whisper.cpp, Groq 또는 llama.cpp, 다중 스타일, 활성 창 자동 붙여넣기를 사용하는 Windows 음성 받아쓰기.
- [localflow](https://github.com/sidharth-n/localflow) — Moonshine STT, Qwen3-4B 다듬기, 푸시-토-토크, 스킵 게이트를 사용하는 로컬 크로스 플랫폼 음성 받아쓰기.
- [yammer](https://github.com/andynu/yammer) — Whisper 및 LLM 정리, Tauri 오버레이 UI, xdotool 입력 삽입을 갖춘 Linux 로컬 음성-텍스트.

### 로컬/오프라인 STT 엔진 및 툴킷

앱 통합용 오프라인 ASR 엔진 및 음성 툴킷: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech, SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — OpenAI Whisper의 고성능 C/C++ 포트, CPU/GPU 추론, 양자화, 크로스 플랫폼 지원.
- [FunASR](https://github.com/modelscope/FunASR) — Paraformer, SenseVoice, VAD, 화자 분리, 스트리밍, OpenAI 호환 API를 갖춘 산업용 ASR 툴킷.
- [vosk-api](https://github.com/alphacep/vosk-api) — 20개 이상 언어용 소형 CPU 전용 모델과 다중 언어 바인딩을 갖춘 오프라인 음성 인식 툴킷.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — 차세대 Kaldi와 ONNX Runtime을 사용하는 STT, TTS, 화자 식별, VAD 등을 위한 오프라인 음성 툴킷.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — ASR, TTS, 음성 지문, 화자 분리, 번역, 스트리밍 서비스를 갖춘 종합 음성 툴킷.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — 50개 이상 언어의 ASR, 감정, 오디오 이벤트, 빠른 비자기 회귀 추론을 지원하는 음성 모델.

### 시스템 수준 음성 입력 / IME

입력법, IBus/Fcitx 확장, Android IME, iOS 키보드 등 시스템 수준에 통합된 음성 입력 솔루션.

- [Whisper IME](https://github.com/woheller69/whisperIME) — 오프라인 음성 인식 및 영어 번역을 위해 Whisper를 사용하는 Android IME 및 음성 입력 서비스.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — whisper.cpp, Whisper, VOSK 엔진, Vulkan GPU, GTK GUI를 갖춘 Linux 오프라인 음성 받아쓰기 앱.
- [blurt](https://github.com/QuantiusBenignus/blurt) — whisper.cpp를 통한 오프라인 음성 입력을 위한 GNOME Shell 확장, 핫키 트리거, X11 및 Wayland 지원.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — 표준 RecognitionService API를 지원하는 Vosk 기반 Android 오프라인 음성 인식 서비스.
- [Dictus](https://github.com/getdictus/dictus-ios) — WhisperKit 및 CoreML을 사용한 온디바이스 음성 받아쓰기 iOS 키보드, 모든 앱에서 작동.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — 스트리밍 STT, 선택적 Whisper 정제, GPU 가속을 갖춘 Linux IBus 음성-텍스트 입력법.

### 중국어 음성 입력 / IME

FunASR, Paraformer, SenseVoice 기반 중국어 IME 및 키보드를 포함한 중국어 음성 인식 및 입력 최적화 프로젝트.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — FunASR Paraformer, IBus/Fcitx5, PTT 핫키, 문장 다듬기를 사용하는 Linux 오프라인 중국어 음성 입력.
- [voice-input-method](https://github.com/pofice/voice-input-method) — FunASR을 사용하는 크로스 플랫폼 오프라인 음성 입력법, 핫워드 수정, 자동 붙여넣기, GUI/CLI 모드.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — 11개 ASR 엔진, LLM 후처리, 플로팅 볼, Material3 UI를 갖춘 Android 음성 입력 키보드.

### 브라우저 및 웹 음성 입력

확장 프로그램, WebAssembly 래퍼, Web UI를 통한 브라우저 기반 음성 입력, 일반적으로 로컬 또는 클라우드 STT 백엔드 필요.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — 파일, YouTube, 마이크에서 자막을 생성하는 Gradio Whisper WebUI, VAD, BGM 분리, 화자 분리.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Vosk를 통한 실시간 오프라인 음성-텍스트 브라우저 확장, 아랍어 및 영어 음성 명령.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — WebWorker에서 WebAssembly로 실행되는 Vosk를 패키징한 브라우저 기반 오프라인 음성 인식 라이브러리.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Firefox 및 Chrome에서 Alt+A를 통한 오프라인 음성-텍스트를 위한 브라우저 확장 및 로컬 Whisper 서버.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — 핫키로 음성을 녹음하고 OpenAI Whisper API로 전사한 후 텍스트를 자동으로 붙여넣는 Chrome 확장.
- [voico](https://github.com/Kirera-Wainaina/voico) — 웹 필드에 음성-텍스트 입력을 제공하는 Chrome 확장, Google 및 OpenAI STT를 사용하는 Node.js 백엔드.

### 모바일 음성 입력 (IME 아님)

입력법 키보드가 아닌 Android 또는 iOS의 독립형 음성 전사 앱.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — whisper.cpp를 통한 Whisper와 Silero VAD를 사용하는 Android용 온디바이스 음성 인식 키보드.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Whisper.cpp를 사용한 오프라인 음성 전사 iOS 앱, 녹음 및 오디오 내보기.
- [seamless](https://github.com/woheller69/seamless) — Meta Seamless M4T Lite를 사용한 5개 언어 TTS 출력 지원 Android 오프라인 음성-텍스트 번역 앱.

### 경량 스크립트, CLI 및 음성 제어

개발자 통합용 또는 기존 툴체인 보완용으로 적합한 경량 스크립트, CLI 도구, 트레이 트리거, 유틸리티.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Vosk를 사용하는 Linux 오프라인 음성-텍스트 도구, 모든 애플리케이션에 키보드 입력을 시뮬레이션.
- [voice_typing](https://github.com/themanyone/voice_typing) — TTY, X11, Wayland, WSL용 오프라인 음성 입력 Bash 스크립트, 선택적 LLM 편집.
- [hns](https://github.com/primaprashant/hns) — faster-whisper를 사용한 로컬 마이크 음성-텍스트 CLI 도구, 클립보드 복사 및 stdout 파이프.
- [Elograf](https://github.com/papoteur-mga/elograf) — 시스템 트레이, Vosk 모델, 입력 시뮬레이션, KDE 핫키를 갖춘 nerd-dictation용 PyQt6 GUI 관리자.
- [Osprey](https://github.com/osprey-voice/osprey) — Kaldi 및 Dragonfly를 사용한 명령 기반 음성 제어 및 입력 도구, 완전한 로컬 음성 인식.

### 기타

아직 카테고리에 할당되지 않은 프로젝트.

- [VoxType](https://github.com/peteonrails/voxtype) — Linux 및 Wayland 푸시-토-토크 음성-텍스트, 7개 로컬 ASR 엔진, GPU 지원, 회의 모드.

## 오픈 소스 대 벤치마크

| 프로젝트 | 가격 | 오픈 소스 | 확장 가능 | 오프라인 | 중국어 |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Free (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Free (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## 선택 방법

- **다듬어진 크로스 플랫폼 데스크톱 앱** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281개 스타, Whisper/Parakeet 오프라인.
- **미니멀한 Linux 오프라인, 스크립트 가능** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, 모든 앱에 키보드 입력 시뮬레이션.
- **자신의 앱에 STT 임베드** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, 임베드 가능.
- **중국어 중심 입력** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; FunASR Paraformer, IBus/Fcitx5, PTT 핫키, 문장 다듬기를 사용하는 Linux 오프라인 중국어 음성 입력.
- **전사 API/서버 자체 호스팅** → [FunASR](https://github.com/modelscope/FunASR) — Paraformer, SenseVoice, VAD, 화자 분리, 스트리밍, OpenAI 호환 API를 갖춘 산업용 ASR 툴킷.

## 기여 贡献

기여는 환영합니다 — 자세한 내용은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참조하세요. 프로젝트는 완전한 오픈 소스, 확장 가능, 경량이어야 합니다; 설명 스타일 가이드를 따르세요(영어, 한 줄, 사실적, 마케팅 과장 금지).

참여를 환영합니다 — 자세한 내용은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참조하세요. 프로젝트는 완전한 오픈 소스, 확장 가능, 경량이어야 하며; 설명 스타일 가이드(영어, 한 줄, 사실 기반, 마케팅 과장 배제)를 따라주세요.

## Star History

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

이 목록에서 가장 스타가 많은 프로젝트의 시간별 성장. 리포지토리는 검토 중에는 비공개이며, 공개 후 자체 Star History가 여기에 추가될 예정입니다.

## 라이선스

[MIT](LICENSE).

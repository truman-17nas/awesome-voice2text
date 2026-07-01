# Awesome Voice Input

> 這是一份精選的開源語音輸入 / 語音聽打軟體清單——完全開放、可擴充，並且輕量化。以 Typeless、Lazytype 與 閃電說（Shandianshuo）這三款閉源軟體作為對照。

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*如果這份清單對你有幫助，請幫我們 ⭐ 這個 repo，讓更多人找到它。*

[English](README.md) · [简体中文](README.zh-CN.md) · **繁體中文** · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## 目錄

- [評測對照（閉源）](#評測對照閉源)
- [為什麼是這份清單](#為什麼是這份清單)
- [收錄標準](#收錄標準)
- [精選推薦](#精選推薦)
- [全部專案](#全部專案)
- [分類清單](#分類清單)
  - [跨平台桌面即時語音輸入](#跨平台桌面即時語音輸入)
  - [原生 macOS 語音輸入](#原生-macos-語音輸入)
  - [AI 語音整理 / LLM 後處理](#ai-語音整理-llm-後處理)
  - [本地/離線 STT 引擎與工具包](#本地離線-stt-引擎與工具包)
  - [系統層級語音輸入 / IME](#系統層級語音輸入-ime)
  - [中文語音輸入 / IME](#中文語音輸入-ime)
  - [瀏覽器與網頁語音輸入](#瀏覽器與網頁語音輸入)
  - [行動裝置語音輸入（非 IME）](#行動裝置語音輸入非-ime)
  - [輕量腳本、CLI 與語音控制](#輕量腳本cli-與語音控制)
  - [其他](#其他)
- [開源專案與對照組](#開源專案與對照組)
- [如何選擇](#如何選擇)
- [貢獻](#貢獻)
- [Star 歷史](#star-歷史)
- [授權條款](#授權條款)

## 評測對照（閉源）

| 產品 | 定價 | 平台 | 模型/引擎 | 開源 |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## 為什麼是這份清單

Typeless、Lazytype 與 閃電說（Shandianshuo）功能強大，但皆為閉源。本清單收集符合三項標準的開源替代方案：程式碼完全公開、工具可擴充，以及輕量到足以在個人電腦上執行。目前涵蓋 **9 個分類中的 75 個專案**，且皆已確認為完全開源。

## 收錄標準

- ✅ **完全開源**——所有程式碼皆託管在公開平台（GitHub、GitLab、Codeberg）。
- 🔌 **可擴充**——你可以新增想要的功能、模型或整合。
- ⚡ **輕量化**——最少的累贅、快速啟動、占用空間小。

## 精選推薦

🏆 **[Handy](https://github.com/cjpais/Handy)** — 跨平台離線語音轉文字工具，使用 Whisper 或 Parakeet，具備全域快捷鍵與剪貼簿貼上。*社群旗艦——25,281 顆星，最精緻的選擇。*

**滿分 5 分精選**（符合全部三項標準）：
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — 高效能的 OpenAI Whisper C/C++ 移植版本，支援 CPU/GPU 推論、量化與跨平台。
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linux 離線語音轉文字工具，使用 Vosk，可模擬鍵盤輸入到任何應用程式。
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux 與 Wayland 即按即說語音轉文字，提供七種本地 ASR 引擎、GPU 支援與會議模式。
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash 腳本，透過 Whisper 在 TTY、X11、Wayland 與 WSL 上進行離線語音輸入，可選 LLM 編輯。

## 全部專案

| 名稱 | ⭐ 星星數 | 授權 | 語言 | 適配 | 開源 | 可擴充 | 輕量 | 中文 |
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
| [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) | 11 | MIT | Python | 3 | ✅ | ⚠️ | ⚠️ | ⚠️ |
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

## 分類清單

### 跨平台桌面即時語音輸入

以 Whisper 為基礎的桌面語音輸入應用程式，適用於 Linux、Windows 或跨平台，具備即按即說、本地轉錄與自動輸入功能。

- [Handy](https://github.com/cjpais/Handy) — 跨平台離線語音轉文字工具，使用 Whisper 或 Parakeet，具備全域快捷鍵與剪貼簿貼上。
- [Buzz](https://github.com/chidiwilliams/buzz) — 跨平台桌面 GUI，用於離線 Whisper 轉錄與翻譯，支援 GPU 加速與即時麥克風。
- [Vibe](https://github.com/thewh1teagle/vibe) — 跨平台桌面應用程式，使用 Whisper 進行離線音訊與影片轉錄，支援 GPU 加速。
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — 本地優先的應用程式工具包，具備 Markdown/SQLite 儲存、Yjs CRDT 同步，以及桌面語音轉文字工具。
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux 原生語音轉文字，使用本地 Whisper 與 ONNX 模型、雲端 API、Waybar 整合與視覺化工具。
- [whisper-writer](https://github.com/savbell/whisper-writer) — 桌面語音輸入應用程式，可在本地或透過 API 使用 Whisper，透過全域快捷鍵觸發輸入到作用中視窗。
- [Chirp](https://github.com/Whamp/chirp-stt) — 僅使用 CPU 的 Windows 語音輸入應用程式，使用 ParakeetV3，支援快捷鍵切換、剪貼簿貼上與字詞覆寫。
- [Dabri](https://github.com/AshBuk/dabri) — Linux 離線 STT 應用程式，使用 whisper.cpp，具備 daemon、CLI 與 WebSocket 模式，適用於 X11/Wayland 桌面。
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux 與 Sailfish OS 離線筆記應用程式，具備本地 STT、TTS 與多引擎翻譯。
- [voxd](https://github.com/jakovius/voxd) — Linux 桌面語音輸入，使用 whisper.cpp 進行離線 ASR，搭配 ydotool 輸入與 AI 後處理。
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linux 離線語音輸入，透過 Whisper、Parakeet 或 Canary ONNX，支援 X11/Wayland 並可透過 LLM 潤飾。
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windows 語音輸入助手，使用 Caps Lock 快捷鍵，支援多供應商 STT 與選用的 LLM 潤飾。
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — 跨平台離線語音輸入應用程式，使用 distil-whisper，支援快捷鍵控制與選用的本地 LLM 助理。
- [TalkType](https://github.com/lmacan1/talktype) — 跨平台即按即說語音輸入，使用 faster-whisper，具備全域快捷鍵與智慧貼上。
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — 離線多語言語音輸入應用程式，使用 Faster-Whisper，透過快捷鍵觸發並轉錄到作用中欄位。
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — NixOS/Wayland 本地語音輸入，使用 whisper.cpp，具備 GTK4 回饋與 99 種語言支援。
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux Wayland 語音輸入應用程式，具備 STT、LanguageTool 文法校正與 ydotool 文字輸入。
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — 本地 AI 桌面代理，結合語音輸入、LLM 對話、圖片生成與語音驅動自動化。
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows 桌面語音轉文字，使用 faster-whisper，具備鍵盤模擬、VAD、PTT 與標點符號。
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — 適用於 KDE Wayland 的 Whisper 語音輸入，具備背景 daemon、systemd 服務與剪貼簿貼上。

### 原生 macOS 語音輸入

使用 Swift 與 WhisperKit 建構的原生 macOS 語音輸入應用程式，支援全域快捷鍵、選單列與神經引擎加速。

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — macOS 語音轉錄應用程式，具備 Whisper 與 Parakeet 引擎、全域快捷鍵與批次處理。
- [Pindrop](https://github.com/watzon/pindrop) — 原生 macOS 選單列語音輸入應用程式，使用 WhisperKit 進行離線 STT，支援快捷鍵與選用的 AI 清理。
- [whisper-dictation](https://github.com/foges/whisper-dictation) — 離線多語言語音輸入工具，使用 Whisper，透過快捷鍵觸發並轉錄到任何輸入欄位。
- [FnKey](https://github.com/evoleinik/fnkey) — macOS 選單列應用程式，在按住 Fn 時透過 Deepgram Nova-3 轉錄語音並貼上結果。
- [hush](https://github.com/djmunro/hush) — macOS 即按即說語音輸入應用程式，使用本地 Whisper/Parakeet ONNX，透過快捷鍵自動貼上。
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — macOS 選單列語音輸入應用程式，使用離線 Whisper 與 Metal GPU 加速，並將文字插入游標處。
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS 選單列應用程式，在放開 Globe/Fn 時錄音，透過 faster-whisper 轉錄並貼到游標處。

### AI 語音整理 / LLM 後處理

使用本地或雲端 LLM 來潤飾、格式化、摘要與改寫語音辨識輸出，使其成為乾淨、正式文字的語音輸入工具。

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — macOS 語音輸入應用程式，具備裝置端與雲端 STT、全域快捷鍵、AI 工作流程、外掛、REST API 與 CLI。
- [Amical](https://github.com/amicalhq/amical) — 本地優先的 AI 語音輸入應用程式，使用 Whisper 進行離線轉錄，並使用 Ollama 進行智慧筆記處理。
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — 適用於 macOS/Windows 的離線語音輸入工具，使用 Whisper，具備全域快捷鍵與選用的 AI 增強。
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — 本地優先的語音助理，適用於 macOS 與 Linux，具備即按即說、轉錄與外掛擷取。
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — macOS 即按即說語音輸入應用程式，使用 Whisper 與 LLM 清理，透過 Cmd-V 貼上潤飾後的文字。
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — 本地語音輸入，使用 Whisper 與 LLM 潤飾，具備即按即說、字典與用戶端-伺服器分離架構。
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — 本地語音輸入與會議錄音工具，使用 faster-whisper，具備 LLM 摘要與雙軌道音訊錄製。
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — 原生 macOS 語音轉文字應用程式，使用本地 whisper.cpp 模型，具備全域快捷鍵與情境感知模式。
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — macOS 語音輸入應用程式，具備裝置端語音辨識與選用的 AI 後處理格式化。
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — 桌面語音轉錄應用程式，具備快捷鍵、AI 助理、會議說話人分段與語意搜尋。
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — macOS 選單列應用程式，用於離線語音轉文字與會議摘要，在 Apple Silicon 上使用 Whisper 與 Qwen。
- [Voquill](https://github.com/voquill/voquill) — 跨平台 Tauri 語音輸入應用程式，支援本地 Whisper 或 Groq、AI 清理、詞彙表與語音助理。
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — 跨平台語音輸入助理，具備 LLM 格式化，支援本地 Whisper、Ollama 或雲端 API。
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — 跨平台 Tauri 應用程式，用於 AI 語音輸入、文字改寫與語音問答，具備全域快捷鍵。
- [Aria](https://github.com/Xingxun7777/Aria) — Windows AI 語音輸入，使用離線 Qwen3-ASR，具備 OCR 情境、熱詞校正與語音指令。
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windows 語音輸入，使用 whisper.cpp、Groq 或 llama.cpp，具備多種風格與自動貼上到作用中視窗。
- [localflow](https://github.com/sidharth-n/localflow) — 本地跨平台語音輸入，使用 Moonshine STT、Qwen3-4B 潤飾器、即按即說與跳過閘門。
- [yammer](https://github.com/andynu/yammer) — Linux 本地語音轉文字，使用 Whisper 與 LLM 清理，加上 Tauri 覆疊 UI 與 xdotool 輸入注入。

### 本地/離線 STT 引擎與工具包

用於整合到應用程式的離線 ASR 引擎與語音工具包：Whisper、Kaldi、ONNX、Vosk、FunASR、PaddleSpeech 與 SenseVoice。

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — 高效能的 OpenAI Whisper C/C++ 移植版本，支援 CPU/GPU 推論、量化與跨平台。
- [FunASR](https://github.com/modelscope/FunASR) — 工業級 ASR 工具包，具備 Paraformer、SenseVoice、VAD、說話人分段、串流與 OpenAI 相容 API。
- [vosk-api](https://github.com/alphacep/vosk-api) — 離線語音辨識工具包，具備僅 CPU 的小型模型，支援 20 多種語言與多語言綁定。
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — 離線語音工具包，使用新世代 Kaldi 與 ONNX Runtime，支援 STT、TTS、說話者識別、VAD 等。
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — 全面的語音工具包，具備 ASR、TTS、聲紋、說話人分段、翻譯與串流服務。
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — 語音模型，支援 50 多種語言的 ASR、情緒、音訊事件與快速非自迴歸推論。

### 系統層級語音輸入 / IME

整合在系統層級的語音輸入解決方案，包含輸入法、IBus/Fcitx 擴充、Android IME 與 iOS 鍵盤。

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME 與語音輸入服務，使用 Whisper 進行離線語音辨識與英文翻譯。
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Linux 離線語音輸入應用程式，具備 whisper.cpp、Whisper 與 VOSK 引擎，支援 Vulkan GPU 與 GTK GUI。
- [blurt](https://github.com/QuantiusBenignus/blurt) — GNOME Shell 擴充功能，透過 whisper.cpp 進行離線語音輸入，支援快捷鍵觸發、X11 與 Wayland。
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Android 離線語音辨識服務，使用 Vosk，支援標準 RecognitionService API。
- [Dictus](https://github.com/getdictus/dictus-ios) — 開源 iOS 鍵盤，使用 WhisperKit 與 CoreML 在裝置端進行語音輸入，可在任何 App 中使用。
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linux IBus 語音轉文字輸入法，具備串流 STT、選用的 Whisper 潤飾與 GPU 加速。

### 中文語音輸入 / IME

針對中文語音辨識與輸入最佳化的專案，包含基於 FunASR、Paraformer 與 SenseVoice 的中文輸入法與鍵盤。

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Linux 離線中文語音輸入，使用 FunASR Paraformer、IBus/Fcitx5、PTT 快捷鍵與句子潤飾。
- [voice-input-method](https://github.com/pofice/voice-input-method) — 跨平台離線語音輸入法，使用 FunASR，具備熱詞校正、自動貼上與 GUI/CLI 模式。
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android 語音輸入鍵盤，具備 11 種 ASR 引擎、LLM 後處理、懸浮球與 Material3 UI。

### 瀏覽器與網頁語音輸入

透過擴充功能、WebAssembly 包裝或網頁 UI 實現的瀏覽器語音輸入，通常需要本地或雲端 STT 後端。

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI，可從檔案、YouTube 或麥克風產生字幕，具備 VAD、背景音分離與說話人分段。
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — 瀏覽器擴充功能，透過 Vosk 進行即時離線語音轉文字，支援阿拉伯文與英文語音指令。
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — 瀏覽器端離線語音辨識函式庫，將 Vosk 封裝為在 WebWorker 中執行的 WebAssembly。
- [Speechfire](https://github.com/Jejkobb/Speechfire) — 瀏覽器擴充功能與本地 Whisper 伺服器，透過 Alt+A 在 Firefox 與 Chrome 中進行離線語音轉文字。
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Chrome 擴充功能，透過快捷鍵錄音，使用 OpenAI Whisper API 轉錄並自動貼上文字。
- [voico](https://github.com/Kirera-Wainaina/voico) — Chrome 擴充功能，將語音轉文字輸入到網頁欄位，後端使用 Node.js，並使用 Google 與 OpenAI STT。

### 行動裝置語音輸入（非 IME）

Android 或 iOS 上的獨立語音轉錄應用程式，而非輸入法鍵盤。

- [Transcribro](https://github.com/soupslurpr/Transcribro) — 適用於 Android 的私密裝置端語音辨識鍵盤，使用 Whisper（透過 whisper.cpp）與 Silero VAD。
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — 開源 iOS 應用程式，使用 Whisper.cpp 進行離線語音轉錄，具備錄音與音訊匯出。
- [seamless](https://github.com/woheller69/seamless) — Android 離線語音轉文字翻譯應用程式，使用 Meta Seamless M4T Lite 支援 5 種語言，並具備 TTS 輸出。

### 輕量腳本、CLI 與語音控制

適合開發者整合或作為現有工具鏈補充的輕量腳本、CLI 工具、系統匣觸發器或公用程式。

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linux 離線語音轉文字工具，使用 Vosk，可模擬鍵盤輸入到任何應用程式。
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash 腳本，透過 Whisper 在 TTY、X11、Wayland 與 WSL 上進行離線語音輸入，可選 LLM 編輯。
- [hns](https://github.com/primaprashant/hns) — CLI 工具，使用 faster-whisper 進行本地麥克風語音轉文字，支援複製到剪貼簿與輸出到 stdout。
- [Elograf](https://github.com/papoteur-mga/elograf) — nerd-dictation 的 PyQt6 GUI 管理器，具備系統匣、Vosk 模型、輸入模擬與 KDE 快捷鍵。
- [Osprey](https://github.com/osprey-voice/osprey) — 基於指令的語音控制與輸入工具，使用 Kaldi 與 Dragonfly 進行完全離線的語音辨識。

### 其他

尚未歸類的專案。

- [VoxType](https://github.com/peteonrails/voxtype) — Linux 與 Wayland 即按即說語音轉文字，提供七種本地 ASR 引擎、GPU 支援與會議模式。

## 開源專案與對照組

| 專案 | 價格 | 開源 | 可擴充 | 離線 | 中文 |
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

## 如何選擇

- **精緻的跨平台桌面應用程式** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri，25,281 顆星，Whisper/Parakeet 離線。
- **極簡 Linux 離線、可腳本化** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK，可模擬鍵盤輸入到任何應用程式。
- **將 STT 嵌入你自己的應用程式** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper，CPU/GPU，可嵌入。
- **中文優先輸入** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python、C++、Shell；使用 FunASR Paraformer、IBus/Fcitx5、PTT 快捷鍵與句子潤飾的 Linux 離線中文語音輸入。
- **自行架設轉錄 API/伺服器** → [FunASR](https://github.com/modelscope/FunASR) — 工業級 ASR 工具包，具備 Paraformer、SenseVoice、VAD、說話人分段、串流與 OpenAI 相容 API。

## 貢獻

歡迎貢獻 —— 參見 [CONTRIBUTING.md](CONTRIBUTING.md)。專案必須完全開源、可擴展且輕量；請遵循描述風格指南（使用英語，一行，事實性，無行銷廢話）。

## Star 歷史

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

本列表中獲星最多的專案隨時間的 star 成長情況。倉庫在審核期間為私有；其自身的 star 歷史將在公開後新增至此。

## 授權條款

[MIT](LICENSE).

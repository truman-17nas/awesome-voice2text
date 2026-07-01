# Awesome Voice Input

> 一份精选的开源语音输入 / 听写软件清单——完全开放、可扩展、轻量。以 Typeless、Lazytype 和 闪电说 为参照进行对比，它们均为闭源。

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*如果觉得这份清单有用，请给仓库 ⭐ Star，帮助更多人发现它。*

[English](README.md) · **简体中文** · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## 目录

- [基准（闭源）](#基准闭源)
- [为什么会有这份清单](#为什么会有这份清单)
- [收录标准](#收录标准)
- [精选推荐](#精选推荐)
- [全部项目](#全部项目)
- [分类列表](#分类列表)
  - [跨平台桌面实时听写](#跨平台桌面实时听写)
  - [原生 macOS 听写](#原生-macos-听写)
  - [AI 语音润色 / LLM 后处理](#ai-语音润色-llm-后处理)
  - [本地/离线 STT 引擎与工具包](#本地离线-stt-引擎与工具包)
  - [系统级语音输入 / 输入法](#系统级语音输入-输入法)
  - [中文语音输入 / 输入法](#中文语音输入-输入法)
  - [浏览器与网页语音输入](#浏览器与网页语音输入)
  - [移动设备语音输入（非输入法）](#移动设备语音输入非输入法)
  - [轻量脚本、CLI 与语音控制](#轻量脚本cli-与语音控制)
  - [其他](#其他)
- [开源与基准对比](#开源与基准对比)
- [如何选择](#如何选择)
- [贡献](#贡献)
- [Star 历史](#star-历史)
- [许可证](#许可证)

## 基准（闭源）

| 产品 | 定价 | 平台 | 模型/引擎 | 开源 |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## 为什么会有这份清单

Typeless、Lazytype 和 闪电说 功能强大，但都是闭源。这份清单收集符合三个标准的开源替代品：代码完全公开、工具可扩展、足够轻量，能够在个人机器上运行。目前涵盖 **75 个项目，分 9 个类别**，均已验证为完全开源。

## 收录标准

- ✅ **完全开源** — 所有代码托管在公开仓库（GitHub、GitLab、Codeberg）。
- 🔌 **可扩展** — 你可以添加想要的功能、模型或集成。
- ⚡ **轻量** — 极少冗余，启动迅速，占用资源少。

## 精选推荐

🏆 **[Handy](https://github.com/cjpais/Handy)** — 跨平台离线语音转文字工具，支持 Whisper 或 Parakeet、全局热键与剪贴板粘贴。*社区旗舰项目 — 25,281 Star，是最精致的方案。*

**Fit-5 推荐**（满足全部三个标准）：
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — OpenAI Whisper 的高性能 C/C++ 移植版，支持 CPU/GPU 推理、量化以及跨平台。
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — 基于 Vosk 的 Linux 离线语音转文字工具，可将输入模拟为键盘输入到任何应用。
- **[VoxType](https://github.com/peteonrails/voxtype)** — 适用于 Linux 和 Wayland 的按键即说语音转文字工具，内置七种本地 ASR 引擎、GPU 支持和会议模式。
- **[voice_typing](https://github.com/themanyone/voice_typing)** — 通过 Whisper 为 TTY、X11、Wayland 和 WSL 提供离线语音输入的 Bash 脚本，可选 LLM 编辑。

## 全部项目

| 名称 | ⭐ Star 数 | 许可证 | 语言 | 适配度 | 开源 | 可扩展 | 轻量 | 中文 |
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

## 分类列表

### 跨平台桌面实时听写

适用于 Linux、Windows 或跨平台的 Whisper 桌面听写应用，支持按键即说、本地转录和自动输入。

- [Handy](https://github.com/cjpais/Handy) — 跨平台离线语音转文字工具，支持 Whisper 或 Parakeet、全局热键与剪贴板粘贴。
- [Buzz](https://github.com/chidiwilliams/buzz) — 跨平台桌面 GUI，用于离线 Whisper 转录与翻译，支持 GPU 加速和实时麦克风。
- [Vibe](https://github.com/thewh1teagle/vibe) — 跨平台桌面应用，使用 Whisper 离线转录音频和视频，支持 GPU 加速。
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — 本地优先的应用工具包，支持 Markdown/SQLite 存储、Yjs CRDT 同步和桌面语音转文字工具。
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux 原生语音转文字，支持本地 Whisper 和 ONNX 模型、云端 API、Waybar 集成和可视化。
- [whisper-writer](https://github.com/savbell/whisper-writer) — 桌面听写应用，可在本地或通过 API 使用 Whisper，通过全局热键输入到活动窗口。
- [Chirp](https://github.com/Whamp/chirp-stt) — Windows 仅 CPU 的听写应用，使用 ParakeetV3，支持热键切换、剪贴板粘贴和词覆盖。
- [Dabri](https://github.com/AshBuk/dabri) — Linux 离线 STT 应用，使用 whisper.cpp，支持 X11/Wayland 桌面的守护进程、CLI 和 WebSocket 模式。
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux 和 Sailfish OS 离线笔记应用，使用多种引擎实现本地 STT、TTS 和翻译。
- [voxd](https://github.com/jakovius/voxd) — Linux 桌面语音听写，使用 whisper.cpp 进行离线 ASR，支持 ydotool 输入和 AI 后处理。
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linux 离线语音输入，通过 Whisper、Parakeet 或 Canary ONNX 实现，支持 X11/Wayland 和 LLM 润色。
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windows 语音输入助手，使用 Caps Lock 热键，支持多供应商 STT 和可选 LLM 优化。
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — 跨平台离线听写应用，使用 distil-whisper，支持热键控制和可选本地 LLM 助手。
- [TalkType](https://github.com/lmacan1/talktype) — 跨平台按键即说语音输入，使用 faster-whisper，支持全局热键和智能粘贴。
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — 离线多语言听写应用，使用 Faster-Whisper，通过热键触发转录到活动字段。
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — NixOS/Wayland 本地语音听写，使用 whisper.cpp，提供 GTK4 反馈并支持 99 种语言。
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux Wayland 语音听写应用，支持 STT、通过 LanguageTool 进行语法校正和 ydotool 文本输入。
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — 本地 AI 桌面助手，融合语音听写、LLM 聊天、图像生成和语音驱动自动化。
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows 桌面语音转文字，使用 faster-whisper，支持键盘模拟、VAD、PTT 和标点。
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — 适用于 KDE Wayland 的 Whisper 语音听写，支持后台守护进程、systemd 服务和剪贴板粘贴。

### 原生 macOS 听写

使用 Swift 和 WhisperKit 构建的原生 macOS 听写应用，支持全局热键、菜单栏和 Neural Engine 加速。

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — 支持 Whisper 和 Parakeet 引擎、全局热键和批量处理的 macOS 语音转写应用。
- [Pindrop](https://github.com/watzon/pindrop) — 使用 WhisperKit 进行离线 STT 的原生 macOS 菜单栏听写应用，支持热键和可选 AI 清理。
- [whisper-dictation](https://github.com/foges/whisper-dictation) — 使用 Whisper 的离线多语言听写工具，通过热键触发转录到任意输入字段。
- [FnKey](https://github.com/evoleinik/fnkey) — 按住 Fn 时通过 Deepgram Nova-3 转录语音并粘贴结果的 macOS 菜单栏应用。
- [hush](https://github.com/djmunro/hush) — 使用本地 Whisper/Parakeet ONNX 并通过热键自动粘贴的 macOS 按键即说听写应用。
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — 使用离线 Whisper 并支持 Metal GPU 加速和光标处文本注入的 macOS 菜单栏听写应用。
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS 菜单栏应用，Globe/Fn 释放时开始录音，通过 faster-whisper 转录并粘贴到光标处。

### AI 语音润色 / LLM 后处理

使用本地或云端 LLM 对语音识别输出进行润色、格式化、摘要和重写的听写工具。

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — 支持设备端和云端 STT、全局热键、AI 工作流、插件、REST API 和 CLI 的 macOS 听写应用。
- [Amical](https://github.com/amicalhq/amical) — 使用 Whisper 进行离线转写、使用 Ollama 进行智能笔记处理的本地优先 AI 听写应用。
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — 支持 macOS/Windows、使用 Whisper 的离线语音听写工具，支持全局热键和可选 AI 增强。
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — 面向 macOS 和 Linux 的本地优先语音助手，支持按键即说、转录和插件提取。
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — 使用 Whisper 和 LLM 清理、通过 Cmd-V 粘贴润色文本的 macOS 按键即说听写应用。
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — 支持 Whisper 和 LLM 润色、按键即说、词典和客户端-服务器架构的本地语音听写。
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — 支持 faster-whisper、LLM 摘要和双轨音频录制的本地语音听写和会议记录工具。
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — 使用本地 whisper.cpp 模型、支持全局快捷键和上下文感知模式的原生 macOS 语音转文字应用。
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — 支持设备端语音识别和可选 AI 后处理以进行格式化的 macOS 听写应用。
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — 支持热键、AI 助手、会议说话人分离和语义搜索的桌面语音转写应用。
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — 使用 Whisper 和 Apple Silicon 上的 Qwen 进行离线语音转文字和会议摘要的 macOS 菜单栏应用。
- [Voquill](https://github.com/voquill/voquill) — 使用本地 Whisper 或 Groq、AI 清理、词汇表和语音助手的跨平台 Tauri 语音输入应用。
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — 支持 LLM 格式化、本地 Whisper、Ollama 或云端 API 的跨平台语音听写助手。
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — 支持 AI 语音输入、文本改写和语音问答及全局热键的跨平台 Tauri 应用。
- [Aria](https://github.com/Xingxun7777/Aria) — 使用离线 Qwen3-ASR、OCR 上下文、热词纠正和语音命令的 Windows AI 语音输入。
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — 在 Windows 上使用 whisper.cpp、Groq 或 llama.cpp 进行语音听写，支持多种风格并自动粘贴到活动窗口。
- [localflow](https://github.com/sidharth-n/localflow) — 使用 Moonshine STT、Qwen3-4B 润色、按键即说和跳过门的本地跨平台语音听写。
- [yammer](https://github.com/andynu/yammer) — 支持 Whisper 和 LLM 清理、Tauri 覆盖层 UI 和 xdotool 输入注入的 Linux 本地语音转文字。

### 本地/离线 STT 引擎与工具包

可集成到应用中的离线 ASR 引擎和语音工具包：Whisper、Kaldi、ONNX、Vosk、FunASR、PaddleSpeech 和 SenseVoice。

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — OpenAI Whisper 的高性能 C/C++ 移植版，支持 CPU/GPU 推理、量化以及跨平台。
- [FunASR](https://github.com/modelscope/FunASR) — 工业级 ASR 工具包，支持 Paraformer、SenseVoice、VAD、说话人分离、流式识别和 OpenAI 兼容 API。
- [vosk-api](https://github.com/alphacep/vosk-api) — 离线语音识别工具包，提供 20+ 语言的小型纯 CPU 模型和多种语言绑定。
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — 使用新一代 Kaldi 和 ONNX Runtime 的离线语音工具包，支持 STT、TTS、说话人识别、VAD 等。
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — 综合性语音工具包，支持 ASR、TTS、声纹、说话人分离、翻译和流式服务。
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — 支持 50+ 语言 ASR、情感、音频事件和快速非自回归推理的语音模型。

### 系统级语音输入 / 输入法

在系统层面集成的语音输入方案，包括输入法、IBus/Fcitx 扩展、Android IME 和 iOS 键盘。

- [Whisper IME](https://github.com/woheller69/whisperIME) — 使用 Whisper 进行离线语音识别和英文翻译的 Android IME 和语音输入服务。
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — 支持 whisper.cpp、Whisper 和 VOSK 引擎、Vulkan GPU 和 GTK GUI 的 Linux 离线语音听写应用。
- [blurt](https://github.com/QuantiusBenignus/blurt) — 通过 whisper.cpp 实现离线语音输入的 GNOME Shell 扩展，支持热键触发，兼容 X11 和 Wayland。
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — 使用 Vosk 的 Android 离线语音识别服务，支持标准 RecognitionService API。
- [Dictus](https://github.com/getdictus/dictus-ios) — 使用 WhisperKit 和 CoreML 的 iOS 开源键盘，可在任何应用中进行设备端语音听写。
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — 支持流式 STT、可选 Whisper 优化和 GPU 加速的 Linux IBus 语音输入输入法。

### 中文语音输入 / 输入法

针对中文语音识别和输入优化的项目，包括基于 FunASR、Paraformer 和 SenseVoice 的中文输入法与键盘。

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — 使用 FunASR Paraformer、IBus/Fcitx5、PTT 热键和句子润色的 Linux 离线中文语音输入。
- [voice-input-method](https://github.com/pofice/voice-input-method) — 使用 FunASR 的跨平台离线语音输入法，支持热词纠正、自动粘贴和 GUI/CLI 模式。
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — 集成 11 种 ASR 引擎、LLM 后处理、悬浮球和 Material3 UI 的 Android 语音输入键盘。

### 浏览器与网页语音输入

通过扩展、WebAssembly 包装或 Web UI 实现的基于浏览器的语音输入，通常需要本地或云端 STT 后端。

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — 用于从文件、YouTube 或麦克风生成字幕的 Gradio Whisper WebUI，支持 VAD、背景音乐分离和说话人分离。
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — 通过 Vosk 实现实时离线语音转文字的浏览器扩展，支持阿拉伯语和英语语音命令。
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — 将 Vosk 封装为 WebAssembly 并在 WebWorker 中运行的浏览器离线语音识别库。
- [Speechfire](https://github.com/Jejkobb/Speechfire) — 适用于 Firefox 和 Chrome 的浏览器扩展和本地 Whisper 服务器，通过 Alt+A 离线语音转文字。
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — 通过热键录音并使用 OpenAI Whisper API 转录后自动粘贴文本的 Chrome 扩展。
- [voico](https://github.com/Kirera-Wainaina/voico) — 用于向网页字段输入语音转文字的 Chrome 扩展，后端使用 Google 和 OpenAI STT。

### 移动设备语音输入（非输入法）

Android 或 iOS 上的独立语音转录应用，而非输入法键盘。

- [Transcribro](https://github.com/soupslurpr/Transcribro) — 使用 whisper.cpp 和 Silero VAD 在 Android 上实现设备端私密语音识别键盘。
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — 使用 Whisper.cpp 进行离线语音转录的开源 iOS 应用，支持录音和音频导出。
- [seamless](https://github.com/woheller69/seamless) — 使用 Meta Seamless M4T Lite 在 Android 上实现 5 种语言离线语音转文字翻译和 TTS 输出的应用。

### 轻量脚本、CLI 与语音控制

适合开发者集成或作为现有工具链补充的轻量脚本、CLI 工具、托盘触发器和实用工具。

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — 基于 Vosk 的 Linux 离线语音转文字工具，可将输入模拟为键盘输入到任何应用。
- [voice_typing](https://github.com/themanyone/voice_typing) — 通过 Whisper 为 TTY、X11、Wayland 和 WSL 提供离线语音输入的 Bash 脚本，可选 LLM 编辑。
- [hns](https://github.com/primaprashant/hns) — 使用 faster-whisper 进行本地麦克风语音转文字的 CLI 工具，支持复制到剪贴板和 stdout 管道。
- [Elograf](https://github.com/papoteur-mga/elograf) — 面向 nerd-dictation 的 PyQt6 GUI 管理器，提供系统托盘、Vosk 模型、输入模拟和 KDE 热键。
- [Osprey](https://github.com/osprey-voice/osprey) — 使用 Kaldi 和 Dragonfly 实现完全本地语音识别的基于命令的语音控制和输入工具。

### 其他

尚未分类的项目。

- [VoxType](https://github.com/peteonrails/voxtype) — 适用于 Linux 和 Wayland 的按键即说语音转文字工具，内置七种本地 ASR 引擎、GPU 支持和会议模式。

## 开源与基准对比

| 项目 | 价格 | 开源 | 可扩展 | 离线可用 | 中文 |
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

## 如何选择

- **精致的跨平台桌面应用** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri，25,281 Star，支持 Whisper/Parakeet 离线。
- **极简 Linux 离线、可脚本化** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK，可模拟键盘输入到任何应用。
- **在自己的应用中嵌入 STT** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper，支持 CPU/GPU，可嵌入。
- **中文优先输入** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python、C++、Shell；使用 FunASR Paraformer、IBus/Fcitx5、PTT 热键和句子润色的 Linux 离线中文语音输入。
- **自托管转录 API/服务器** → [FunASR](https://github.com/modelscope/FunASR) — 工业级 ASR 工具包，支持 Paraformer、SenseVoice、VAD、说话人分离、流式识别和 OpenAI 兼容 API。

## 贡献

欢迎投稿——请参阅 [CONTRIBUTING.md](CONTRIBUTING.md)。项目必须完全开源、可扩展、轻量；请遵循描述风格指南（英文、一行、实事求是、无营销花哨）。

## Star 历史

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

本列表中 Star 数最多项目的 Star 增长趋势。本仓库目前处于审核阶段且为私库，公开后会添加它自身的 Star 历史。

## 许可证

[MIT](LICENSE)。

# Awesome Voice Input

> 厳選されたオープンソースの音声入力・口述ソフトウェアのリスト — 完全にオープンで、拡張可能で、軽量。Typeless、Lazytype、Shandianshuo（闪电说）との比較対象であり、いずれもクローズドソースです。

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*このリストが役立つ場合は、repoに⭐をつけてください — 他の人が見つけやすくなります。*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · **日本語** · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## 目次

- [比較対象（クローズドソース）](#比較対象クローズドソース)
- [このリストの理由](#このリストの理由)
- [採用基準](#採用基準)
- [トップピック](#トップピック)
- [すべてのプロジェクト](#すべてのプロジェクト)
- [カテゴリ別リスト](#カテゴリ別リスト)
  - [クロスプラットフォームデスクトップリアルタイム口述](#クロスプラットフォームデスクトップリアルタイム口述)
  - [ネイティブmacOS口述](#ネイティブmacos口述)
  - [AI音声清書/LLM後処理](#ai音声清書llm後処理)
  - [ローカル/オフラインSTTエンジンとツールキット](#ローカルオフラインsttエンジンとツールキット)
  - [システムレベル音声入力/IME](#システムレベル音声入力ime)
  - [中国語音声入力/IME](#中国語音声入力ime)
  - [ブラウザ/ウェブ音声入力](#ブラウザウェブ音声入力)
  - [モバイル音声入力（非IME）](#モバイル音声入力非ime)
  - [軽量スクリプト、CLIと音声制御](#軽量スクリプトcliと音声制御)
  - [その他](#その他)
- [オープンソースと比較対象](#オープンソースと比較対象)
- [選び方](#選び方)
- [コントリビューション](#コントリビューション)
- [Star 履歴](#star-履歴)
- [ライセンス](#ライセンス)

## 比較対象（クローズドソース）

| 製品 | 価格 | プラットフォーム | モデル/エンジン | オープンソース |
| --- | --- | --- | --- | --- |
| Typeless | フリーミアム：無料 8K 文字/週；Pro $12/月 年払い（$30/月 月払い） | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | 無料（ローカル/BYOK）；Pro ¥29/月 または ¥238.8/年 | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## このリストの理由

Typeless、Lazytype、Shandianshuo（闪电说）は強力ですが、クローズドソースです。このリストは、次の3つの基準を満たすオープンソースの代替品を集めています：コードが完全に公開されていること、ツールが拡張可能であること、そして個人のマシンで実行できるほど軽量であることです。現在、**9カテゴリ75プロジェクト**をカバーしており、いずれも完全にオープンソースであることを確認しています。

## 採用基準

- ✅ **完全なオープンソース** — すべてのコードが公開されたForge（GitHub、GitLab、Codeberg）上にあること。
- 🔌 **拡張可能** — 必要な機能、モデル、統合を追加できること。
- ⚡ **軽量** — 肥大化せず、起動が速く、フットプリントが小さいこと。

## トップピック

🏆 **[Handy](https://github.com/cjpais/Handy)** — Whisper または Parakeet を使ったクロスプラットフォームのオフライン音声入力ツール。グローバルホットキーとクリップボード貼り付けに対応。*コミュニティの旗艦 — 25,281 スター、最も洗練された選択肢。*

**Fit-5 選択肢**（3つの基準をすべて満たす）：
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — OpenAI Whisper の高性能 C/C++ 移植版。CPU/GPU 推論、量子化、クロスプラットフォーム対応。
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Vosk を使った Linux 用オフライン音声入力ツール。任意のアプリケーションにキーボード入力を模倣する。
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux および Wayland 向けプッシュトーク型音声入力。7つのローカル ASR エンジン、GPU 対応、会議モードを搭載。
- **[voice_typing](https://github.com/themanyone/voice_typing)** — TTY、X11、Wayland、WSL 上で Whisper を使ったオフライン音声入力を行う Bash スクリプト。LLM による編集も可能。

## すべてのプロジェクト

| 名前 | ⭐ スター | ライセンス | 言語 | 適合 | オープン | 拡張 | 軽量 | 中国語 |
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

## カテゴリ別リスト

### クロスプラットフォームデスクトップリアルタイム口述

Linux、Windows、またはクロスプラットフォーム向けの、プッシュトーク、ローカル文字起こし、自動入力に対応した Whisper ベースのデスクトップ口述アプリ。

- [Handy](https://github.com/cjpais/Handy) — Whisper または Parakeet を使ったクロスプラットフォームのオフライン音声入力ツール。グローバルホットキーとクリップボード貼り付けに対応。
- [Buzz](https://github.com/chidiwilliams/buzz) — GPU 加速とライブマイクに対応した、オフライン Whisper 文字起こし・翻訳用クロスプラットフォームデスクトップ GUI。
- [Vibe](https://github.com/thewh1teagle/vibe) — GPU 加速を備えた、Whisper を使ったオフライン音声・動画文字起こし用クロスプラットフォームデスクトップアプリ。
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Markdown/SQLite ストレージ、Yjs CRDT 同期、デスクトップ音声入力ユーティリティを備えたローカルファーストアプリツールキット。
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — ローカル Whisper と ONNX モデル、クラウド API、Waybar 統合、ビジュアライザーを備えた Linux ネイティブ音声入力。
- [whisper-writer](https://github.com/savbell/whisper-writer) — Whisper をローカルまたは API で使い、グローバルホットキーでアクティブウィンドウに入力するデスクトップ口述アプリ。
- [Chirp](https://github.com/Whamp/chirp-stt) — ParakeetV3 を使った Windows 専用 CPU 口述アプリ。ホットキートグル、クリップボード貼り付け、単語上書きに対応。
- [Dabri](https://github.com/AshBuk/dabri) — whisper.cpp を使った Linux オフライン STT アプリ。X11/Wayland デスクトップ向けにデーモン、CLI、WebSocket モードを提供。
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — 複数のエンジンを使ったローカル STT、TTS、翻訳に対応した Linux および Sailfish OS オフラインメモアプリ。
- [voxd](https://github.com/jakovius/voxd) — whisper.cpp を使ったオフライン ASR で、ydotool 入力と AI 後処理を行う Linux デスクトップ音声口述。
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Whisper、Parakeet、または Canary ONNX を使った Linux オフライン音声入力。X11/Wayland 対応と LLM 修飾を備える。
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Caps Lock ホットキー、マルチプロバイダー STT、オプションの LLM 洗練化を備えた Windows 音声入力アシスタント。
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — distil-whisper、ホットキー制御、オプションのローカル LLM アシスタントを備えたクロスプラットフォームオフライン口述アプリ。
- [TalkType](https://github.com/lmacan1/talktype) — faster-whisper を使ったクロスプラットフォームプッシュトーク音声入力。グローバルホットキーとスマート貼り付けに対応。
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — ホットキーでアクティブフィールドに文字起こしする、Faster-Whisper を使ったオフライン多言語口述アプリ。
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — whisper.cpp を使った NixOS/Wayland ローカル音声口述。GTK4 フィードバックと 99 言語対応。
- [freespeak](https://github.com/Zetaphor/freespeak) — STT、LanguageTool による文法修正、ydotool テキスト入力を備えた Linux Wayland 音声口述アプリ。
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — 音声口述、LLM チャット、画像生成、音声主導の自動化を組み合わせたローカル AI デスクトップエージェント。
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — faster-whisper を使った Windows デスクトップ音声入力。キーボードシミュレーション、VAD、PTT、句読点に対応。
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — バックグラウンドデーモン、systemd サービス、クリップボード貼り付けを備えた KDE Wayland 向け Whisper 音声口述。

### ネイティブmacOS口述

Swift と WhisperKit で構築されたネイティブ macOS 口述アプリ。グローバルホットキー、メニューバー、Neural Engine 加速に対応。

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Whisper と Parakeet エンジン、グローバルホットキー、バッチ処理を備えた macOS 音声文字起こしアプリ。
- [Pindrop](https://github.com/watzon/pindrop) — WhisperKit を使ったオフライン STT のネイティブ macOS メニューバー口述アプリ。ホットキーとオプションの AI 清書に対応。
- [whisper-dictation](https://github.com/foges/whisper-dictation) — ホットキーでトリガーされ、任意の入力フィールドに文字起こしするオフライン多言語口述ツール。
- [FnKey](https://github.com/evoleinik/fnkey) — Fn キー長押し中に Deepgram Nova-3 で音声を文字起こしし、結果を貼り付ける macOS メニューバーアプリ。
- [hush](https://github.com/djmunro/hush) — ローカル Whisper/Parakeet ONNX を使い、ホットキーで自動貼り付けする macOS プッシュトーク口述アプリ。
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — オフライン Whisper と Metal GPU 加速を使い、カーソル位置にテキストを注入する macOS メニューバー口述アプリ。
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Globe/Fn キー離しで録音し、faster-whisper で文字起こし、カーソル位置に貼り付ける Apple macOS メニューバーアプリ。

### AI音声清書/LLM後処理

ローカルまたはクラウド LLM を使って、音声認識結果を清書、整形、要約、スタイル変更する口述ツール。

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — オンデバイスとクラウド STT、グローバルホットキー、AI ワークフロー、プラグイン、REST API、CLI を備えた macOS 口述アプリ。
- [Amical](https://github.com/amicalhq/amical) — Whisper でオフライン文字起こし、Ollama でスマートメモ処理を行うローカルファースト AI 口述アプリ。
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Whisper を使った macOS/Windows 向けオフライン音声口述ツール。グローバルホットキーとオプションの AI 強化に対応。
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — プッシュトーク、文字起こし、プラグイン抽出を備えた macOS と Linux 向けローカルファースト音声アシスタント。
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Whisper と LLM 清書を使い、Cmd-V で整形済みテキストを貼り付ける macOS プッシュトーク口述アプリ。
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Whisper と LLM 研磨、プッシュトーク、辞書、クライアント-サーバー分割を備えたローカル音声口述。
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — faster-whisper、LLM 要約、デュアルトラック音声録音を備えたローカル音声口述と会議録音ツール。
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — ローカル whisper.cpp モデルを使ったネイティブ macOS 音声入力アプリ。グローバルショートカットとコンテキスト対応モードを備える。
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — オンデバイス音声認識と、オプションの AI 後処理による整形を備えた macOS 口述アプリ。
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — ホットキー、AI アシスタント、会議話者分離、セマンティック検索を備えたデスクトップ音声文字起こしアプリ。
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Whisper と Apple Silicon 上の Qwen を使ったオフライン音声入力と会議要約を行う macOS メニューバーアプリ。
- [Voquill](https://github.com/voquill/voquill) — ローカル Whisper または Groq、AI 清書、用語集、音声アシスタントを備えたクロスプラットフォーム Tauri 音声入力アプリ。
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — LLM 整形に対応したクロスプラットフォーム音声口述アシスタント。ローカル Whisper、Ollama、またはクラウド API を選択可能。
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — AI 音声入力、テキスト書き換え、音声 Q&A をグローバルホットキーで行うクロスプラットフォーム Tauri アプリ。
- [Aria](https://github.com/Xingxun7777/Aria) — OCR コンテキスト、ホットワード補正、音声コマンドを備えた、オフライン Qwen3-ASR を使う Windows AI 音声入力。
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — whisper.cpp、Groq、または llama.cpp を使い、複数のスタイルでアクティブウィンドウに自動貼り付けする Windows 音声口述。
- [localflow](https://github.com/sidharth-n/localflow) — Moonshine STT、Qwen3-4B 研磨、プッシュトーク、スキップゲートを備えたローカルクロスプラットフォーム音声口述。
- [yammer](https://github.com/andynu/yammer) — Whisper と LLM 清書、Tauri オーバーレイ UI、xdotool 入力注入を備えた Linux ローカル音声入力。

### ローカル/オフラインSTTエンジンとツールキット

アプリ統合向けのオフライン ASR エンジンと音声ツールキット：Whisper、Kaldi、ONNX、Vosk、FunASR、PaddleSpeech、SenseVoice。

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — OpenAI Whisper の高性能 C/C++ 移植版。CPU/GPU 推論、量子化、クロスプラットフォーム対応。
- [FunASR](https://github.com/modelscope/FunASR) — Paraformer、SenseVoice、VAD、話者分離、ストリーミング、OpenAI 互換 API を備えた産業用 ASR ツールキット。
- [vosk-api](https://github.com/alphacep/vosk-api) — 20 言語以上の小型 CPU 専用モデルとマルチ言語バインディングを備えたオフライン音声認識ツールキット。
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — 次世代 Kaldi と ONNX Runtime を使った、STT、TTS、話者識別、VAD などを行うオフライン音声ツールキット。
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — ASR、TTS、声紋、話者分離、翻訳、ストリーミングサービスを備えた総合的な音声ツールキット。
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — 50 言語以上の ASR、感情、音声イベント、高速非自動回帰推論に対応した音声モデル。

### システムレベル音声入力/IME

入力メソッド、IBus/Fcitx 拡張、Android IME、iOS キーボードなど、システムレベルで統合された音声入力ソリューション。

- [Whisper IME](https://github.com/woheller69/whisperIME) — Whisper を使ったオフライン音声認識と英語翻訳を行う Android IME および音声入力サービス。
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — whisper.cpp、Whisper、VOSK エンジン、Vulkan GPU、GTK GUI を備えた Linux オフライン音声口述アプリ。
- [blurt](https://github.com/QuantiusBenignus/blurt) — whisper.cpp を使ったオフライン音声入力用 GNOME Shell 拡張。ホットキーでトリガーし、X11 と Wayland に対応。
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — 標準 RecognitionService API に対応した Vosk を使う Android オフライン音声認識サービス。
- [Dictus](https://github.com/getdictus/dictus-ios) — WhisperKit と CoreML を使ったオンデバイス音声口述用オープンソース iOS キーボード。任意のアプリで動作。
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — ストリーミング STT、オプションの Whisper 洗練化、GPU 加速を備えた Linux IBus 音声入力メソッド。

### 中国語音声入力/IME

中国語音声認識と入力に最適化されたプロジェクト。FunASR、Paraformer、SenseVoice ベースの中国語 IME とキーボードを含む。

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — FunASR Paraformer、IBus/Fcitx5、PTT ホットキー、文の洗練化を備えた Linux オフライン中国語音声入力。
- [voice-input-method](https://github.com/pofice/voice-input-method) — ホットワード補正、自動貼り付け、GUI/CLI モードを備えた FunASR を使うクロスプラットフォームオフライン音声入力メソッド。
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — 11 の ASR エンジン、LLM 後処理、フローティングボール、Material3 UI を備えた Android 音声入力キーボード。

### ブラウザ/ウェブ音声入力

拡張機能、WebAssembly ラッパー、Web UI を介したブラウザベースの音声入力。通常、ローカルまたはクラウド STT バックエンドが必要。

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — ファイル、YouTube、マイクからの字幕生成用 Gradio Whisper WebUI。VAD、BGM 分離、話者分離に対応。
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Vosk を使ったリアルタイムオフライン音声入力のブラウザ拡張。アラビア語と英語の音声コマンドに対応。
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Vosk を WebAssembly として WebWorker 内で動作させるブラウザベースオフライン音声認識ライブラリ。
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Firefox と Chrome で Alt+A によるオフライン音声入力を行う、ブラウザ拡張とローカル Whisper サーバー。
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — ホットキーで音声を録音し、OpenAI Whisper API で文字起こし、自動貼り付けする Chrome 拡張。
- [voico](https://github.com/Kirera-Wainaina/voico) — Google および OpenAI STT を使う Node.js バックエンドと共に、Web フィールドへの音声入力を行う Chrome 拡張。

### モバイル音声入力（非IME）

入力メソッドキーボードではなく、Android または iOS 上の独立した音声文字起こしアプリ。

- [Transcribro](https://github.com/soupslurpr/Transcribro) — whisper.cpp と Silero VAD を使った Android 向けオンデバイス音声認識キーボード。
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Whisper.cpp を使ったオフライン音声文字起こし用オープンソース iOS アプリ。録音と音声エクスポートに対応。
- [seamless](https://github.com/woheller69/seamless) — Meta Seamless M4T Lite を使った 5 言語対応の Android オフライン音声入力翻訳アプリ。TTS 出力付き。

### 軽量スクリプト、CLIと音声制御

開発者の統合や既存のツールチェインの補助に適した、軽量なスクリプト、CLI ツール、トレイトリガー、ユーティリティ。

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Vosk を使った Linux オフライン音声入力ツール。任意のアプリケーションにキーボード入力を模倣する。
- [voice_typing](https://github.com/themanyone/voice_typing) — TTY、X11、Wayland、WSL 上で Whisper を使ったオフライン音声入力を行う Bash スクリプト。LLM による編集も可能。
- [hns](https://github.com/primaprashant/hns) — faster-whisper を使ったローカルマイク音声入力 CLI ツール。クリップボードコピーと stdout パイプに対応。
- [Elograf](https://github.com/papoteur-mga/elograf) — システムトレイ、Vosk モデル、入力シミュレーション、KDE ホットキーを備えた nerd-dictation 用 PyQt6 GUI マネージャー。
- [Osprey](https://github.com/osprey-voice/osprey) — Kaldi と Dragonfly を使った、完全にローカルな音声認識を行うコマンドベースの音声制御・入力ツール。

### その他

まだカテゴリに割り当てられていないプロジェクト。

- [VoxType](https://github.com/peteonrails/voxtype) — Linux と Wayland 向けプッシュトーク音声入力。7つのローカル ASR エンジン、GPU 対応、会議モードを搭載。

## オープンソースと比較対象

| プロジェクト | 価格 | オープンソース | 拡張 | オフライン | 中国語 |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 無料 (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | 無料 (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | 無料 (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | 無料 (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | 無料 (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | 無料 (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(クローズド)* | フリーミアム：無料 8K 文字/週；Pro $12/月 年払い（$30/月 月払い） | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(クローズド)* | パーソナル €25 一回払い（BYOK Groq）；Pro €5/月 ホスト型 | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(クローズド)* | 無料（ローカル/BYOK）；Pro ¥29/月 または ¥238.8/年 | ❌ | ❌ | ◐ | ◐ |

## 選び方

- **洗練されたクロスプラットフォームデスクトップアプリ** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri、25,281 スター、Whisper/Parakeet オフライン。
- **ミニマルな Linux オフライン、スクリプト可能** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK、任意のアプリにキーボード入力を模倣。
- **独自のアプリに STT を組み込む** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper、CPU/GPU、組み込み可能。
- **中国語優先の入力** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python、C++、Shell；FunASR Paraformer、IBus/Fcitx5、PTT ホットキー、文の洗練化を備えた Linux オフライン中国語音声入力。
- **文字起こし API/サーバーを自前でホストする** → [FunASR](https://github.com/modelscope/FunASR) — Paraformer、SenseVoice、VAD、話者分離、ストリーミング、OpenAI 互換 API を備えた産業用 ASR ツールキット。

## コントリビューション

コントリビューションを歓迎します — 詳しくは [CONTRIBUTING.md](CONTRIBUTING.md) を参照してください。プロジェクトは完全にオープンソースで、拡張性があり、軽量である必要があります。説明のスタイルガイド（英語で、1行、事実に基づき、マーケティング表現なし）に従ってください。

## Star 履歴

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

このリストで最もスター数の多いプロジェクトの経時的なスター増加状況です。リポジトリ自体はレビュー中はプライベートです。公開後にそのスター履歴をこちらに追加します。

## ライセンス

[MIT](LICENSE).

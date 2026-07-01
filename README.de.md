# Awesome Voice2Text

> Eine kuratierte Liste quelloffener Spracheingabe-/Diktat-Software — vollständig offen, erweiterbar und leichtgewichtig. Verglichen mit Typeless, Lazytype und Shandianshuo (闪电说), die alle Closed-Source sind.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Wenn diese Liste nützlich ist, gib dem Repo bitte einen ⭐ — das hilft anderen, es zu finden.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · **Deutsch** · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Inhaltsverzeichnis

- [Benchmarks (Closed-Source)](#benchmarks-closed-source)
- [Warum diese Liste](#warum-diese-liste)
- [Aufnahmekriterien](#aufnahmekriterien)
- [Top-Empfehlungen](#top-empfehlungen)
- [Alle Projekte](#alle-projekte)
- [Kategorisierte Liste](#kategorisierte-liste)
  - [Plattformübergreifende Desktop-Echtzeit-Diktat](#plattformübergreifende-desktop-echtzeit-diktat)
  - [Native macOS-Diktat](#native-macos-diktat)
  - [KI-Sprachbereinigung / LLM-Nachbearbeitung](#ki-sprachbereinigung-llm-nachbearbeitung)
  - [Lokale/Offline-STT-Engines und Toolkits](#lokaleoffline-stt-engines-und-toolkits)
  - [Systemweite Spracheingabe / IME](#systemweite-spracheingabe-ime)
  - [Chinesische Spracheingabe / IME](#chinesische-spracheingabe-ime)
  - [Browser und Web-Spracheingabe](#browser-und-web-spracheingabe)
  - [Mobile Spracheingabe (Non-IME)](#mobile-spracheingabe-non-ime)
  - [Leichtgewichtige Skripte, CLI & Sprachsteuerung](#leichtgewichtige-skripte-cli-sprachsteuerung)
  - [Sonstiges](#sonstiges)
- [Open-Source vs. Benchmarks](#open-source-vs-benchmarks)
- [Auswahlhilfe](#auswahlhilfe)
- [Mitwirken](#mitwirken)
- [Star-Verlauf](#star-verlauf)
- [Lizenz](#lizenz)

## Benchmarks (Closed-Source)

| Produkt | Preisgestaltung | Plattformen | Modell/Engine | Open Source |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Kostenlos 8K Wörter/Woche; Pro $12/mo jährlich ($30/mo monatlich) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 einmalig (BYOK Groq); Pro €5/mo gehostet | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Kostenlos (lokal/BYOK); Pro ¥29/mo oder ¥238.8/Jahr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Warum diese Liste

Typeless, Lazytype und Shandianshuo (闪电说) sind leistungsstark, aber Closed-Source. Diese Liste sammelt quelloffene Alternativen, die drei Kriterien erfüllen: Der Code ist vollständig öffentlich, das Tool lässt sich erweitern und ist leicht genug, um auf einem persönlichen Rechner zu laufen. Sie umfasst aktuell **75 Projekte in 9 Kategorien**, alle als vollständig quelloffen verifiziert.

## Aufnahmekriterien

- ✅ **Vollständig quelloffen** — gesamter Code in einem öffentlichen Forge (GitHub, GitLab, Codeberg).
- 🔌 **Erweiterbar** — du kannst die Features, Modelle oder Integrationen hinzufügen, die du möchtest.
- ⚡ **Leichtgewichtig** — wenig Ballast, schneller Start, kleiner Fußabdruck.

## Top-Empfehlungen

🏆 **[Handy](https://github.com/cjpais/Handy)** — Plattformübergreifendes Offline-Sprache-zu-Text-Tool, das Whisper oder Parakeet nutzt, mit globalen Hotkeys und Einfügen aus der Zwischenablage. *Community-Flaggschiff — 25,281 Sterne, die am besten ausgereifte Lösung.*

**Fit-5-Empfehlungen** (erfüllen alle drei Kriterien):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Hochleistungsfähige C/C++-Portierung von OpenAI Whisper mit CPU/GPU-Inferenz, Quantisierung und plattformübergreifender Unterstützung.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linux-Offline-Sprache-zu-Text-Tool, das Vosk nutzt und Tastatureingaben in jede Anwendung simuliert.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Push-to-Talk-Sprache-zu-Text für Linux und Wayland mit sieben lokalen ASR-Engines, GPU-Unterstützung und Meeting-Modus.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash-Skript für Offline-Spracheingabe via Whisper für TTY, X11, Wayland und WSL mit optionaler LLM-Bearbeitung.

## Alle Projekte

| Name | ⭐ Sterne | Lizenz | Sprache | Fit | Open | Ext | LW | Chinesisch |
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

## Kategorisierte Liste

### Plattformübergreifende Desktop-Echtzeit-Diktat

Whisper-basierte Desktop-Diktat-Apps für Linux, Windows oder plattformübergreifend, mit Push-to-Talk, lokaler Transkription und automatischer Eingabe.

- [Handy](https://github.com/cjpais/Handy) — Plattformübergreifendes Offline-Sprache-zu-Text-Tool, das Whisper oder Parakeet nutzt, mit globalen Hotkeys und Einfügen aus der Zwischenablage.
- [Buzz](https://github.com/chidiwilliams/buzz) — Plattformübergreifende Desktop-GUI für Offline-Whisper-Transkription und -Übersetzung mit GPU-Beschleunigung und Live-Mikrofon.
- [Vibe](https://github.com/thewh1teagle/vibe) — Plattformübergreifende Desktop-App für Offline-Audio- und -Video-Transkription mit Whisper und GPU-Beschleunigung.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Lokal-first-App-Toolkit mit Markdown/SQLite-Speicher, Yjs-CRDT-Synchronisation und einem Desktop-Sprache-zu-Text-Utility.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux-native Sprache-zu-Text mit lokalen Whisper- und ONNX-Modellen, Cloud-APIs, Waybar-Integration und Visualizer.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Desktop-Diktat-App, die Whisper lokal oder via API nutzt, ausgelöst durch globalen Hotkey zum Eintippen ins aktive Fenster.
- [Chirp](https://github.com/Whamp/chirp-stt) — Windows-Diktat-App nur für CPU mit ParakeetV3, Hotkey-Umschaltung, Zwischenablage-Einfügen und Wort-Overrides.
- [Dabri](https://github.com/AshBuk/dabri) — Linux-Offline-STT-App mit whisper.cpp im Daemon-, CLI- und WebSocket-Modus für X11/Wayland-Desktops.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Offline-Notiz-App für Linux und Sailfish OS mit lokaler STT, TTS und Übersetzung über mehrere Engines.
- [voxd](https://github.com/jakovius/voxd) — Linux-Desktop-Sprachdiktat mit whisper.cpp für offline ASR, ydotool-Tastatureingaben und KI-Nachbearbeitung.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linux-Offline-Spracheingabe via Whisper, Parakeet oder Canary ONNX mit X11/Wayland-Unterstützung und LLM-Feinschliff.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windows-Spracheingabe-Assistent mit Caps-Lock-Hotkey, Multi-Provider-STT und optionaler LLM-Verfeinerung.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Plattformübergreifende Offline-Diktat-App mit distil-whisper, Hotkey-Steuerung und optionalem lokalem LLM-Assistenten.
- [TalkType](https://github.com/lmacan1/talktype) — Plattformübergreifende Push-to-Talk-Spracheingabe mit faster-whisper, globalen Hotkeys und intelligentem Einfügen.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Offline mehrsprachige Diktat-App mit Faster-Whisper, ausgelöst durch Hotkey, um ins aktive Feld zu transkribieren.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Lokales Sprachdiktat für NixOS/Wayland mit whisper.cpp, GTK4-Feedback und Unterstützung für 99 Sprachen.
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux-Wayland-Sprachdiktat-App mit STT, Grammatikkorrektur via LanguageTool und ydotool-Texteingabe.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Lokaler KI-Desktop-Agent, der Sprachdiktat, LLM-Chat, Bildgenerierung und sprachgesteuerte Automatisierung verbindet.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows-Desktop-Sprache-zu-Text mit faster-whisper, Tastatursimulation, VAD, PTT und Zeichensetzung.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Whisper-Sprachdiktat für KDE Wayland mit Hintergrund-Daemon, systemd-Service und Einfügen aus der Zwischenablage.

### Native macOS-Diktat

Native macOS-Diktat-Apps mit Swift und WhisperKit, die globale Hotkeys, die Menüleiste und Neural-Engine-Beschleunigung unterstützen.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — macOS-Sprachtranskriptions-App mit Whisper- und Parakeet-Engines, globalen Hotkeys und Batch-Verarbeitung.
- [Pindrop](https://github.com/watzon/pindrop) — Native macOS-Menüleisten-Diktat-App mit WhisperKit für Offline-STT, Hotkeys und optionaler KI-Bereinigung.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Offline mehrsprachiges Diktat-Tool mit Whisper, ausgelöst durch Hotkey, um in jedes Eingabefeld zu transkribieren.
- [FnKey](https://github.com/evoleinik/fnkey) — macOS-Menüleisten-App, die Sprache via Deepgram Nova-3 transkribiert, während Fn gedrückt ist, und das Ergebnis einfügt.
- [hush](https://github.com/djmunro/hush) — macOS-Push-to-Talk-Diktat-App mit lokalen Whisper/Parakeet-ONNX und Auto-Einfügen via Hotkey.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — macOS-Menüleisten-Diktat-App mit offline Whisper, Metal-GPU-Beschleunigung und Texteingabe am Cursor.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — macOS-Menüleisten-App nimmt bei Loslassen von Globe/Fn auf, transkribiert via faster-whisper und fügt am Cursor ein.

### KI-Sprachbereinigung / LLM-Nachbearbeitung

Diktat-Tools, die lokale oder Cloud-LLMs nutzen, um Spracherkennungsausgaben zu polieren, zu formatieren, zusammenzufassen und in sauberen, formellen Text zu überführen.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — macOS-Diktat-App mit On-Device- und Cloud-STT, globalen Hotkeys, KI-Workflows, Plugins, REST-API und CLI.
- [Amical](https://github.com/amicalhq/amical) — Lokal-first-KI-Diktat-App mit Whisper für Offline-Transkription und Ollama für intelligente Notizverarbeitung.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Offline-Sprachdiktat-Tool für macOS/Windows mit Whisper, globalen Hotkeys und optionaler KI-Verbesserung.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Lokal-first-Sprachassistent für macOS und Linux mit Push-to-Talk, Transkription und Plugin-Extraktion.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — macOS-Push-to-Talk-Diktat-App mit Whisper und LLM-Bereinigung, die polierten Text via Cmd-V einfügt.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Lokales Sprachdiktat mit Whisper und LLM-Polishing, Push-to-Talk, Wörterbuch und Client-Server-Architektur.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Lokale Sprachdiktat- und Meeting-Recorder-App mit faster-whisper, LLM-Zusammenfassungen und Zwei-Spur-Audioaufnahme.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Native macOS-Sprache-zu-Text-App mit lokalen whisper.cpp-Modellen, globalen Tastaturkürzeln und kontextbewussten Modi.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — macOS-Diktat-App mit On-Device-Spracherkennung und optionaler KI-Nachbearbeitung zur Formatierung.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Desktop-Sprachtranskriptions-App mit Hotkeys, KI-Assistent, Meeting-Diarization und semantischer Suche.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — macOS-Menüleisten-App für Offline-Sprache-zu-Text und Meeting-Zusammenfassungen mit Whisper und Qwen auf Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Plattformübergreifende Tauri-Spracheingabe-App mit lokalem Whisper oder Groq, KI-Bereinigung, Glossar und Sprachassistent.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Plattformübergreifender Sprachdiktat-Assistent mit LLM-Formatierung, unterstützt lokales Whisper, Ollama oder Cloud-APIs.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Plattformübergreifende Tauri-App für KI-Spracheingabe, Textumformulierung und Sprach-Q&A mit globalen Hotkeys.
- [Aria](https://github.com/Xingxun7777/Aria) — Windows-KI-Spracheingabe mit offline Qwen3-ASR, OCR-Kontext, Hotword-Korrektur und Sprachbefehlen.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windows-Sprachdiktat mit whisper.cpp, Groq oder llama.cpp, mehreren Stilen und Auto-Einfügen ins aktive Fenster.
- [localflow](https://github.com/sidharth-n/localflow) — Lokales plattformübergreifendes Sprachdiktat mit Moonshine STT, Qwen3-4B-Polisher, Push-to-Talk und Skip-Gate.
- [yammer](https://github.com/andynu/yammer) — Linux-lokale Sprache-zu-Text mit Whisper und LLM-Bereinigung, plus Tauri-Overlay-UI und xdotool-Eingabeinjektion.

### Lokale/Offline-STT-Engines und Toolkits

Offline-ASR-Engines und Sprachtoolkits zur Integration in Apps: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech und SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Hochleistungsfähige C/C++-Portierung von OpenAI Whisper mit CPU/GPU-Inferenz, Quantisierung und plattformübergreifender Unterstützung.
- [FunASR](https://github.com/modelscope/FunASR) — Industrielles ASR-Toolkit mit Paraformer, SenseVoice, VAD, Diarization, Streaming und OpenAI-kompatibler API.
- [vosk-api](https://github.com/alphacep/vosk-api) — Offline-Spracherkennungs-Toolkit mit kleinen CPU-only-Modellen für 20+ Sprachen und mehrsprachigen Bindings.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Offline-Sprachtoolkit mit next-gen Kaldi und ONNX Runtime für STT, TTS, Sprecher-ID, VAD und mehr.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Umfassendes Sprachtoolkit mit ASR, TTS, Stimmbdruck, Diarization, Übersetzung und Streaming-Services.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Sprachmodell mit ASR für 50+ Sprachen, Emotionen, Audioereignisse und schnelle nicht-autoregressive Inferenz.

### Systemweite Spracheingabe / IME

Systemweit integrierte Spracheingabe-Lösungen, einschließlich Eingabemethoden, IBus/Fcitx-Erweiterungen, Android-IME und iOS-Tastaturen.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android-IME und Spracheingabe-Service mit Whisper für Offline-Spracherkennung und Englisch-Übersetzung.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Offline-Linux-Sprachdiktat-App mit whisper.cpp, Whisper und VOSK-Engines, Vulkan-GPU und GTK-GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — GNOME-Shell-Erweiterung für Offline-Spracheingabe via whisper.cpp mit Hotkey-Trigger, unterstützt X11 und Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Android-Offline-Spracherkennungs-Service mit Vosk und Standard-RecognitionService-API-Unterstützung.
- [Dictus](https://github.com/getdictus/dictus-ios) — Quelloffene iOS-Tastatur für On-Device-Sprachdiktat mit WhisperKit und CoreML, funktioniert in jeder App.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linux-IBus-Sprache-zu-Text-Eingabemethode mit Streaming-STT, optionaler Whisper-Verfeinerung und GPU-Beschleunigung.

### Chinesische Spracheingabe / IME

Projekte optimiert für chinesische Spracherkennung und -eingabe, einschließlich FunASR-, Paraformer- und SenseVoice-basierter chinesischer IMEs und Tastaturen.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Offline-Linux-Chinesisch-Spracheingabe mit FunASR Paraformer, IBus/Fcitx5, PTT-Hotkey und Satzpolishing.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Plattformübergreifende Offline-Spracheingabemethode mit FunASR, Hotword-Korrektur, Auto-Einfügen und GUI/CLI-Modi.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android-Spracheingabe-Tastatur mit 11 ASR-Engines, LLM-Nachbearbeitung, Floating-Ball und Material3-UI.

### Browser und Web-Spracheingabe

Browserbasierte Spracheingabe via Erweiterungen, WebAssembly-Wrappern oder Web-UIs, die typischerweise einen lokalen oder Cloud-STT-Backend benötigen.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio-Whisper-WebUI für Untertitel aus Dateien, YouTube oder Mikrofon, mit VAD, BGM-Trennung und Diarization.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Browser-Erweiterung für Echtzeit-Offline-Sprache-zu-Text via Vosk, mit arabischen und englischen Sprachbefehlen.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Browserbasierte Offline-Spracherkennungs-Bibliothek, die Vosk als WebAssembly in einem WebWorker paketiert.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Browser-Erweiterung und lokaler Whisper-Server für Offline-Sprache-zu-Text in Firefox und Chrome via Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Chrome-Erweiterung, die Sprache via Hotkey aufzeichnet, mit OpenAI Whisper API transkribiert und Text automatisch einfügt.
- [voico](https://github.com/Kirera-Wainaina/voico) — Chrome-Erweiterung für Sprache-zu-Text-Eingabe in Webfelder, mit einem Node.js-Backend, das Google und OpenAI STT nutzt.

### Mobile Spracheingabe (Non-IME)

Eigenständige Sprachtranskriptions-Apps auf Android oder iOS, nicht als Eingabemethoden-Tastaturen.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Private On-Device-Spracherkennungs-Tastatur für Android mit Whisper via whisper.cpp und Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Quelloffene iOS-App für Offline-Sprachtranskription mit Whisper.cpp, mit Aufnahme und Audio-Export.
- [seamless](https://github.com/woheller69/seamless) — Android-Offline-Sprache-zu-Text-Übersetzungs-App mit Meta Seamless M4T Lite für 5 Sprachen mit TTS-Ausgabe.

### Leichtgewichtige Skripte, CLI & Sprachsteuerung

Leichtgewichtige Skripte, CLI-Tools, Tray-Trigger oder Utilities für Entwickler-Integrationen oder als Ergänzung bestehender Toolchains.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linux-Offline-Sprache-zu-Text-Tool, das Vosk nutzt und Tastatureingaben in jede Anwendung simuliert.
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash-Skript für Offline-Spracheingabe via Whisper für TTY, X11, Wayland und WSL mit optionaler LLM-Bearbeitung.
- [hns](https://github.com/primaprashant/hns) — CLI-Tool für lokale Mikrofon-Sprache-zu-Text mit faster-whisper, Zwischenablage-Kopie und stdout-Piping.
- [Elograf](https://github.com/papoteur-mga/elograf) — PyQt6-GUI-Manager für nerd-dictation mit System-Tray, Vosk-Modellen, Eingabesimulation und KDE-Hotkeys.
- [Osprey](https://github.com/osprey-voice/osprey) — Befehlsbasiertes Sprachsteuerungs- und Eingabetool mit Kaldi und Dragonfly für vollständig lokale Spracherkennung.

### Sonstiges

Projekte, die noch keiner Kategorie zugeordnet sind.

- [VoxType](https://github.com/peteonrails/voxtype) — Push-to-Talk-Sprache-zu-Text für Linux und Wayland mit sieben lokalen ASR-Engines, GPU-Unterstützung und Meeting-Modus.

## Open-Source vs. Benchmarks

| Projekt | Preis | Open Source | Erweiterbar | Offline | Chinesisch |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Kostenlos (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: Kostenlos 8K Wörter/Woche; Pro $12/mo jährlich ($30/mo monatlich) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Personal €25 einmalig (BYOK Groq); Pro €5/mo gehostet | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Kostenlos (lokal/BYOK); Pro ¥29/mo oder ¥238.8/Jahr | ❌ | ❌ | ◐ | ◐ |

## Auswahlhilfe

- **Ausgereifte plattformübergreifende Desktop-App** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 Sterne, Whisper/Parakeet offline.
- **Minimale Linux-Offline-Lösung, skriptfähig** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simuliert Tastatureingaben in jede App.
- **STT in eigene App einbetten** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, einbettbar.
- **Chinesische Spracheingabe im Fokus** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; Offline-Linux-Chinesisch-Spracheingabe mit FunASR Paraformer, IBus/Fcitx5, PTT-Hotkey und Satzpolishing.
- **Transkriptions-API/Server selbst hosten** → [FunASR](https://github.com/modelscope/FunASR) — Industrielles ASR-Toolkit mit Paraformer, SenseVoice, VAD, Diarization, Streaming und OpenAI-kompatibler API.

## Mitwirken

Beiträge sind willkommen — siehe [CONTRIBUTING.md](CONTRIBUTING.md). Projekte müssen vollständig Open Source, erweiterbar und leichtgewichtig sein; bitte folge dem Stilguide für Beschreibungen (auf Englisch, eine Zeile, sachlich, kein Marketing-Blabla).

## Star-Verlauf

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Star-Wachstum im Laufe der Zeit für die beliebtesten Projekte in dieser Liste, einschließlich dieses Repositorys.

## Lizenz

[MIT](LICENSE).

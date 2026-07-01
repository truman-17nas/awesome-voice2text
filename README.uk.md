# Awesome Voice Input

> Курирована добірка відкритого програмного забезпечення для голосового введення / диктування — повністю відкритого, розширюваного та легкого. Порівнюється з Typeless, Lazytype та Shandianshuo (闪电说), які є закритими.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Якщо ця добірка корисна, будь ласка, поставте ⭐ репозиторію — це допомагає іншим знайти його.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · **Українська** · [Català](README.ca.md)

## Зміст

- [Бенчмарки (закриті)](#бенчмарки-закриті)
- [Чому цей список](#чому-цей-список)
- [Критерії включення](#критерії-включення)
- [Топ вибір](#топ-вибір)
- [Усі проєкти](#усі-проєкти)
- [Категоризований список](#категоризований-список)
  - [Кросплатформне десктопне диктування в реальному часі](#кросплатформне-десктопне-диктування-в-реальному-часі)
  - [Рідне диктування macOS](#рідне-диктування-macos)
  - [Очищення мовлення ШІ / постобробка LLM](#очищення-мовлення-ші-постобробка-llm)
  - [Локальні/офлайн STT рушії та тулкіти](#локальніофлайн-stt-рушії-та-тулкіти)
  - [Системне голосове введення / IME](#системне-голосове-введення-ime)
  - [Китайське голосове введення / IME](#китайське-голосове-введення-ime)
  - [Голосове введення в браузері та веб](#голосове-введення-в-браузері-та-веб)
  - [Мобільне голосове введення (не IME)](#мобільне-голосове-введення-не-ime)
  - [Легкі скрипти, CLI та голосове керування](#легкі-скрипти-cli-та-голосове-керування)
  - [Інше](#інше)
- [Відкриті продукти vs. бенчмарки](#відкриті-продукти-vs-бенчмарки)
- [Як обрати](#як-обрати)
- [Участь](#участь)
- [Історія Зірок](#історія-зірок)
- [Ліцензія](#ліцензія)

## Бенчмарки (закриті)

| Продукт | Ціноутворення | Платформи | Модель/Рушій | Відкритий код |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Чому цей список

Typeless, Lazytype та Shandianshuo (闪电说) є потужними, але закритими. Цей список збирає відкриті альтернативи, які відповідають трьом критеріям: код повністю публічний, інструмент можна розширювати, і він залишається достатньо легким для роботи на персональному комп'ютері. Зараз він охоплює **75 проєктів у 9 категоріях**, усі перевірені на повну відкритість.

## Критерії включення

- ✅ **Повністю відкритий код** — увесь код у публічному forge (GitHub, GitLab, Codeberg).
- 🔌 **Розширюваність** — ви можете додавати функції, моделі чи інтеграції, які забажаєте.
- ⚡ **Легкість** — мінімум надмірності, швидкий запуск, невеликий слід.

## Топ вибір

🏆 **[Handy](https://github.com/cjpais/Handy)** — Кросплатформний офлайн інструмент перетворення голосу в текст за допомогою Whisper або Parakeet, із глобальними гарячими клавішами та вставкою з буфера обміну. *Флагман спільноти — 25,281 зірок, найбільш доопрацьоване рішення.*

**Fit-5 вибір** (відповідають усім трьом критеріям):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Високопродуктивний C/C++ порт OpenAI Whisper із CPU/GPU інференсом, квантизацією та кросплатформною підтримкою.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Офлайн інструмент перетворення мови в текст для Linux на базі Vosk, який імітує введення з клавіатури в будь-яку програму.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Голосове введення натискай-та-говори для Linux та Wayland із сімома локальними ASR рушіями, підтримкою GPU та режимом нарад.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash скрипт для офлайн голосового введення через Whisper для TTY, X11, Wayland, та WSL із опціональним редагуванням LLM.

## Усі проєкти

| Назва | ⭐ Зірки | Ліцензія | Мова | Fit | Відкритий | Розш. | Легкий | Китайська |
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

## Категоризований список

### Кросплатформне десктопне диктування в реальному часі

Десктопні програми для диктування на базі Whisper для Linux, Windows або кросплатформні, із натискай-та-говори, локальним транскрибуванням та автоматичним введенням.

- [Handy](https://github.com/cjpais/Handy) — Кросплатформний офлайн інструмент перетворення голосу в текст за допомогою Whisper або Parakeet, із глобальними гарячими клавішами та вставкою з буфера обміну.
- [Buzz](https://github.com/chidiwilliams/buzz) — Кросплатформний десктопний GUI для офлайн транскрипції та перекладу Whisper, із прискоренням GPU та живим мікрофоном.
- [Vibe](https://github.com/thewh1teagle/vibe) — Кросплатформна десктопна програма для офлайн транскрибування аудіо та відео за допомогою Whisper, із прискоренням GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Local-first тулкіт програм із Markdown/SQLite сховищем, Yjs CRDT синхронізацією та десктопним інструментом мови в текст.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Рідне для Linux перетворення мови в текст на локальному Whisper та ONNX моделях, хмарних API, інтеграції Waybar, візуалізатор.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Десктопна програма для диктування, що використовує Whisper локально або через API, запускається глобальним гарячим клавішом для введення в активне вікно.
- [Chirp](https://github.com/Whamp/chirp-stt) — Диктування для Windows лише на CPU, що використовує ParakeetV3, із перемиканням гарячою клавішою, вставкою з буфера та перевизначеннями слів.
- [Dabri](https://github.com/AshBuk/dabri) — Офлайн STT програма для Linux на базі whisper.cpp з режимами daemon, CLI та WebSocket для десктопів X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Офлайн програма для нотаток для Linux та Sailfish OS з локальним STT, TTS та перекладом за допомогою кількох рушіїв.
- [voxd](https://github.com/jakovius/voxd) — Десктопне голосове диктування для Linux на базі whisper.cpp для офлайн ASR із введенням ydotool та AI постобробкою.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Офлайн голосове введення для Linux через Whisper, Parakeet або Canary ONNX, із підтримкою X11/Wayland та поліровкою LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Асистент голосового введення для Windows за допомогою гарячої клавіші Caps Lock, із багатопровайдерним STT та опціональним уточненням LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Кросплатформна офлайн програма для диктування на базі distil-whisper, керування гарячими клавішами та опціональним локальним LLM асистентом.
- [TalkType](https://github.com/lmacan1/talktype) — Кросплатформне голосове введення натискай-та-говори за допомогою faster-whisper, із глобальними гарячими клавішами та розумною вставкою.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Офлайн багатомовна програма для диктування за допомогою Faster-Whisper, запускається гарячою клавішою для транскрипції в активне поле.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Локальне голосове диктування для NixOS/Wayland за допомогою whisper.cpp із зворотним зв'язком GTK4 та підтримкою 99 мов.
- [freespeak](https://github.com/Zetaphor/freespeak) — Програма голосового диктування для Linux Wayland із STT, корекцією граматики через LanguageTool та введенням тексту ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Локальний AI десктопний агент, що поєднує голосове диктування, чат LLM, генерацію зображень та голосову автоматизацію.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Десктопне перетворення мови в текст для Windows за допомогою faster-whisper із симуляцією клавіатури, VAD, PTT та пунктуацією.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Голосове диктування Whisper для KDE Wayland із фоновим daemon, systemd сервісом та вставкою з буфера обміну.

### Рідне диктування macOS

Рідні програми диктування для macOS, створені на Swift та WhisperKit, із підтримкою глобальних гарячих клавіш, меню-бару та прискорення Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Програма транскрипції мови для macOS із рушіями Whisper та Parakeet, глобальними гарячими клавішами та пакетним обробленням.
- [Pindrop](https://github.com/watzon/pindrop) — Рідна програма диктування в меню-барі macOS за допомогою WhisperKit для офлайн STT, із гарячими клавішами та опціональним очищенням AI.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Офлайн багатомовний інструмент диктування за допомогою Whisper, запускається гарячою клавішою для транскрипції в будь-яке поле введення.
- [FnKey](https://github.com/evoleinik/fnkey) — Програма в меню-барі macOS, що транскрибує мову через Deepgram Nova-3, поки утримується Fn, і вставляє результат.
- [hush](https://github.com/djmunro/hush) — Програма диктування натискай-та-говори для macOS на локальному Whisper/Parakeet ONNX із автоматичною вставкою через гарячу клавішу.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Програма диктування в меню-барі macOS на офлайн Whisper, із прискоренням Metal GPU та ін'єкцією тексту курсором.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Програма в меню-барі Apple macOS записує при відпусканні Globe/Fn, транскрибує через faster-whisper і вставляє біля курсора.

### Очищення мовлення ШІ / постобробка LLM

Інструменти диктування, що використовують локальні або хмарні LLM для полірування, форматування, узагальнення та перестилізації виходу розпізнавання мови в чистий, формальний текст.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Програма диктування для macOS з локальним та хмарним STT, глобальними гарячими клавішами, AI робочими процесами, плаґінами, REST API та CLI.
- [Amical](https://github.com/amicalhq/amical) — Local-first AI програма диктування, що використовує Whisper для офлайн транскрипції та Ollama для розумного оброблення нотаток.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Офлайн інструмент голосового диктування для macOS/Windows на базі Whisper, із глобальними гарячими клавішами та опціональним покращенням AI.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Local-first голосовий асистент для macOS та Linux із натискай-та-говори, транскрипцією та вилученням плаґінів.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Програма диктування натискай-та-говори для macOS на базі Whisper та очищення LLM, що вставляє полірований текст через Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Локальне голосове диктування з Whisper та поліруванням LLM, натискай-та-говори, словником та клієнт-серверним поділом.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Локальне голосове диктування та запис нарад за допомогою faster-whisper, узагальнень LLM та двоканального запису аудіо.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Рідна програма перетворення голосу в текст для macOS на локальних моделях whisper.cpp, із глобальними скороченнями та контекстно-залежними режимами.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Програма диктування для macOS із розпізнаванням мови на пристрої та опціональним AI постобробленням для форматування.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Десктопна програма транскрипції голосу з гарячими клавішами, AI асистентом, діаризацією нарад та семантичним пошуком.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Програма в меню-барі macOS для офлайн перетворення мови в текст та узагальнення нарад за допомогою Whisper та Qwen на Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Кросплатформна програма голосового введення на Tauri на локальному Whisper або Groq, очищенням AI, глосарієм та голосовим асистентом.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Кросплатформний асистент голосового диктування з форматуванням LLM, що підтримує локальний Whisper, Ollama або хмарні API.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Кросплатформна програма на Tauri для AI голосового введення, переписування тексту та голосових питань-відповідей із глобальними гарячими клавішами.
- [Aria](https://github.com/Xingxun7777/Aria) — AI голосове введення для Windows на офлайн Qwen3-ASR з контекстом OCR, корекцією гарячих слів та голосовими командами.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Голосове диктування для Windows за допомогою whisper.cpp, Groq або llama.cpp, кількох стилів, автоматична вставка в активне вікно.
- [localflow](https://github.com/sidharth-n/localflow) — Локальне кросплатформне голосове диктування за допомогою Moonshine STT, Qwen3-4B полірування, натискай-та-говори та skip-gate.
- [yammer](https://github.com/andynu/yammer) — Локальне перетворення мови в текст для Linux на базі Whisper та очищення LLM, плюс Tauri оверлей UI та ін'єкція введення xdotool.

### Локальні/офлайн STT рушії та тулкіти

Офлайн ASR рушії та мовні тулкіти для інтеграції в додатки: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech та SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Високопродуктивний C/C++ порт OpenAI Whisper із CPU/GPU інференсом, квантизацією та кросплатформною підтримкою.
- [FunASR](https://github.com/modelscope/FunASR) — Промисловий ASR тулкіт із Paraformer, SenseVoice, VAD, діаризацією, стрімінгом та OpenAI-compatible API.
- [vosk-api](https://github.com/alphacep/vosk-api) — Офлайн тулкіт розпізнавання мови з компактними CPU-only моделями для 20+ мов та багатомовними біндингами.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Офлайн мовний тулкіт на базі next-gen Kaldi та ONNX Runtime для STT, TTS, ідентифікації спікера, VAD тощо.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Комплексний мовний тулкіт із ASR, TTS, вокальним відбитком, діаризацією, перекладом та стрімінговими сервісами.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Мовна модель із ASR для 50+ мов, емоцій, аудіоподій та швидким неавторегресійним інференсом.

### Системне голосове введення / IME

Рішення голосового введення інтегровані на системному рівні, включаючи методи введення, розширення IBus/Fcitx, Android IME та iOS клавіатури.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME та сервіс голосового введення на базі Whisper для офлайн розпізнавання мови та англійського перекладу.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Офлайн програма голосового диктування для Linux на рушіях whisper.cpp, Whisper та VOSK, із Vulkan GPU та GTK GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Розширення GNOME Shell для офлайн голосового введення через whisper.cpp із запуском гарячою клавішою, що підтримує X11 та Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Офлайн сервіс розпізнавання мови для Android на базі Vosk з підтримкою стандартного RecognitionService API.
- [Dictus](https://github.com/getdictus/dictus-ios) — Відкрита iOS клавіатура для голосового диктування на пристрої за допомогою WhisperKit та CoreML, працює в будь-якій програмі.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Метод введення мови в текст Linux IBus із потоковим STT, опціональним уточненням Whisper та прискоренням GPU.

### Китайське голосове введення / IME

Проєкти, оптимізовані для китайського розпізнавання та введення мови, включаючи FunASR, Paraformer та SenseVoice на основі китайських IME та клавіатур.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Офлайн китайське голосове введення для Linux на базі FunASR Paraformer, IBus/Fcitx5, PTT гарячої клавіші та поліровки речень.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Кросплатформний офлайн метод голосового введення на базі FunASR, із корекцією гарячих слів, автоматичною вставкою та режимами GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android клавіатура голосового введення з 11 ASR рушіями, LLM постобробкою, плаваючою кнопкою та Material3 UI.

### Голосове введення в браузері та веб

Голосове введення в браузері через розширення, WebAssembly обгортки або веб інтерфейси, яке зазвичай потребує локального або хмарного STT бекенду.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI для субтитрів із файлів, YouTube або мікрофона, із VAD, розділенням BGM та діаризацією.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Розширення браузера для офлайн перетворення мови в текст в реальному часі через Vosk, з арабськими та англійськими голосовими командами.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Бібліотека офлайн розпізнавання мови в браузері, що пакує Vosk як WebAssembly, що працює в WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Розширення браузера та локальний Whisper сервер для офлайн перетворення мови в текст у Firefox та Chrome через Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Розширення Chrome, що записує голос через гарячу клавішу, транскрибує за допомогою OpenAI Whisper API та автоматично вставляє текст.
- [voico](https://github.com/Kirera-Wainaina/voico) — Розширення Chrome для введення голосу в текст у веб-поля, з Node.js бекендом, що використовує Google та OpenAI STT.

### Мобільне голосове введення (не IME)

Автономні програми транскрипції голосу для Android або iOS, а не клавіатури методів введення.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Приватна клавіатура розпізнавання мови на пристрої для Android на базі Whisper через whisper.cpp та Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Відкрита iOS програма для офлайн транскрипції голосу за допомогою Whisper.cpp, із записом та експортом аудіо.
- [seamless](https://github.com/woheller69/seamless) — Офлайн програма перекладу мови в текст для Android на базі Meta Seamless M4T Lite для 5 мов із TTS виходом.

### Легкі скрипти, CLI та голосове керування

Легкі скрипти, CLI інструменти, трейгерти або утиліти, придатні для інтеграції розробником або як доповнення до існуючих тулчейнів.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Офлайн інструмент перетворення мови в текст для Linux на базі Vosk, що імітує введення з клавіатури в будь-яку програму.
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash скрипт для офлайн голосового введення через Whisper для TTY, X11, Wayland, та WSL із опціональним редагуванням LLM.
- [hns](https://github.com/primaprashant/hns) — CLI інструмент для локального мікрофонного перетворення мови в текст за допомогою faster-whisper, із копіюванням у буфер обміну та stdout piping.
- [Elograf](https://github.com/papoteur-mga/elograf) — PyQt6 GUI менеджер для nerd-dictation з системним треєм, моделями Vosk, імітацією введення та гарячими клавішами KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Інструмент голосового керування та введення на основі команд, що використовує Kaldi та Dragonfly для повністю локального розпізнавання мови.

### Інше

Проєкти, які ще не віднесено до категорії.

- [VoxType](https://github.com/peteonrails/voxtype) — Голосове введення натискай-та-говори для Linux та Wayland із сімома локальними ASR рушіями, підтримкою GPU та режимом нарад.

## Відкриті продукти vs. бенчмарки

| Проєкт | Ціна | Відкритий код | Розширюваний | Офлайн | Китайська |
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

## Як обрати

- **Доопрацьована кросплатформна десктопна програма** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 зірок, Whisper/Parakeet офлайн.
- **Мінімальний Linux офлайн, скриптабельний** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, імітує введення з клавіатури в будь-яку програму.
- **Вбудувати STT у власний додаток** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, вбудовуваний.
- **Китайсько-орієнтоване введення** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; Офлайн китайське голосове введення для Linux за допомогою FunASR Paraformer, IBus/Fcitx5, PTT гарячої клавіші та поліровки речень.
- **Self-host транскрипційний API/сервер** → [FunASR](https://github.com/modelscope/FunASR) — Промисловий ASR тулкіт із Paraformer, SenseVoice, VAD, діаризацією, стрімінгом та OpenAI-compatible API.

## Участь

Внесків вітаються — див. [CONTRIBUTING.md](CONTRIBUTING.md). Проєкти мають бути повністю відкритими, розширюваними та легкими; дотримуйтесь гіда щодо стилю описів (англійською, один рядок, фактологічно, без маркетингової балаканини).

## Історія Зірок

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

Зростання кількості зірок з часом для найпопулярніших проєктів у цьому списку. Сам репозиторій є приватним під час рев'ю; власна історія зірок буде додана сюди після того, як він стане публічним.

## Ліцензія

[MIT](LICENSE).

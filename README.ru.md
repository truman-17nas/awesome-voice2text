# Awesome Voice2Text

> Подборка открытых программ для голосового ввода и диктовки — полностью открытых, расширяемых и лёгких. Сравнивается с Typeless, Lazytype и Shandianshuo (闪电说), все из которых закрыты.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Если эта подборка пригодилась, поставьте ⭐ репозиторию — это помогает другим находить его.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · **Русский** · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Содержание

- [Закрытые продукты-эталоны](#закрытые-продукты-эталоны)
- [Почему этот список](#почему-этот-список)
- [Критерии включения](#критерии-включения)
- [Лучший выбор](#лучший-выбор)
- [Все проекты](#все-проекты)
- [Категории](#категории)
  - [Кроссплатформенная диктовка на рабочий стол](#кроссплатформенная-диктовка-на-рабочий-стол)
  - [Нативная macOS диктовка](#нативная-macos-диктовка)
  - [AI-очистка речи / постобработка LLM](#ai-очистка-речи-постобработка-llm)
  - [Локальные офлайн STT-движки и тулкиты](#локальные-офлайн-stt-движки-и-тулкиты)
  - [Системный голосовой ввод / IME](#системный-голосовой-ввод-ime)
  - [Китайский голосовой ввод / IME](#китайский-голосовой-ввод-ime)
  - [Браузерный и веб-голосовой ввод](#браузерный-и-веб-голосовой-ввод)
  - [Мобильный голосовой ввод (не IME)](#мобильный-голосовой-ввод-не-ime)
  - [Лёгкие скрипты, CLI и голосовое управление](#лёгкие-скрипты-cli-и-голосовое-управление)
  - [Прочее](#прочее)
- [Открытые источники против эталонов](#открытые-источники-против-эталонов)
- [Как выбрать](#как-выбрать)
- [Участие](#участие)
- [История Звёзд](#история-звёзд)
- [Лицензия](#лицензия)

## Закрытые продукты-эталоны

| Проект | Цена | Платформы | Модель/движок | Открытый исходный код |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Почему этот список

Typeless, Lazytype и Shandianshuo (闪电说) мощные, но закрыты. Этот список собирает открытые альтернативы, которые соответствуют трём критериям: код полностью публичен, инструмент можно расширять, и он достаточно лёгкий, чтобы работать на персональной машине. Сейчас он охватывает **75 проектов в 9 категориях**, все проверены на полную открытость.

## Критерии включения

- ✅ **Полностью открытый исходный код** — весь код в публичном репозитории (GitHub, GitLab, Codeberg).
- 🔌 **Расширяемость** — вы можете добавлять нужные функции, модели или интеграции.
- ⚡ **Лёгкость** — минимум раздувания, быстрый запуск, небольшой объём.

## Лучший выбор

🏆 **[Handy](https://github.com/cjpais/Handy)** — Кроссплатформенный офлайн инструмент преобразования речи в текст с использованием Whisper или Parakeet, с глобальными горячими клавишами и вставкой из буфера обмена. *Флагман сообщества — 25 281 звезда, самое продуманное решение.*

**Выбор Fit-5** (соответствуют всем трём критериям):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Высокопроизводительный порт OpenAI Whisper на C/C++ с CPU/GPU-инференсом, квантизацией и кроссплатформенной поддержкой.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Офлайн инструмент распознавания речи для Linux с использованием Vosk, имитирующий ввод с клавиатуры в любое приложение.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Push-to-talk голосовой ввод в текст для Linux и Wayland с семью локальными ASR-движками, поддержкой GPU и режимом встреч.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Bash-скрипт для офлайн голосового ввода текста через Whisper для TTY, X11, Wayland и WSL с опциональной LLM-редактурой.

## Все проекты

| Название | ⭐ Звёзды | Лицензия | Язык | Соответствие | Открыт | Расширяем | Лёгкий | Китайский |
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

## Категории

### Кроссплатформенная диктовка на рабочий стол

Десктопные приложения для диктовки на базе Whisper для Linux, Windows или кроссплатформенные, с push-to-talk, локальной транскрипцией и автоматическим вводом.

- [Handy](https://github.com/cjpais/Handy) — Кроссплатформенный офлайн инструмент преобразования речи в текст с использованием Whisper или Parakeet, с глобальными горячими клавишами и вставкой из буфера обмена.
- [Buzz](https://github.com/chidiwilliams/buzz) — Кроссплатформенный десктопный GUI для офлайн транскрипции и перевода Whisper с GPU-ускорением и живым микрофоном.
- [Vibe](https://github.com/thewh1teagle/vibe) — Кроссплатформенное десктопное приложение для офлайн транскрипции аудио и видео с использованием Whisper, с GPU-ускорением.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Local-first тулкит приложений с хранилищем Markdown/SQLite, синхронизацией Yjs CRDT и десктопной утилитой преобразования речи в текст.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Нативная для Linux распознавание речи в текст с локальными моделями Whisper и ONNX, облачными API, интеграцией Waybar и визуализатором.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Десктопное приложение для диктовки, использующее Whisper локально или через API, запускаемое глобальной горячей клавишей для ввода в активное окно.
- [Chirp](https://github.com/Whamp/chirp-stt) — Диктовка для Windows только на CPU с использованием ParakeetV3, с переключением горячей клавишей, вставкой из буфера и переопределением слов.
- [Dabri](https://github.com/AshBuk/dabri) — Офлайн STT-приложение для Linux с использованием whisper.cpp в режимах демона, CLI и WebSocket для десктопов X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Офлайн приложение для заметок для Linux и Sailfish OS с локальными STT, TTS и переводом с использованием нескольких движков.
- [voxd](https://github.com/jakovius/voxd) — Десктопная голосовая диктовка для Linux с использованием whisper.cpp для офлайн ASR с вводом через ydotool и AI-постобработкой.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Офлайн голосовой ввод в Linux через Whisper, Parakeet или Canary ONNX с поддержкой X11/Wayland и LLM-полировкой.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Ассистент голосового ввода для Windows с использованием Caps Lock как горячей клавиши, с мультипровайдерным STT и опциональной LLM-редактурой.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Кроссплатформенное офлайн приложение для диктовки с distil-whisper, управлением горячими клавишами и опциональным локальным LLM-ассистентом.
- [TalkType](https://github.com/lmacan1/talktype) — Кроссплатформенный push-to-talk голосовой ввод с использованием faster-whisper, с глобальными горячими клавишами и умной вставкой.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Офлайн многоязычное приложение для диктовки с использованием Faster-Whisper, запускаемое горячей клавишей для транскрипции в активное поле.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Локальная голосовая диктовка для NixOS/Wayland с использованием whisper.cpp с GTK4-интерфейсом и поддержкой 99 языков.
- [freespeak](https://github.com/Zetaphor/freespeak) — Приложение для голосовой диктовки на Linux Wayland с STT, исправлением грамматики через LanguageTool и вводом текста через ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Локальный AI-десктопный агент, сочетающий голосовую диктовку, LLM-чат, генерацию изображений и голосовую автоматизацию.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Десктопная распознавание речи в текст для Windows с использованием faster-whisper, симуляцией клавиатуры, VAD, PTT и пунктуацией.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Голосовая диктовка Whisper для KDE Wayland с фоновым демоном, systemd-сервисом и вставкой из буфера обмена.

### Нативная macOS диктовка

Нативные приложения для диктовки на macOS, созданные на Swift и WhisperKit, поддерживающие глобальные горячие клавиши, меню-бар и ускорение на Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — macOS-приложение для транскрипции речи с движками Whisper и Parakeet, глобальными горячими клавишами и пакетной обработкой.
- [Pindrop](https://github.com/watzon/pindrop) — Нативное macOS-приложение для диктовки из меню-бара с использованием WhisperKit для офлайн STT, с горячими клавишами и опциональной AI-очисткой.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Офлайн многоязычный инструмент для диктовки с использованием Whisper, запускаемый горячей клавишей для транскрипции в любое поле ввода.
- [FnKey](https://github.com/evoleinik/fnkey) — macOS-приложение из меню-бара, которое транскрибирует речь через Deepgram Nova-3 при удержании Fn и вставляет результат.
- [hush](https://github.com/djmunro/hush) — macOS push-to-talk приложение для диктовки с использованием локальных ONNX-моделей Whisper/Parakeet и автовставкой через горячую клавишу.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — macOS-приложение для диктовки из меню-бара с использованием офлайн Whisper и GPU-ускорения Metal, с вставкой текста в позицию курсора.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — macOS-приложение из меню-бара записывает при отпускании Globe/Fn, транскрибирует через faster-whisper и вставляет в позицию курсора.

### AI-очистка речи / постобработка LLM

Инструменты диктовки, использующие локальные или облачные LLM для полировки, форматирования, суммаризации и переработки результата распознавания речи в чистый, формальный текст.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — macOS-приложение для диктовки с локальным и облачным STT, глобальными горячими клавишами, AI-воркфлоу, плагинами, REST API и CLI.
- [Amical](https://github.com/amicalhq/amical) — Local-first AI-приложение для диктовки с использованием Whisper для офлайн транскрипции и Ollama для умной обработки заметок.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Офлайн инструмент голосовой диктовки для macOS/Windows с использованием Whisper, с глобальными горячими клавишами и опциональным AI-улучшением.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Local-first голосовой ассистент для macOS и Linux с push-to-talk, транскрипцией и извлечением плагинов.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — macOS push-to-talk приложение для диктовки с использованием Whisper и LLM-очистки, вставляющее полированный текст через Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Локальная голосовая диктовка с Whisper и LLM-полировкой, push-to-talk, словарём и клиент-серверной архитектурой.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Локальная голосовая диктовка и записывающий встречи с faster-whisper, LLM-резюме и двухдорожечным аудиозахватом.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Нативное macOS-приложение преобразования речи в текст с использованием локальных моделей whisper.cpp, с глобальными ярлыками и контекстно-зависимыми режимами.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — macOS-приложение для диктовки с локальным распознаванием речи и опциональной AI-постобработкой для форматирования.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Десктопное приложение для транскрипции речи с горячими клавишами, AI-ассистентом, диаризацией встреч и семантическим поиском.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — macOS-приложение из меню-бара для офлайн преобразования речи в текст и суммаризации встреч с использованием Whisper и Qwen на Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Кроссплатформенное Tauri-приложение голосового ввода с локальным Whisper или Groq, AI-очисткой, глоссарием и голосовым ассистентом.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Кроссплатформенный голосовой ассистент диктовки с LLM-форматированием, поддерживающий локальный Whisper, Ollama или облачные API.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Кроссплатформенное Tauri-приложение для AI-голосового ввода, переписывания текста и голосового Q&A с глобальными горячими клавишами.
- [Aria](https://github.com/Xingxun7777/Aria) — AI-голосовой ввод для Windows с использованием офлайн Qwen3-ASR с OCR-контекстом, коррекцией ключевых слов и голосовыми командами.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Голосовая диктовка для Windows с использованием whisper.cpp, Groq или llama.cpp, несколькими стилями и автовставкой в активное окно.
- [localflow](https://github.com/sidharth-n/localflow) — Локальная кроссплатформенная голосовая диктовка с использованием Moonshine STT, Qwen3-4B полировщика, push-to-talk и skip-gate.
- [yammer](https://github.com/andynu/yammer) — Локальное распознавание речи в текст для Linux с Whisper и LLM-очисткой, плюс Tauri-оверлей UI и инжекция ввода через xdotool.

### Локальные офлайн STT-движки и тулкиты

Офлайн ASR-движки и речевые тулкиты для интеграции в приложения: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech и SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Высокопроизводительный порт OpenAI Whisper на C/C++ с CPU/GPU-инференсом, квантизацией и кроссплатформенной поддержкой.
- [FunASR](https://github.com/modelscope/FunASR) — Промышленный ASR-тулкит с Paraformer, SenseVoice, VAD, диаризацией, стримингом и OpenAI-совместимым API.
- [vosk-api](https://github.com/alphacep/vosk-api) — Офлайн тулкит распознавания речи с небольшими CPU-only моделями для 20+ языков и мультиязычными биндингами.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Офлайн речевой тулкит с использованием next-gen Kaldi и ONNX Runtime для STT, TTS, идентификации говорящего, VAD и др.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Комплексный речевой тулкит с ASR, TTS, голосовым отпечатком, диаризацией, переводом и стриминговыми сервисами.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Речевая модель с ASR для 50+ языков, эмоций, аудиособытий и быстрым неавторегрессионным инференсом.

### Системный голосовой ввод / IME

Решения для голосового ввода, интегрированные на уровне системы, включая методы ввода, расширения IBus/Fcitx, Android IME и iOS-клавиатуры.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME и сервис голосового ввода с использованием Whisper для офлайн распознавания речи и английского перевода.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Офлайн приложение голосовой диктовки для Linux с движками whisper.cpp, Whisper и VOSK, Vulkan GPU и GTK GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Расширение GNOME Shell для офлайн голосового ввода через whisper.cpp с горячей клавишей, поддерживающее X11 и Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Офлайн сервис распознавания речи для Android с использованием Vosk с поддержкой стандартного RecognitionService API.
- [Dictus](https://github.com/getdictus/dictus-ios) — Открытая iOS-клавиатура для локальной голосовой диктовки с использованием WhisperKit и CoreML, работает в любом приложении.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Метод ввода Linux IBus speech-to-text со стримингом STT, опциональной Whisper-редактурой и GPU-ускорением.

### Китайский голосовой ввод / IME

Проекты, оптимизированные для китайского распознавания речи и ввода, включая китайские IME и клавиатуры на базе FunASR, Paraformer и SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Офлайн китайский голосовой ввод для Linux с использованием FunASR Paraformer, IBus/Fcitx5, PTT-горячей клавишей и полировкой предложений.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Кроссплатформенный офлайн метод голосового ввода с использованием FunASR, с коррекцией ключевых слов, автовставкой и режимами GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android-клавиатура голосового ввода с 11 ASR-движками, LLM-постобработкой, плавающей кнопкой и Material3 UI.

### Браузерный и веб-голосовой ввод

Браузерный голосовой ввод через расширения, WebAssembly-обёртки или веб-интерфейсы, обычно требующие локального или облачного STT-бэкенда.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI для субтитров из файлов, YouTube или микрофона, с VAD, разделением BGM и диаризацией.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Браузерное расширение для офлайн распознавания речи в реальном времени через Vosk, с голосовыми командами на арабском и английском.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Браузерная офлайн библиотека распознавания речи, упаковывающая Vosk как WebAssembly, работающую в WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Браузерное расширение и локальный Whisper-сервер для офлайн распознавания речи в Firefox и Chrome через Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Расширение Chrome, которое записывает голос по горячей клавише, транскрибирует с помощью OpenAI Whisper API и автоматически вставляет текст.
- [voico](https://github.com/Kirera-Wainaina/voico) — Расширение Chrome для голосового ввода текста в веб-поля, с Node.js-бэкендом, использующим Google и OpenAI STT.

### Мобильный голосовой ввод (не IME)

Автономные приложения для голосовой транскрипции на Android или iOS, а не клавиатуры методов ввода.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Приватная клавиатура распознавания речи на устройстве для Android с использованием Whisper через whisper.cpp и Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Открытое iOS-приложение для офлайн голосовой транскрипции с использованием Whisper.cpp, с записью и экспортом аудио.
- [seamless](https://github.com/woheller69/seamless) — Офлайн Android-приложение для распознавания речи и перевода с использованием Meta Seamless M4T Lite для 5 языков с TTS-выводом.

### Лёгкие скрипты, CLI и голосовое управление

Лёгкие скрипты, инструменты CLI, трей-триггеры или утилиты, подходящие для интеграции разработчиками или как дополнения к существующим тулчейнам.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Офлайн инструмент распознавания речи для Linux с использованием Vosk, имитирующий ввод с клавиатуры в любое приложение.
- [voice_typing](https://github.com/themanyone/voice_typing) — Bash-скрипт для офлайн голосового ввода текста через Whisper для TTY, X11, Wayland и WSL с опциональной LLM-редактурой.
- [hns](https://github.com/primaprashant/hns) — CLI-инструмент для локального распознавания речи с микрофона с использованием faster-whisper, с копированием в буфер обмена и piping в stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — PyQt6 GUI-менеджер для nerd-dictation с системным треем, моделями Vosk, симуляцией ввода и KDE-горячими клавишами.
- [Osprey](https://github.com/osprey-voice/osprey) — Инструмент голосового управления и ввода на основе команд с использованием Kaldi и Dragonfly для полностью локального распознавания речи.

### Прочее

Проекты, ещё не отнесённые к категории.

- [VoxType](https://github.com/peteonrails/voxtype) — Push-to-talk голосовой ввод в текст для Linux и Wayland с семью локальными ASR-движками, поддержкой GPU и режимом встреч.

## Открытые источники против эталонов

| Проект | Цена | Открытый исходный код | Расширяемость | Офлайн | Китайский |
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

## Как выбрать

- **Полированное кроссплатформенное десктопное приложение** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25 281 звезда, офлайн Whisper/Parakeet.
- **Минималистичный офлайн для Linux, скриптуемый** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, имитирует ввод с клавиатуры в любое приложение.
- **Встраивайте STT в своё приложение** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, встраиваемый.
- **Китайский ввод в приоритете** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; офлайн китайский голосовой ввод для Linux с использованием FunASR Paraformer, IBus/Fcitx5, PTT-горячей клавишей и полировкой предложений.
- **Самохостинг транскрипционного API/сервера** → [FunASR](https://github.com/modelscope/FunASR) — Промышленный ASR-тулкит с Paraformer, SenseVoice, VAD, диаризацией, стримингом и OpenAI-совместимым API.

## Участие

Вклады приветствуются — см. [CONTRIBUTING.md](CONTRIBUTING.md). Проекты должны быть полностью открытыми, расширяемыми и легковесными; пожалуйста, следуйте гиду по стилю описаний (на английском, одна строка, фактологически, без маркетинговой трепотни).

## История Звёзд

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Динамика роста звёзд со временем для самых популярных проектов из этого списка, включая этот репозиторий.

## Лицензия

[MIT](LICENSE).

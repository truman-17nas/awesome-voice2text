# Awesome Voice Input

> Daftar perangkat lunak input suara / dikte sumber terbuka yang dikurator — sepenuhnya terbuka, dapat diperluas, dan ringan. Dibandingkan dengan Typeless, Lazytype, dan Shandianshuo (闪电说), yang semuanya bersumber tertutup.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Jika daftar ini berguna, silakan ⭐ repo ini — ini membantu orang lain menemukannya.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · **Bahasa Indonesia** · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Daftar Isi

- [Benchmark (Sumber Tertutup)](#benchmark-sumber-tertutup)
- [Mengapa Daftar Ini](#mengapa-daftar-ini)
- [Kriteria Penyertaan](#kriteria-penyertaan)
- [Pilihan Utama](#pilihan-utama)
- [Semua Proyek](#semua-proyek)
- [Daftar Terkategori](#daftar-terkategori)
  - [Dikte Desktop Lintas Platform Secara Real-Time](#dikte-desktop-lintas-platform-secara-real-time)
  - [Dikte macOS Asli](#dikte-macos-asli)
  - [Pembersihan Ucapan AI / Pasca-Pemrosesan LLM](#pembersihan-ucapan-ai-pasca-pemrosesan-llm)
  - [Mesin dan Toolkit STT Lokal/Offline](#mesin-dan-toolkit-stt-lokaloffline)
  - [Input Suara Tingkat Sistem / IME](#input-suara-tingkat-sistem-ime)
  - [Input Ucapan Mandarin / IME](#input-ucapan-mandarin-ime)
  - [Input Suara Peramban & Web](#input-suara-peramban-web)
  - [Input Suara Seluler (Non-IME)](#input-suara-seluler-non-ime)
  - [Skrip Ringan, CLI & Kontrol Suara](#skrip-ringan-cli-kontrol-suara)
  - [Lainnya](#lainnya)
- [Sumber Terbuka vs. Benchmark](#sumber-terbuka-vs-benchmark)
- [Cara Memilih](#cara-memilih)
- [Kontribusi](#kontribusi)
- [Riwayat Bintang](#riwayat-bintang)
- [Lisensi](#lisensi)

## Benchmark (Sumber Tertutup)

| Produk | Harga | Platform | Model/Mesin | Sumber Terbuka |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Gratis 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | API AI cloud (proprietari) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo pada Groq; whisper.cpp lokal | ❌ |
| Shandianshuo (闪电说) | Gratis (lokal/BYOK); Pro ¥29/mo atau ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (lokal) + ASR cloud | ❌ |

## Mengapa Daftar Ini

Typeless, Lazytype, dan Shandianshuo (闪电说) sangat kuat tetapi bersumber tertutup. Daftar ini mengumpulkan alternatif sumber terbuka yang memenuhi tiga kriteria: kode sepenuhnya publik, alat dapat diperluas, dan tetap ringan hingga dapat berjalan di mesin pribadi. Saat ini mencakup **75 proyek dalam 9 kategori**, semuanya telah diverifikasi sepenuhnya sumber terbuka.

## Kriteria Penyertaan

- ✅ **Sepenuhnya sumber terbuka** — seluruh kode di forge publik (GitHub, GitLab, Codeberg).
- 🔌 **Dapat diperluas** — Anda dapat menambahkan fitur, model, atau integrasi yang Anda inginkan.
- ⚡ **Ringan** — minimal pemborosan, startup cepat, jejak kecil.

## Pilihan Utama

🏆 **[Handy](https://github.com/cjpais/Handy)** — Alat suara-ke-teks lintas platform secara offline menggunakan Whisper atau Parakeet, dengan hotkey global dan tempel papan klip. *Unggulan komunitas — 25,281 bintang, tawaran paling matang.*

**Pilihan Fit-5** (memenuhi ketiga kriteria):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Port C/C++ berkinerja tinggi dari OpenAI Whisper dengan inferensi CPU/GPU, kuantisasi, dan dukungan lintas platform.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Alat Linux offline suara-ke-teks menggunakan Vosk yang mensimulasikan input keyboard ke aplikasi apa pun.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Suara-ke-teks push-to-talk untuk Linux dan Wayland dengan tujuh mesin ASR lokal, dukungan GPU, dan mode rapat.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Skrip Bash untuk pengetik suara offline melalui Whisper untuk TTY, X11, Wayland, dan WSL dengan pengeditan LLM opsional.

## Semua Proyek

| Nama | ⭐ Bintang | Lisensi | Bahasa | Cocok | Terbuka | Dapat Diperluas | Ringan | Mandarin |
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
| [Speechfire](https://github.com/Jejkobb/Speechfire) | 27 | Tidak ada | JavaScript, Python | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
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

## Daftar Terkategori

### Dikte Desktop Lintas Platform Secara Real-Time

Aplikasi dikte desktop berbasis Whisper untuk Linux, Windows, atau lintas platform, dengan push-to-talk, transkripsi lokal, dan input otomatis.

- [Handy](https://github.com/cjpais/Handy) — Alat suara-ke-teks lintas platform secara offline menggunakan Whisper atau Parakeet, dengan hotkey global dan tempel papan klip.
- [Buzz](https://github.com/chidiwilliams/buzz) — GUI desktop lintas platform untuk transkripsi dan terjemahan Whisper offline dengan akselerasi GPU, mikrofon langsung.
- [Vibe](https://github.com/thewh1teagle/vibe) — Aplikasi desktop lintas platform untuk transkripsi audio dan video offline menggunakan Whisper, dengan akselerasi GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Toolkit aplikasi local-first dengan penyimpanan Markdown/SQLite, sinkronisasi Yjs CRDT, dan utilitas suara-ke-teks desktop.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Suara-ke-teks native Linux dengan Whisper lokal dan model ONNX, API cloud, integrasi Waybar, visualizer.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Aplikasi dikte desktop menggunakan Whisper secara lokal atau melalui API, dipicu oleh hotkey global untuk mengetik ke jendela aktif.
- [Chirp](https://github.com/Whamp/chirp-stt) — Aplikasi dikte Windows hanya-CPU menggunakan ParakeetV3, dengan toggle hotkey, tempel papan klip, dan penggantian kata.
- [Dabri](https://github.com/AshBuk/dabri) — Aplikasi STT offline Linux menggunakan whisper.cpp dengan mode daemon, CLI, dan WebSocket untuk desktop X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Aplikasi pencatatan offline untuk Linux dan Sailfish OS dengan STT lokal, TTS, dan terjemahan menggunakan berbagai mesin.
- [voxd](https://github.com/jakovius/voxd) — Dikte suara desktop Linux menggunakan whisper.cpp untuk ASR offline dengan pengetikan ydotool dan pasca-pemrosesan AI.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Pengetik suara offline Linux melalui Whisper, Parakeet, atau Canary ONNX, dengan dukungan X11/Wayland dan polesan LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Asisten pengetik suara Windows menggunakan tombol Caps Lock, dengan STT multi-penyedia dan penyempurnaan LLM opsional.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Aplikasi dikte offline lintas platform dengan distil-whisper, kontrol hotkey, dan asisten LLM lokal opsional.
- [TalkType](https://github.com/lmacan1/talktype) — Pengetik suara push-to-talk lintas platform menggunakan faster-whisper, dengan hotkey global dan tempel pintar.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Aplikasi dikte multibahasa offline menggunakan Faster-Whisper, dipicu oleh hotkey untuk mentranskripsi ke bidang aktif.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Dikte suara lokal NixOS/Wayland menggunakan whisper.cpp dengan umpan balik GTK4 dan dukungan 99 bahasa.
- [freespeak](https://github.com/Zetaphor/freespeak) — Aplikasi dikte suara Linux Wayland dengan STT, koreksi tata bahasa melalui LanguageTool, dan input teks ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agen desktop AI lokal yang menggabungkan dikte suara, chat LLM, pembuatan gambar, dan otomasi berbasis suara.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Suara-ke-teks desktop Windows menggunakan faster-whisper dengan simulasi keyboard, VAD, PTT, dan tanda baca.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dikte suara Whisper untuk KDE Wayland dengan daemon latar belakang, layanan systemd, dan tempel papan klip.

### Dikte macOS Asli

Aplikasi dikte macOS asli yang dibangun dengan Swift dan WhisperKit, mendukung hotkey global, menu bar, dan akselerasi Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Aplikasi transkripsi suara macOS dengan mesin Whisper dan Parakeet, hotkey global, dan pemrosesan batch.
- [Pindrop](https://github.com/watzon/pindrop) — Aplikasi dikte menu-bar macOS asli menggunakan WhisperKit untuk STT offline, dengan hotkey dan pembersihan AI opsional.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Alat dikte multibahasa offline menggunakan Whisper, dipicu oleh hotkey untuk mentranskripsi ke bidang input apa pun.
- [FnKey](https://github.com/evoleinik/fnkey) — Aplikasi menu-bar macOS yang mentranskripsi ucapan melalui Deepgram Nova-3 saat Fn ditahan dan menempel hasilnya.
- [hush](https://github.com/djmunro/hush) — Aplikasi dikte push-to-talk macOS menggunakan Whisper/Parakeet ONNX lokal dengan tempel otomatis melalui hotkey.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Aplikasi dikte menu-bar macOS menggunakan Whisper offline dengan akselerasi GPU Metal dan injeksi teks kursor.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Aplikasi menu-bar Apple macOS merekam saat Globe/Fn dilepas, mentranskripsi melalui faster-whisper, dan menempel di kursor.

### Pembersihan Ucapan AI / Pasca-Pemrosesan LLM

Alat dikte yang menggunakan LLM lokal atau cloud untuk memoles, memformat, merangkum, dan menata ulang output pengenalan suara menjadi teks bersih dan formal.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Aplikasi dikte macOS dengan STT pada perangkat dan cloud, hotkey global, alur kerja AI, plugin, REST API, dan CLI.
- [Amical](https://github.com/amicalhq/amical) — Aplikasi dikte AI local-first menggunakan Whisper untuk transkripsi offline dan Ollama untuk pemrosesan catatan pintar.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Alat dikte suara offline untuk macOS/Windows menggunakan Whisper, dengan hotkey global dan peningkatan AI opsional.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Asisten suara local-first untuk macOS dan Linux dengan push-to-talk, transkripsi, dan ekstraksi plugin.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Aplikasi dikte push-to-talk macOS menggunakan Whisper dan pembersihan LLM, menempel teks yang dipoles melalui Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Dikte suara lokal dengan pemolesan Whisper dan LLM, push-to-talk, kamus, dan pemisahan klien-server.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Dikte suara lokal dan perekam rapat dengan faster-whisper, ringkasan LLM, dan penangkapan audio dual-track.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Aplikasi suara-ke-teks macOS asli menggunakan model whisper.cpp lokal, dengan pintasan global dan mode yang sadar konteks.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Aplikasi dikte macOS dengan pengenalan suara pada perangkat dan pasca-pemrosesan AI opsional untuk pemformatan.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Aplikasi transkripsi suara desktop dengan hotkey, asisten AI, diarisasi rapat, dan pencarian semantik.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Aplikasi menu-bar macOS untuk suara-ke-teks offline dan ringkasan rapat menggunakan Whisper dan Qwen di Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Aplikasi pengetik suara Tauri lintas platform dengan Whisper lokal atau Groq, pembersihan AI, glosarium, dan asisten suara.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Asisten dikte suara lintas platform dengan pemformatan LLM, mendukung Whisper lokal, Ollama, atau API cloud.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Aplikasi Tauri lintas platform untuk pengetik suara AI, penulisan ulang teks, dan tanya-jawab suara dengan hotkey global.
- [Aria](https://github.com/Xingxun7777/Aria) — Input suara AI Windows menggunakan Qwen3-ASR offline dengan konteks OCR, koreksi kata panas, dan perintah suara.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Dikte suara Windows menggunakan whisper.cpp, Groq, atau llama.cpp, beberapa gaya, tempel otomatis ke jendela aktif.
- [localflow](https://github.com/sidharth-n/localflow) — Dikte suara lintas platform lokal menggunakan Moonshine STT, penoles Qwen3-4B, push-to-talk, dan skip-gate.
- [yammer](https://github.com/andynu/yammer) — Suara-ke-teks lokal Linux dengan Whisper dan pembersihan LLM, ditambah UI overlay Tauri dan injeksi input xdotool.

### Mesin dan Toolkit STT Lokal/Offline

Mesin ASR offline dan toolkit pidato untuk integrasi aplikasi: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech, dan SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Port C/C++ berkinerja tinggi dari OpenAI Whisper dengan inferensi CPU/GPU, kuantisasi, dan dukungan lintas platform.
- [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industri dengan Paraformer, SenseVoice, VAD, diarisasi, streaming, dan API yang kompatibel dengan OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Toolkit pengenalan suara offline dengan model hanya-CPU kecil untuk 20+ bahasa dan binding multi-bahasa.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Toolkit pidato offline menggunakan Kaldi generasi berikutnya dan ONNX Runtime untuk STT, TTS, ID pembicara, VAD, dan lainnya.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Toolkit pidato komprehensif dengan ASR, TTS, sidik suara, diarisasi, terjemahan, dan layanan streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Model pidato dengan ASR untuk 50+ bahasa, emosi, peristiwa audio, dan inferensi non-autoregresif cepat.

### Input Suara Tingkat Sistem / IME

Solusi input suara yang terintegrasi di tingkat sistem, termasuk metode input, ekstensi IBus/Fcitx, IME Android, dan keyboard iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android dan layanan input suara menggunakan Whisper untuk pengenalan suara offline dan terjemahan bahasa Inggris.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Aplikasi dikte suara Linux offline dengan mesin whisper.cpp, Whisper, dan VOSK, GPU Vulkan, dan GUI GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Ekstensi GNOME Shell untuk input suara offline melalui whisper.cpp dengan pemicu hotkey, mendukung X11 dan Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Layanan pengenalan suara offline Android menggunakan Vosk dengan dukungan API RecognitionService standar.
- [Dictus](https://github.com/getdictus/dictus-ios) — Keyboard iOS sumber terbuka untuk dikte suara pada perangkat menggunakan WhisperKit dan CoreML, berfungsi di aplikasi apa pun.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Metode input suara-ke-teks IBus Linux dengan streaming STT, penyempurnaan Whisper opsional, dan akselerasi GPU.

### Input Ucapan Mandarin / IME

Proyek yang dioptimalkan untuk pengenalan dan input ucapan Mandarin, termasuk IME dan keyboard berbasis FunASR, Paraformer, dan SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Input suara Mandarin Linux offline menggunakan FunASR Paraformer, IBus/Fcitx5, hotkey PTT, dan pemolesan kalimat.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Metode input suara offline lintas platform menggunakan FunASR, dengan koreksi hotword, tempel otomatis, dan mode GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Keyboard input suara Android dengan 11 mesin ASR, pasca-pemrosesan LLM, floating ball, dan UI Material3.

### Input Suara Peramban & Web

Input suara berbasis peramban melalui ekstensi, pembungkus WebAssembly, atau Web UI, yang biasanya memerlukan backend STT lokal atau cloud.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI untuk subtitle dari file, YouTube, atau mikrofon, dengan VAD, pemisahan BGM, dan diarisasi.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Ekstensi peramban untuk suara-ke-teks offline real-time melalui Vosk, dengan perintah suara bahasa Arab dan Inggris.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Library pengenalan suara offline berbasis peramban yang mengemas Vosk sebagai WebAssembly yang berjalan di WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Ekstensi peramban dan server Whisper lokal untuk suara-ke-teks offline di Firefox dan Chrome melalui Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Ekstensi Chrome yang merekam suara melalui hotkey, mentranskripsi dengan OpenAI Whisper API, dan menempel teks secara otomatis.
- [voico](https://github.com/Kirera-Wainaina/voico) — Ekstensi Chrome untuk input suara-ke-teks ke bidang web, dengan backend Node.js menggunakan Google dan OpenAI STT.

### Input Suara Seluler (Non-IME)

Aplikasi transkripsi suara mandiri di Android atau iOS, bukan keyboard metode input.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Keyboard pengenalan suara pribadi pada perangkat untuk Android menggunakan Whisper melalui whisper.cpp dan Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Aplikasi iOS sumber terbuka untuk transkripsi suara offline menggunakan Whisper.cpp, dengan perekaman dan ekspor audio.
- [seamless](https://github.com/woheller69/seamless) — Aplikasi terjemahan suara-ke-teks offline Android menggunakan Meta Seamless M4T Lite untuk 5 bahasa dengan output TTS.

### Skrip Ringan, CLI & Kontrol Suara

Skrip ringan, alat CLI, pemicu tray, atau utilitas yang cocok untuk integrasi pengembang atau sebagai pelengkap toolchain yang ada.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Alat Linux offline suara-ke-teks menggunakan Vosk yang mensimulasikan input keyboard ke aplikasi apa pun.
- [voice_typing](https://github.com/themanyone/voice_typing) — Skrip Bash untuk pengetik suara offline melalui Whisper untuk TTY, X11, Wayland, dan WSL dengan pengeditan LLM opsional.
- [hns](https://github.com/primaprashant/hns) — Alat CLI untuk mikrofon lokal suara-ke-teks menggunakan faster-whisper, dengan salinan papan klip dan piping stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Manajer GUI PyQt6 untuk nerd-dictation dengan system tray, model Vosk, simulasi input, dan hotkey KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Alat kontrol suara dan pengetik berbasis perintah menggunakan Kaldi dan Dragonfly untuk pengenalan suara sepenuhnya lokal.

### Lainnya

Proyek yang belum ditetapkan ke kategori.

- [VoxType](https://github.com/peteonrails/voxtype) — Suara-ke-teks push-to-talk untuk Linux dan Wayland dengan tujuh mesin ASR lokal, dukungan GPU, dan mode rapat.

## Sumber Terbuka vs. Benchmark

| Proyek | Harga | Sumber Terbuka | Dapat Diperluas | Offline | Mandarin |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Gratis (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Gratis (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Gratis (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(tertutup)* | Freemium: Gratis 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(tertutup)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(tertutup)* | Gratis (lokal/BYOK); Pro ¥29/mo atau ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Cara Memilih

- **Aplikasi desktop lintas platform yang matang** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 bintang, Whisper/Parakeet offline.
- **Linux offline minimal, dapat diskrip** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, mensimulasikan input keyboard ke aplikasi apa pun.
- **Tanamkan STT di aplikasi Anda sendiri** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Whisper C/C++, CPU/GPU, dapat ditanam.
- **Input Mandarin utama** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; Input suara Mandarin Linux offline menggunakan FunASR Paraformer, IBus/Fcitx5, hotkey PTT, dan pemolesan kalimat.
- **Self-host API/server transkripsi** → [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industri dengan Paraformer, SenseVoice, VAD, diarisasi, streaming, dan API yang kompatibel dengan OpenAI.

## Kontribusi

Kontribusi sangat welcome — lihat [CONTRIBUTING.md](CONTRIBUTING.md). Proyek harus sepenuhnya sumber terbuka, dapat diperluas, dan ringan; harap ikuti panduan gaya deskripsi (bahasa Inggris, satu baris, faktual, tanpa jargon pemasaran).

Kontribusi diterima dengan senang hati — silakan lihat [CONTRIBUTING.md](CONTRIBUTING.md). Proyek harus sepenuhnya sumber terbuka, dapat diperluas, dan ringan; harap ikuti panduan gaya deskripsi (bahasa Inggris, satu baris, faktual, tanpa jargon pemasaran).

## Riwayat Bintang

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

Pertumbuhan bintang dari waktu ke waktu untuk proyek dengan bintang terbanyak di daftar ini. Repo itu sendiri bersifat pribadi selama peninjauan; riwayat bintangnya akan ditambahkan di sini setelah dipublikasikan.

## Lisensi

[MIT](LICENSE).

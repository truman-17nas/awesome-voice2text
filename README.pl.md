# Awesome Voice Input

> Wyselekcjonowana lista otwartego oprogramowania do wprowadzania głosem / dyktowania — w pełni otwarte, rozszerzalne i lekkie. Zestawiona w porównaniu z Typeless, Lazytype i Shandianshuo (闪电说), które są zamkniętoźródłowe.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Jeśli ta lista jest przydatna, zostaw ⭐ w repozytorium — pomoże to innym ją znaleźć.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · **Polski** · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Spis treści

- [Benchmarki (zamkniętoźródłowe)](#benchmarki-zamkniętoźródłowe)
- [Dlaczego ta lista](#dlaczego-ta-lista)
- [Kryteria wyboru](#kryteria-wyboru)
- [Najlepsze wybory](#najlepsze-wybory)
- [Wszystkie projekty](#wszystkie-projekty)
- [Lista kategorii](#lista-kategorii)
  - [Wieloplatformowe dyktowanie pulpitu w czasie rzeczywistym](#wieloplatformowe-dyktowanie-pulpitu-w-czasie-rzeczywistym)
  - [Natywne dyktowanie macOS](#natywne-dyktowanie-macos)
  - [Oczyszczanie mowy przez AI / przetwarzanie końcowe LLM](#oczyszczanie-mowy-przez-ai-przetwarzanie-końcowe-llm)
  - [Lokalne/offline'owe silniki STT i zestawy narzędziowe](#lokalneofflineowe-silniki-stt-i-zestawy-narzędziowe)
  - [Wprowadzanie głosem na poziomie systemu / IME](#wprowadzanie-głosem-na-poziomie-systemu-ime)
  - [Chińskie wprowadzanie głosem / IME](#chińskie-wprowadzanie-głosem-ime)
  - [Wprowadzanie głosem w przeglądarce i sieci](#wprowadzanie-głosem-w-przeglądarce-i-sieci)
  - [Mobilne wprowadzanie głosem (inne niż IME)](#mobilne-wprowadzanie-głosem-inne-niż-ime)
  - [Lekkie skrypty, CLI i sterowanie głosem](#lekkie-skrypty-cli-i-sterowanie-głosem)
  - [Inne](#inne)
- [Otwarte źródło vs. benchmarki](#otwarte-źródło-vs-benchmarki)
- [Jak wybrać](#jak-wybrać)
- [Współtworzenie](#współtworzenie)
- [Historia Gwiazd](#historia-gwiazd)
- [Licencja](#licencja)

## Benchmarki (zamkniętoźródłowe)

| Produkt | Cena | Platformy | Model/Silnik | Otwarte źródło |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Dlaczego ta lista

Typeless, Lazytype i Shandianshuo (闪电说) są potężne, ale zamkniętoźródłowe. Ta lista gromadzi otwarte alternatywy, które spełniają trzy kryteria: kod jest w pełni publiczny, narzędzie można rozszerzać, a jednocześnie jest na tyle lekkie, by działać na osobistej maszynie. Obecnie obejmuje **75 projektów w 9 kategoriach**, wszystkie zweryfikowane jako w pełni otwarte źródło.

## Kryteria wyboru

- ✅ **W pełni otwarte źródło** — cały kod w publicznej platformie (GitHub, GitLab, Codeberg).
- 🔌 **Rozszerzalne** — możesz dodawać funkcje, modele lub integracje, które chcesz.
- ⚡ **Lekkie** — minimalna nadmiarowość, szybki start, mały ślad.

## Najlepsze wybory

🏆 **[Handy](https://github.com/cjpais/Handy)** — Wieloplatformowe offline'owe narzędzie głos-na-tekst używające Whisper lub Parakeet, z globalnymi skrótami klawiszowymi i wklejaniem ze schowka. *Flagowa pozycja społeczności — 25,281 stars, najbardziej dopracowana propozycja.*

**Wybory fit=5** (spełniają wszystkie trzy kryteria):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Wysokowydajny port C/C++ OpenAI Whisper z inferencją CPU/GPU, kwantyzacją i wieloplatformowym wsparciem.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linuxowe offline'owe narzędzie głos-na-tekst używające Vosk, symulujące wprowadzanie klawiatury do dowolnej aplikacji.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Głos-na-tekst typu push-to-talk dla Linux i Wayland z siedmioma lokalnymi silnikami ASR, wsparciem GPU i trybem spotkań.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Skrypt Bash do offline'owego pisania głosem przez Whisper dla TTY, X11, Wayland i WSL z opcjonalną edycją LLM.

## Wszystkie projekty

| Nazwa | ⭐ Stars | Licencja | Język | Fit | Open | Ext | LW | Chinese |
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

## Lista kategorii

### Wieloplatformowe dyktowanie pulpitu w czasie rzeczywistym

Aplikacje do dyktowania na pulpicie oparte na Whisper dla Linux, Windows lub wieloplatformowe, z push-to-talk, lokalną transkrypcją i automatycznym wprowadzaniem tekstu.

- [Handy](https://github.com/cjpais/Handy) — Wieloplatformowe offline'owe narzędzie głos-na-tekst używające Whisper lub Parakeet, z globalnymi skrótami klawiszowymi i wklejaniem ze schowka.
- [Buzz](https://github.com/chidiwilliams/buzz) — Wieloplatformowe GUI dla offline'owej transkrypcji i tłumaczenia Whisper z akceleracją GPU i mikrofonem na żywo.
- [Vibe](https://github.com/thewh1teagle/vibe) — Wieloplatformowa aplikacja desktopowa do offline'owej transkrypcji audio i wideo za pomocą Whisper, z akceleracją GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Zestaw narzędzi aplikacji local-first z przechowywaniem Markdown/SQLite, synchronizacją Yjs CRDT i narzędziem głos-na-tekst.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linuxowe głos-na-tekst z lokalnym Whisper i modelami ONNX, chmurowymi API, integracją Waybar i wizualizerem.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Aplikacja do dyktowania używająca Whisper lokalnie lub przez API, wywoływana globalnym skrótem, która wpisuje tekst do aktywnego okna.
- [Chirp](https://github.com/Whamp/chirp-stt) — Dyktowanie na Windows tylko na CPU używające ParakeetV3, z przełącznikiem hotkey, wklejaniem ze schowka i nadpisywaniem słów.
- [Dabri](https://github.com/AshBuk/dabri) — Linuxowa offline'owa aplikacja STT używająca whisper.cpp z daemonem, CLI i trybami WebSocket dla pulpitów X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linuxowa i Sailfish OS aplikacja do notatek offline z lokalnym STT, TTS i tłumaczeniem używająca wielu silników.
- [voxd](https://github.com/jakovius/voxd) — Linuxowe desktopowe dyktowanie głosem używające whisper.cpp do offline'owego ASR z ydotool i przetwarzaniem końcowym AI.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Linuxowe offline'owe pisanie głosem przez Whisper, Parakeet lub Canary ONNX, z obsługą X11/Wayland i wygładzaniem przez LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Windowsowy asystent pisania głosem używający klawisza Caps Lock, z wieloma dostawcami STT i opcjonalnym wykończeniem LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Wieloplatformowa offline'owa aplikacja do dyktowania z distil-whisper, sterowaniem hotkey i opcjonalnym lokalnym asystentem LLM.
- [TalkType](https://github.com/lmacan1/talktype) — Wieloplatformowe pisanie głosem typu push-to-talk używające faster-whisper, z globalnymi skrótami i inteligentnym wklejaniem.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Wielojęzyczna aplikacja do dyktowania offline używająca Faster-Whisper, wywoływana hotkey do transkrypcji w aktywnym polu.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Lokalne dyktowanie głosem dla NixOS/Wayland używające whisper.cpp z interfejsem GTK4 i obsługą 99 języków.
- [freespeak](https://github.com/Zetaphor/freespeak) — Linuxowa Waylandowa aplikacja do dyktowania głosem z STT, poprawą gramatyki przez LanguageTool i wprowadzaniem tekstu przez ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Lokalny agent desktopowy AI łączący dyktowanie głosem, czat LLM, generowanie obrazów i automatyzację sterowaną głosem.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windowsowa desktopowa aplikacja głos-na-tekst używająca faster-whisper z symulacją klawiatury, VAD, PTT i interpunkcją.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dyktowanie głosem Whisper dla KDE Wayland z daemonem w tle, usługą systemd i wklejaniem ze schowka.

### Natywne dyktowanie macOS

Natywne aplikacje do dyktowania macOS zbudowane w Swift i WhisperKit, obsługujące globalne skróty klawiszowe, pasek menu i akcelerację Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — macOS aplikacja do transkrypcji mowy z silnikami Whisper i Parakeet, globalnymi skrótami i przetwarzaniem wsadowym.
- [Pindrop](https://github.com/watzon/pindrop) — Natywna macOS menu-barowa aplikacja do dyktowania używająca WhisperKit do offline'owego STT, z hotkeyami i opcjonalnym czyszczeniem AI.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Offline'owe wielojęzyczne narzędzie do dyktowania używające Whisper, wywoływane hotkey do transkrypcji w dowolnym polu tekstowym.
- [FnKey](https://github.com/evoleinik/fnkey) — macOS menu-barowa aplikacja, która transkrybuje mowę przez Deepgram Nova-3 podczas przytrzymywania Fn i wkleja wynik.
- [hush](https://github.com/djmunro/hush) — macOS push-to-talk dyktowanie używające lokalnego Whisper/Parakeet ONNX z auto-wklejaniem przez hotkey.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — macOS menu-barowa aplikacja do dyktowania używająca offline'owego Whisper z akceleracją Metal GPU i wstrzykiwaniem tekstu przy kursorze.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS menu-barowa aplikacja nagrywająca po zwolnieniu Globe/Fn, transkrybująca przez faster-whisper i wklejająca przy kursorze.

### Oczyszczanie mowy przez AI / przetwarzanie końcowe LLM

Narzędzia do dyktowania używające lokalnych lub chmurowych LLM do polerowania, formatowania, podsumowywania i restrylizowania wyników rozpoznawania mowy w czysty, formalny tekst.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — macOS aplikacja do dyktowania z on-device i chmurowym STT, globalnymi skrótami, przepływami AI, wtyczkami, REST API i CLI.
- [Amical](https://github.com/amicalhq/amical) — Local-first aplikacja AI do dyktowania używająca Whisper do offline'owej transkrypcji i Ollama do inteligentnego przetwarzania notatek.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Offline'owe narzędzie do dyktowania głosem dla macOS/Windows używające Whisper, z globalnymi skrótami i opcjonalnym wzbogacaniem AI.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Local-first asystent głosowy dla macOS i Linux z push-to-talk, transkrypcją i ekstrakcją przez wtyczki.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — macOS push-to-talk dyktowanie używające Whisper i czyszczenia LLM, wklejające wypolerowany tekst przez Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Lokalne dyktowanie głosem z Whisper i polerowaniem LLM, push-to-talk, słownikiem i podziałem klient-serwer.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Lokalne dyktowanie głosem i rejestrator spotkań z faster-whisper, podsumowaniami LLM i dwutorowym przechwytywaniem audio.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Natywna macOS aplikacja głos-na-tekst używająca lokalnych modeli whisper.cpp, z globalnymi skrótami i trybami świadomymi kontekstu.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — macOS aplikacja do dyktowania z on-device rozpoznawaniem mowy i opcjonalnym przetwarzaniem końcowym AI do formatowania.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Desktopowa aplikacja do transkrypcji głosu z hotkeyami, asystentem AI, diarizacją spotkań i semantycznym wyszukiwaniem.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — macOS menu-barowa aplikacja do offline'owego głos-na-tekst i podsumowań spotkań używająca Whisper i Qwen na Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Wieloplatformowa Tauri aplikacja do pisania głosem z lokalnym Whisper lub Groq, czyszczeniem AI, glosariuszem i asystentem głosowym.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Wieloplatformowy asystent do dyktowania głosem z formatowaniem LLM, obsługą lokalnego Whisper, Ollama lub chmurowych API.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Wieloplatformowa Tauri aplikacja do AI pisania głosem, przepisywania tekstu i głosowych Q&A z globalnymi skrótami.
- [Aria](https://github.com/Xingxun7777/Aria) — Windowsowe AI wprowadzanie głosem używające offline'owego Qwen3-ASR z kontekstem OCR, poprawką hot word i komendami głosowymi.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windowsowe dyktowanie głosem używające whisper.cpp, Groq lub llama.cpp, wieloma stylami i auto-wklejaniem do aktywnego okna.
- [localflow](https://github.com/sidharth-n/localflow) — Wieloplatformowe lokalne dyktowanie głosem używające Moonshine STT, Qwen3-4B polisher, push-to-talk i skip-gate.
- [yammer](https://github.com/andynu/yammer) — Linuxowe lokalne głos-na-tekst z Whisper i czyszczeniem LLM, plus Tauri nakładka UI i wstrzykiwanie xdotool.

### Lokalne/offline'owe silniki STT i zestawy narzędziowe

Offline'owe silniki ASR i zestawy narzędziowe mowy do integracji z aplikacjami: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech i SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Wysokowydajny port C/C++ OpenAI Whisper z inferencją CPU/GPU, kwantyzacją i wieloplatformowym wsparciem.
- [FunASR](https://github.com/modelscope/FunASR) — Przemysłowy zestaw narzędzi ASR z Paraformer, SenseVoice, VAD, diarizacją, strumieniowaniem i API kompatybilnym z OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Offline'owy zestaw narzędzi do rozpoznawania mowy z małymi modelami tylko CPU dla 20+ języków i powiązaniami wielojęzycznymi.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Offline'owy zestaw narzędzi mowy używający nowej generacji Kaldi i ONNX Runtime do STT, TTS, identyfikacji mówcy, VAD i innych.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Kompleksowy zestaw narzędzi mowy z ASR, TTS, voiceprint, diarizacją, tłumaczeniem i usługami strumieniowymi.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Model mowy z ASR dla 50+ języków, emocji, zdarzeń audio i szybką inferencją nieautoregresyjną.

### Wprowadzanie głosem na poziomie systemu / IME

Rozwiązania wprowadzania głosem zintegrowane na poziomie systemu, w tym metody wprowadzania, rozszerzenia IBus/Fcitx, IME Androida i klawiatury iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME i usługa wprowadzania głosem używająca Whisper do offline'owego rozpoznawania mowy i tłumaczenia na angielski.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Offline'owa Linuxowa aplikacja do dyktowania głosem z silnikami whisper.cpp, Whisper i VOSK, GPU Vulkan i GTK GUI.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Rozszerzenie GNOME Shell do offline'owego wprowadzania głosem przez whisper.cpp z hotkey, obsługujące X11 i Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Androidowa offline'owa usługa rozpoznawania mowy używająca Vosk ze standardowym wsparciem RecognitionService API.
- [Dictus](https://github.com/getdictus/dictus-ios) — Otwarta iOS klawiatura do on-device dyktowania głosem używająca WhisperKit i CoreML, działająca w dowolnej aplikacji.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linuxowa IBus metoda wprowadzania głos-na-tekst ze strumieniowym STT, opcjonalnym wykończeniem Whisper i akceleracją GPU.

### Chińskie wprowadzanie głosem / IME

Projekty zoptymalizowane pod chińskie rozpoznawanie mowy i wprowadzanie tekstu, w tym chińskie IME i klawiatury oparte na FunASR, Paraformer i SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Offline'owe chińskie wprowadzanie głosem w Linux używające FunASR Paraformer, IBus/Fcitx5, hotkey PTT i polerowania zdań.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Wieloplatformowa offline'owa metoda wprowadzania głosem używająca FunASR, z poprawką hotword, auto-wklejaniem i trybami GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Androidowa klawiatura wprowadzania głosem z 11 silnikami ASR, przetwarzaniem końcowym LLM, pływającą kulą i Material3 UI.

### Wprowadzanie głosem w przeglądarce i sieci

Wprowadzanie głosem w przeglądarce poprzez rozszerzenia, opakowania WebAssembly lub interfejsy sieciowe, zazwyczaj wymagające lokalnego lub chmurowego backendu STT.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI do napisów z plików, YouTube lub mikrofonu, z VAD, separacją BGM i diarizacją.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Rozszerzenie przeglądarki do offline'owego głos-na-tekst w czasie rzeczywistym przez Vosk, z arabskimi i angielskimi komendami głosowymi.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Biblioteka do offline'owego rozpoznawania mowy w przeglądarce pakująca Vosk jako WebAssembly działający w WebWorkerze.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Rozszerzenie przeglądarki i lokalny serwer Whisper do offline'owego głos-na-tekst w Firefox i Chrome przez Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Rozszerzenie Chrome nagrywające głos przez hotkey, transkrybujące przez OpenAI Whisper API i auto-wklejające tekst.
- [voico](https://github.com/Kirera-Wainaina/voico) — Rozszerzenie Chrome do wprowadzania głos-na-tekst w pola sieciowe, z backendem Node.js używającym Google i OpenAI STT.

### Mobilne wprowadzanie głosem (inne niż IME)

Samodzielne aplikacje do transkrypcji głosu na Androida lub iOS, a nie klawiatury metod wprowadzania.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Prywatna klawiatura rozpoznawania mowy on-device dla Androida używająca Whisper przez whisper.cpp i Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Otwarta iOS aplikacja do offline'owej transkrypcji głosu używająca Whisper.cpp, z nagrywaniem i eksportem audio.
- [seamless](https://github.com/woheller69/seamless) — Androidowa offline'owa aplikacja tłumaczenia głos-na-tekst używająca Meta Seamless M4T Lite dla 5 języków z wyjściem TTS.

### Lekkie skrypty, CLI i sterowanie głosem

Lekkie skrypty, narzędzia CLI, wyzwalacze zasobnika lub narzędzia przydatne do integracji deweloperskiej lub jako uzupełnienie istniejących łańcuchów narzędzi.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linuxowe offline'owe narzędzie głos-na-tekst używające Vosk, symulujące wprowadzanie klawiatury do dowolnej aplikacji.
- [voice_typing](https://github.com/themanyone/voice_typing) — Skrypt Bash do offline'owego pisania głosem przez Whisper dla TTY, X11, Wayland i WSL z opcjonalną edycją LLM.
- [hns](https://github.com/primaprashant/hns) — Narzędzie CLI do lokalnego mikrofonowego głos-na-tekst używające faster-whisper, z kopiowaniem do schowka i przekierowaniem do stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — GUI menedżer PyQt6 dla nerd-dictation z zasobnikiem systemowym, modelami Vosk, symulacją wprowadzania i hotkeyami KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Narzędzie do sterowania głosem i pisania oparte na komendach używające Kaldi i Dragonfly do w pełni lokalnego rozpoznawania mowy.

### Inne

Projekty jeszcze nie przypisane do kategorii.

- [VoxType](https://github.com/peteonrails/voxtype) — Linux i Wayland push-to-talk głos-na-tekst z siedmioma lokalnymi silnikami ASR, wsparciem GPU i trybem spotkań.

## Otwarte źródło vs. benchmarki

| Projekt | Cena | Otwarte źródło | Rozszerzalne | Offline | Chiński |
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

## Jak wybrać

- **Dopracowana wieloplatformowa aplikacja desktopowa** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 stars, Whisper/Parakeet offline.
- **Minimalny Linux offline, skryptowalny** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, symuluje wprowadzanie klawiatury do dowolnej aplikacji.
- **Osadź STT we własnej aplikacji** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, możliwy do osadzenia.
- **Wprowadzanie z naciskiem na chiński** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; offline'owe chińskie wprowadzanie głosem w Linux używające FunASR Paraformer, IBus/Fcitx5, hotkey PTT i polerowania zdań.
- **Samodzielnie hostuj API/server transkrypcji** → [FunASR](https://github.com/modelscope/FunASR) — Przemysłowy zestaw narzędzi ASR z Paraformer, SenseVoice, VAD, diarizacją, strumieniowaniem i API kompatybilnym z OpenAI.

## Współtworzenie

Wkłady są mile widziane — zobacz [CONTRIBUTING.md](CONTRIBUTING.md). Projekty muszą być w pełni open source, rozszerzalne i lekkie; postępuj zgodnie z przewodnikiem stylu opisów (po angielsku, jedna linia, rzeczowo, bez marketingowego bełkotu).

## Historia Gwiazd

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

Wzrost liczby gwiazd na przestrzeni czasu dla najbardziej popularnych projektów na tej liście. Repozytorium jest prywatne podczas przeglądu; jego historia gwiazd zostanie tu dodana, gdy stanie się publiczne.

## Licencja

[MIT](LICENSE).

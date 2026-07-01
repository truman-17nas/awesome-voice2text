# Awesome Voice2Text

> Una llista curada de programari d'entrada de veu / dictat de codi obert — totalment obert, extensible i lleuger. Comparada amb Typeless, Lazytype i Shandianshuo (闪电说), tots els quals són de codi tancat.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Si aquesta llista és útil, si us plau, fes ⭐ al repo — això ajuda altres persones a trobar-lo.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · **Català**

## Contingut

- [Comparativa (de codi tancat)](#comparativa-de-codi-tancat)
- [Per què aquesta llista](#per-què-aquesta-llista)
- [Criteris d'inclusió](#criteris-dinclusió)
- [Selecció destacada](#selecció-destacada)
- [Tots els projectes](#tots-els-projectes)
- [Llista per categories](#llista-per-categories)
  - [Dictat d'escriptori en temps real multiplataforma](#dictat-descriptori-en-temps-real-multiplataforma)
  - [Dictat natiu per a macOS](#dictat-natiu-per-a-macos)
  - [Neteja de veu amb IA / postprocessament amb LLM](#neteja-de-veu-amb-ia-postprocessament-amb-llm)
  - [Motors i eines STT locals / sense connexió](#motors-i-eines-stt-locals-sense-connexió)
  - [Entrada de veu a nivell de sistema / IME](#entrada-de-veu-a-nivell-de-sistema-ime)
  - [Entrada de veu en xinès / IME](#entrada-de-veu-en-xinès-ime)
  - [Entrada de veu per a navegador i web](#entrada-de-veu-per-a-navegador-i-web)
  - [Entrada de veu mòbil (no IME)](#entrada-de-veu-mòbil-no-ime)
  - [Scripts lleugers, CLI i control per veu](#scripts-lleugers-cli-i-control-per-veu)
  - [Altres](#altres)
- [Codi obert vs. comparativa](#codi-obert-vs-comparativa)
- [Com triar](#com-triar)
- [Contribucions](#contribucions)
- [Historial d'Estrelles](#historial-destrelles)
- [Llicència](#llicència)

## Comparativa (de codi tancat)

| Producte | Preu | Plataformes | Model/Motor | Codi obert |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Per què aquesta llista

Typeless, Lazytype i Shandianshuo (闪电说) són poderosos però de codi tancat. Aquesta llista recopila alternatives de codi obert que compleixen tres criteris: el codi és totalment públic, l'eina es pot ampliar i és prou lleugera per executar-se en una màquina personal. Actualment cobreix **75 projectes en 9 categories**, tots verificats com a totalment de codi obert.

## Criteris d'inclusió

- ✅ **Totalment de codi obert** — tot el codi en una forja pública (GitHub, GitLab, Codeberg).
- 🔌 **Extensible** — pots afegir les funcions, models o integracions que vulguis.
- ⚡ **Lleuger** — sense excés de pes, arrencada ràpida i petita petjada.

## Selecció destacada

🏆 **[Handy](https://github.com/cjpais/Handy)** — Eina de veu a text multiplataforma i sense connexió que utilitza Whisper o Parakeet, amb dreceres globals i enganxament al porta-retalls. *Bandera de la comunitat — 25,281 estrelles, l'oferta més acabada.*

**Selecció Fit-5** (complexen els tres criteris):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Port d'altes prestacions del Whisper d'OpenAI en C/C++ amb inferència CPU/GPU, quantització i suport multiplataforma.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Eina de veu a text fora de línia per a Linux que utilitza Vosk i simula l'entrada de teclat a qualsevol aplicació.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Veut a text amb botó per parlar per a Linux i Wayland amb set motors ASR locals, suport de GPU i mode de reunions.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Script Bash per a l'escriptura de veu fora de línia mitjançant Whisper per a TTY, X11, Wayland i WSL amb edició opcional per LLM.

## Tots els projectes

| Nom | ⭐ Estrelles | Llicència | Llenguatge | Aptitud | Obert | Extensible | Lleuger | Xinès |
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

## Llista per categories

### Dictat d'escriptori en temps real multiplataforma

Aplicacions de dictat d'escriptori basades en Whisper per a Linux, Windows o multiplataforma, amb botó per parlar, transcripció local i entrada automàtica.

- [Handy](https://github.com/cjpais/Handy) — Eina de veu a text multiplataforma i sense connexió que utilitza Whisper o Parakeet, amb dreceres globals i enganxament al porta-retalls.
- [Buzz](https://github.com/chidiwilliams/buzz) — Interfície gràfica d'escriptori multiplataforma per a la transcripció i traducció fora de línia amb Whisper, acceleració per GPU i micròfon en viu.
- [Vibe](https://github.com/thewh1teagle/vibe) — Aplicació d'escriptori multiplataforma per a la transcripció d'àudio i vídeo fora de línia mitjançant Whisper, amb acceleració per GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Kit d'eines d'aplicacions local-first amb emmagatzematge Markdown/SQLite, sincronització Yjs CRDT i una utilitat d'escriptori de veu a text.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Veut a text natiu per a Linux amb models Whisper i ONNX locals, APIs al núvol, integració amb Waybar i visualitzador.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Aplicació de dictat d'escriptori que utilitza Whisper localment o mitjançant API, activada per una drecera global per escriure a la finestra activa.
- [Chirp](https://github.com/Whamp/chirp-stt) — Aplicació de dictat només per a CPU de Windows que utilitza ParakeetV3, amb activació per drecera, enganxament al porta-retalls i substitucions de paraules.
- [Dabri](https://github.com/AshBuk/dabri) — Aplicació STT fora de línia per a Linux que utilitza whisper.cpp amb modes dimoni, CLI i WebSocket per a escriptoris X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Aplicació de notes fora de línia per a Linux i Sailfish OS amb STT local, TTS i traducció mitjançant diversos motors.
- [voxd](https://github.com/jakovius/voxd) — Dictat de veu d'escriptori per a Linux que utilitza whisper.cpp per a ASR fora de línia amb escriptura per ydotool i postprocessament amb IA.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Escriptura de veu fora de línia per a Linux mitjançant Whisper, Parakeet o Canary ONNX, amb suport X11/Wayland i retoc per LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Assistència d'escriptura de veu per a Windows que utilitza la tecla de bloqueig de majúscules com a drecera, amb STT de diversos proveïdors i refinament opcional per LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Aplicació de dictat fora de línia multiplataforma amb distil-whisper, control per dreceres i assistent local opcional per LLM.
- [TalkType](https://github.com/lmacan1/talktype) — Escriptura de veu amb botó per parlar multiplataforma que utilitza faster-whisper, amb dreceres globals i enganxament intel·ligent.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Aplicació de dictat multilingüe fora de línia que utilitza Faster-Whisper, activada per drecera per transcriure al camp actiu.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Dictat de veu local per a NixOS/Wayland que utilitza whisper.cpp amb retroalimentació GTK4 i suport per a 99 idiomes.
- [freespeak](https://github.com/Zetaphor/freespeak) — Aplicació de dictat de veu per a Linux Wayland amb STT, correcció gramatical mitjançant LanguageTool i entrada de text per ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agent d'escriptori d'IA local que combina dictat de veu, xat per LLM, generació d'imatges i automatització controlada per veu.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Veut a text d'escriptori per a Windows que utilitza faster-whisper amb simulació de teclat, VAD, PTT i puntuació.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dictat de veu per a Whisper per a KDE Wayland amb dimoni en segon pla, servei systemd i enganxament al porta-retalls.

### Dictat natiu per a macOS

Aplicacions de dictat nadius per a macOS fetes amb Swift i WhisperKit, amb suport per a dreceres globals, barra de menús i acceleració per Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Aplicació de transcripció de veu per a macOS amb motors Whisper i Parakeet, dreceres globals i processament per lots.
- [Pindrop](https://github.com/watzon/pindrop) — Aplicació de dictat nativa a la barra de menús de macOS que utilitza WhisperKit per a STT fora de línia, amb dreceres i neteja opcional per IA.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Eina de dictat multilingüe fora de línia que utilitza Whisper, activada per drecera per transcriure a qualsevol camp d'entrada.
- [FnKey](https://github.com/evoleinik/fnkey) — Aplicació de la barra de menús de macOS que transcriu la veu mitjançant Deepgram Nova-3 mentre es manté premida la tecla Fn i enganxa el resultat.
- [hush](https://github.com/djmunro/hush) — Aplicació de dictat amb botó per parlar per a macOS que utilitza Whisper/Parakeet ONNX locals amb enganxament automàtic per drecera.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Aplicació de dictat a la barra de menús de macOS que utilitza Whisper fora de línia amb acceleració GPU Metal i injecció de text al cursor.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Aplicació de la barra de menús d'Apple macOS que enregistra en alliberar Globe/Fn, transcriu mitjançant faster-whisper i enganxa al cursor.

### Neteja de veu amb IA / postprocessament amb LLM

Eines de dictat que utilitzen LLM locals o al núvol per polir, formatar, resumir i reestilitzar la sortida del reconeixement de veu en text net i formal.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Aplicació de dictat per a macOS amb STT al dispositiu i al núvol, dreceres globals, fluxos de treball d'IA, connectors, API REST i CLI.
- [Amical](https://github.com/amicalhq/amical) — Aplicació de dictat d'IA local-first que utilitza Whisper per a la transcripció fora de línia i Ollama per al processament intel·ligent de notes.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Eina de dictat de veu fora de línia per a macOS/Windows que utilitza Whisper, amb dreceres globals i millora opcional per IA.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Assistent de veu local-first per a macOS i Linux amb botó per parlar, transcripció i extracció per connectors.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Aplicació de dictat amb botó per parlar per a macOS que utilitza Whisper i neteja per LLM, enganxant text poliment via Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Dictat de veu local amb poliment per Whisper i LLM, botó per parlar, diccionari i divisió client-servidor.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Dictat de veu local i enregistrador de reunions amb faster-whisper, resums per LLM i captura d'àudio de doble pista.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Aplicació de veu a text nativa per a macOS que utilitza models whisper.cpp locals, amb dreceres globals i modes sensibles al context.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Aplicació de dictat per a macOS amb reconeixement de veu al dispositiu i postprocessament opcional per IA per al format.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Aplicació d'escriptori de transcripció de veu amb dreceres, assistent d'IA, diarització de reunions i cerca semàntica.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Aplicació de la barra de menús de macOS per a veu a text fora de línia i resums de reunions utilitzant Whisper i Qwen en Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Aplicació d'escriptura de veu multiplataforma en Tauri amb Whisper local o Groq, neteja per IA, glossari i assistent de veu.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Assistent de dictat de veu multiplataforma amb format per LLM, compatible amb Whisper local, Ollama o APIs al núvol.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Aplicació multiplataforma en Tauri per a escriptura de veu amb IA, reescriptura de text i preguntes i respostes per veu amb dreceres globals.
- [Aria](https://github.com/Xingxun7777/Aria) — Entrada de veu amb IA per a Windows que utilitza Qwen3-ASR fora de línia amb context OCR, correcció per paraula clau i ordres per veu.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Dictat de veu per a Windows que utilitza whisper.cpp, Groq o llama.cpp, diversos estils i enganxament automàtic a la finestra activa.
- [localflow](https://github.com/sidharth-n/localflow) — Dictat de veu local multiplataforma que utilitza Moonshine STT, polidor Qwen3-4B, botó per parlar i skip-gate.
- [yammer](https://github.com/andynu/yammer) — Veut a text local per a Linux amb Whisper i neteja per LLM, més interfície de superposició Tauri i injecció d'entrada per xdotool.

### Motors i eines STT locals / sense connexió

Motors ASR fora de línia i eines de veu per a la integració en aplicacions: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech i SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Port d'altes prestacions del Whisper d'OpenAI en C/C++ amb inferència CPU/GPU, quantització i suport multiplataforma.
- [FunASR](https://github.com/modelscope/FunASR) — Kit d'eines ASR industrial amb Paraformer, SenseVoice, VAD, diarització, streaming i API compatible amb OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Kit d'eines de reconeixement de veu fora de línia amb petits models només per a CPU per a més de 20 idiomes i bindings multillenguatge.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Kit d'eines de veu fora de línia que utilitza Kaldi de nova generació i ONNX Runtime per a STT, TTS, identificació d'altaveus, VAD i més.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Kit d'eines de veu complet amb ASR, TTS, empremta de veu, diarització, traducció i serveis de streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Model de veu amb ASR per a més de 50 idiomes, emoció, esdeveniments d'àudio i inferència ràpida no autoregressiva.

### Entrada de veu a nivell de sistema / IME

Solucions d'entrada de veu integrades a nivell de sistema, incloent mètodes d'entrada, extensions IBus/Fcitx, IME d'Android i teclats d'iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME d'Android i servei d'entrada de veu que utilitza Whisper per al reconeixement de veu fora de línia i la traducció a l'anglès.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Aplicació de dictat de veu fora de línia per a Linux amb motors whisper.cpp, Whisper i VOSK, GPU Vulkan i interfície GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Extensió del GNOME Shell per a l'entrada de veu fora de línia mitjançant whisper.cpp amb activador per drecera, compatible amb X11 i Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Servei de reconeixement de veu fora de línia per a Android que utilitza Vosk amb suport de l'API estàndard RecognitionService.
- [Dictus](https://github.com/getdictus/dictus-ios) — Teclat iOS de codi obert per a dictat de veu al dispositiu que utilitza WhisperKit i CoreML, funciona a qualsevol aplicació.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Mètode d'entrada de veu a text IBus per a Linux amb STT en streaming, refinament opcional per Whisper i acceleració per GPU.

### Entrada de veu en xinès / IME

Projectes optimitzats per al reconeixement i entrada de veu en xinès, incloent IME i teclats xinesos basats en FunASR, Paraformer i SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Entrada de veu xinesa fora de línia per a Linux que utilitza FunASR Paraformer, IBus/Fcitx5, drecera PTT i poliment de frases.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Mètode d'entrada de veu fora de línia multiplataforma que utilitza FunASR, amb correcció per paraula clau, enganxament automàtic i modes GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Teclat d'entrada de veu per a Android amb 11 motors ASR, postprocessament per LLM, bola flotant i interfície Material3.

### Entrada de veu per a navegador i web

Entrada de veu basada en navegador mitjançant extensions, embolcalls WebAssembly o interfícies web, que normalment requereix un backend STT local o al núvol.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — WebUI de Whisper en Gradio per a subtítols de fitxers, YouTube o micròfon, amb VAD, separació de BGM i diarització.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Extensió de navegador per a veu a text en temps real fora de línia mitjançant Vosk, amb ordres de veu en àrab i anglès.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Biblioteca de reconeixement de veu fora de línia basada en navegador que empaqueta Vosk com a WebAssembly executant-se en un WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Extensió de navegador i servidor local Whisper per a veu a text fora de línia a Firefox i Chrome mitjançant Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Extensió de Chrome que enregistra veu mitjançant drecera, transcriu amb l'API d'OpenAI Whisper i enganxa el text automàticament.
- [voico](https://github.com/Kirera-Wainaina/voico) — Extensió de Chrome per a l'entrada de veu a text als camps web, amb un backend Node.js que utilitza STT de Google i OpenAI.

### Entrada de veu mòbil (no IME)

Aplicacions independents de transcripció de veu per a Android o iOS, en lloc de teclats de mètodes d'entrada.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Teclat de reconeixement de veu privat al dispositiu per a Android que utilitza Whisper mitjançant whisper.cpp i Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Aplicació iOS de codi obert per a la transcripció de veu fora de línia utilitzant Whisper.cpp, amb enregistrament i exportació d'àudio.
- [seamless](https://github.com/woheller69/seamless) — Aplicació de traducció de veu a text fora de línia per a Android que utilitza Meta Seamless M4T Lite per a 5 idiomes amb sortida TTS.

### Scripts lleugers, CLI i control per veu

Scripts lleugers, eines CLI, activadors de safata o utilitats adequades per a la integració de desenvolupadors o com a suplements a cadenes d'eines existents.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Eina de veu a text fora de línia per a Linux que utilitza Vosk i simula l'entrada de teclat a qualsevol aplicació.
- [voice_typing](https://github.com/themanyone/voice_typing) — Script Bash per a l'escriptura de veu fora de línia mitjançant Whisper per a TTY, X11, Wayland i WSL amb edició opcional per LLM.
- [hns](https://github.com/primaprashant/hns) — Eina CLI per a veu a text local des del micròfon utilitzant faster-whisper, amb còpia al porta-retalls i canalització a stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Gestor d'interfície PyQt6 per a nerd-dictation amb safata del sistema, models Vosk, simulació d'entrada i dreceres de KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Eina de control per veu i escriptura basada en ordres que utilitza Kaldi i Dragonfly per a un reconeixement de veu totalment local.

### Altres

Projectes no assignats encara a cap categoria.

- [VoxType](https://github.com/peteonrails/voxtype) — Veut a text amb botó per parlar per a Linux i Wayland amb set motors ASR locals, suport de GPU i mode de reunions.

## Codi obert vs. comparativa

| Projecte | Preu | Codi obert | Extensible | Sense connexió | Xinès |
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

## Com triar

- **Aplicació d'escriptori multiplataforma acabada** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 estrelles, Whisper/Parakeet offline.
- **Linux minimalista fora de línia, scriptable** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simula l'entrada de teclat a qualsevol aplicació.
- **Integrar STT a la teva pròpia aplicació** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Whisper en C/C++, CPU/GPU, integrable.
- **Entrada prioritària en xinès** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; entrada de veu xinesa fora de línia per a Linux amb FunASR Paraformer, IBus/Fcitx5, drecera PTT i poliment de frases.
- **Autoallotjar una API/servidor de transcripció** → [FunASR](https://github.com/modelscope/FunASR) — Kit d'eines ASR industrial amb Paraformer, SenseVoice, VAD, diarització, streaming i API compatible amb OpenAI.

## Contribucions

Les contribucions són benvingudes — vegeu [CONTRIBUTING.md](CONTRIBUTING.md). Els projectes han de ser totalment de codi obert, extensibles i lleugers; si us plau, seguiu la guia d'estil de les descripcions (en anglès, una línia, factual, sense màrqueting buit).

## Historial d'Estrelles

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Creixement d'estrelles al llarg del temps per als projectes amb més estrelles d'aquesta llista, inclòs aquest repositori.

## Llicència

[MIT](LICENSE).
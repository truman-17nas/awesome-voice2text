# Awesome Voice2Text

> Lista curada de software de entrada de voz / dictado de código abierto — totalmente abierto, extensible y ligero. Comparado con Typeless, Lazytype y Shandianshuo (闪电说), todos los cuales son de código cerrado.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Si esta lista es útil, por favor ⭐ el repositorio — ayuda a otros a encontrarlo.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · **Español** · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Contenido

- [Benchmarks (código cerrado)](#benchmarks-código-cerrado)
- [Por qué esta lista](#por-qué-esta-lista)
- [Criterios de inclusión](#criterios-de-inclusión)
- [Selecciones principales](#selecciones-principales)
- [Todos los proyectos](#todos-los-proyectos)
- [Lista categorizada](#lista-categorizada)
  - [Dictado en tiempo real multiplataforma para escritorio](#dictado-en-tiempo-real-multiplataforma-para-escritorio)
  - [Dictado nativo para macOS](#dictado-nativo-para-macos)
  - [Limpieza de voz con IA / Postprocesamiento con LLM](#limpieza-de-voz-con-ia-postprocesamiento-con-llm)
  - [Motores y herramientas STT locales/sin conexión](#motores-y-herramientas-stt-localessin-conexión)
  - [Entrada de voz a nivel del sistema / IME](#entrada-de-voz-a-nivel-del-sistema-ime)
  - [Entrada de voz en chino / IME](#entrada-de-voz-en-chino-ime)
  - [Entrada de voz para navegador y web](#entrada-de-voz-para-navegador-y-web)
  - [Entrada de voz móvil (no IME)](#entrada-de-voz-móvil-no-ime)
  - [Scripts ligeros, CLI y control por voz](#scripts-ligeros-cli-y-control-por-voz)
  - [Otros](#otros)
- [Código abierto vs. benchmarks](#código-abierto-vs-benchmarks)
- [Cómo elegir](#cómo-elegir)
- [Contribuciones](#contribuciones)
- [Historial de Estrellas](#historial-de-estrellas)
- [Licencia](#licencia)

## Benchmarks (código cerrado)

| Producto | Precio | Plataformas | Modelo/Motor | Código abierto |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Por qué esta lista

Typeless, Lazytype y Shandianshuo (闪电说) son potentes pero de código cerrado. Esta lista recopila alternativas de código abierto que cumplen tres criterios: el código es totalmente público, la herramienta se puede extender y es lo suficientemente ligera como para ejecutarse en una máquina personal. Actualmente cubre **75 proyectos en 9 categorías**, todos verificados como totalmente de código abierto.

## Criterios de inclusión

- ✅ **Totalmente de código abierto** — todo el código en una forja pública (GitHub, GitLab, Codeberg).
- 🔌 **Extensible** — puedes añadir las características, modelos o integraciones que desees.
- ⚡ **Ligero** — bloat mínimo, inicio rápido, huella pequeña.

## Selecciones principales

 🏆 **[Handy](https://github.com/cjpais/Handy)** — Herramienta multiplataforma de voz a texto sin conexión usando Whisper o Parakeet, con atajos globales y pegado al portapapeles. *Abanderado de la comunidad — 25,281 estrellas, la opción más pulida.*

**Selecciones Fit-5** (cumplen los tres criterios):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Porte de alto rendimiento en C/C++ de OpenAI Whisper con inferencia CPU/GPU, cuantización y soporte multiplataforma.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Herramienta de voz a texto sin conexión para Linux usando Vosk que simula entrada de teclado en cualquier aplicación.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Voz a texto pulsado para Linux y Wayland con siete motores ASR locales, soporte GPU y modo reuniones.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Script Bash para dictado de voz sin conexión mediante Whisper para TTY, X11, Wayland y WSL con edición opcional por LLM.

## Todos los proyectos

| Nombre | ⭐ Estrellas | Licencia | Lenguaje | Ajuste | Abierto | Extensible | Ligero | Chino |
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

## Lista categorizada

### Dictado en tiempo real multiplataforma para escritorio

Aplicaciones de dictado para escritorio basadas en Whisper para Linux, Windows o multiplataforma, con pulsado para hablar, transcripción local e inserción automática.

- [Handy](https://github.com/cjpais/Handy) — Herramienta multiplataforma de voz a texto sin conexión usando Whisper o Parakeet, con atajos globales y pegado al portapapeles.
- [Buzz](https://github.com/chidiwilliams/buzz) — GUI de escritorio multiplataforma para transcripción y traducción sin conexión con Whisper, aceleración por GPU y micrófono en vivo.
- [Vibe](https://github.com/thewh1teagle/vibe) — Aplicación de escritorio multiplataforma para transcripción sin conexión de audio y video usando Whisper, con aceleración por GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Kit de herramientas local-first con almacenamiento Markdown/SQLite, sincronización CRDT Yjs y utilidad de escritorio de voz a texto.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Voz a texto nativa para Linux con Whisper local y modelos ONNX, APIs en la nube, integración con Waybar y visualizador.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Aplicación de dictado para escritorio usando Whisper localmente o vía API, activada por atajo global para escribir en la ventana activa.
- [Chirp](https://github.com/Whamp/chirp-stt) — Aplicación de dictado para Windows solo CPU usando ParakeetV3, con alternancia por atajo, pegado al portapapeles y sustituciones de palabras.
- [Dabri](https://github.com/AshBuk/dabri) — Aplicación STT sin conexión para Linux usando whisper.cpp con modos daemon, CLI y WebSocket para escritorios X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Aplicación de notas sin conexión para Linux y Sailfish OS con STT local, TTS y traducción usando múltiples motores.
- [voxd](https://github.com/jakovius/voxd) — Dictado por voz para escritorio Linux usando whisper.cpp para ASR sin conexión con escritura mediante ydotool y postprocesamiento con IA.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Escritura por voz sin conexión para Linux mediante Whisper, Parakeet o Canary ONNX, con soporte X11/Wayland y pulido con LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Asistente de escritura por voz para Windows usando la tecla Bloq Mayús, con STT de múltiples proveedores y refinación opcional con LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Aplicación de dictado sin conexión multiplataforma con distil-whisper, control por atajo y asistente local opcional con LLM.
- [TalkType](https://github.com/lmacan1/talktype) — Escritura por voz pulsada multiplataforma usando faster-whisper, con atajos globales y pegado inteligente.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Aplicación de dictado multilingüe sin conexión usando Faster-Whisper, activada por atajo para transcribir en el campo activo.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Dictado por voz local para NixOS/Wayland usando whisper.cpp con retroalimentación GTK4 y soporte para 99 idiomas.
- [freespeak](https://github.com/Zetaphor/freespeak) — Aplicación de dictado para Wayland Linux con STT, corrección gramatical mediante LanguageTool e inserción de texto con ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agente de escritorio local con IA que combina dictado por voz, chat con LLM, generación de imágenes y automatización por voz.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Voz a texto para escritorio Windows usando faster-whisper con simulación de teclado, VAD, PTT y puntuación.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dictado por voz con Whisper para KDE Wayland con daemon en segundo plano, servicio systemd y pegado al portapapeles.

### Dictado nativo para macOS

Aplicaciones de dictado nativas para macOS construidas con Swift y WhisperKit, que soportan atajos globales, barra de menú y aceleración por Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Aplicación de transcripción de voz para macOS con motores Whisper y Parakeet, atajos globales y procesamiento por lotes.
- [Pindrop](https://github.com/watzon/pindrop) — Aplicación de dictado nativa para macOS en la barra de menú usando WhisperKit para STT sin conexión, con atajos y limpieza opcional con IA.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Herramienta de dictado multilingüe sin conexión usando Whisper, activada por atajo para transcribir en cualquier campo de entrada.
- [FnKey](https://github.com/evoleinik/fnkey) — Aplicación para la barra de menú de macOS que transcribe voz mediante Deepgram Nova-3 mientras se mantiene presionada Fn y pega el resultado.
- [hush](https://github.com/djmunro/hush) — Aplicación de dictado pulsado para macOS usando Whisper/Parakeet ONNX local con pegado automático mediante atajo.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Aplicación de dictado para la barra de menú de macOS usando Whisper sin conexión con aceleración Metal GPU e inserción de texto en el cursor.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Aplicación para la barra de menú de macOS que graba al soltar Globo/Fn, transcribe mediante faster-whisper y pega en el cursor.

### Limpieza de voz con IA / Postprocesamiento con LLM

Herramientas de dictado que usan LLMs locales o en la nube para pulir, formatear, resumir y reestilizar la salida del reconocimiento de voz en texto limpio y formal.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Aplicación de dictado para macOS con STT local y en la nube, atajos globales, flujos de trabajo con IA, plugins, API REST y CLI.
- [Amical](https://github.com/amicalhq/amical) — Aplicación de dictado con IA local-first usando Whisper para transcripción sin conexión y Ollama para procesamiento inteligente de notas.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Herramienta de dictado por voz sin conexión para macOS/Windows usando Whisper, con atajos globales y mejora opcional con IA.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Asistente de voz local-first para macOS y Linux con pulsado para hablar, transcripción y extracción mediante plugins.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Aplicación de dictado pulsado para macOS usando Whisper y limpieza con LLM, pegando texto pulido mediante Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Dictado por voz local con pulido mediante Whisper y LLM, pulsado para hablar, diccionario y arquitectura cliente-servidor.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Dictado por voz local y grabadora de reuniones con faster-whisper, resúmenes con LLM y captura de audio de dos pistas.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Aplicación nativa de voz a texto para macOS usando modelos whisper.cpp locales, con atajos globales y modos contextuales.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Aplicación de dictado para macOS con reconocimiento de voz en el dispositivo y postprocesamiento opcional con IA para formatear.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Aplicación de escritorio de transcripción de voz con atajos, asistente de IA, diarización de reuniones y búsqueda semántica.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Aplicación para la barra de menú de macOS para voz a texto sin conexión y resúmenes de reuniones usando Whisper y Qwen en Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Aplicación multiplataforma Tauri de escritura por voz con Whisper local o Groq, limpieza con IA, glosario y asistente de voz.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Asistente de dictado por voz multiplataforma con formateo mediante LLM, soportando Whisper local, Ollama o APIs en la nube.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Aplicación multiplataforma Tauri para escritura por voz con IA, reescritura de texto y preguntas-respuestas por voz con atajos globales.
- [Aria](https://github.com/Xingxun7777/Aria) — Entrada de voz con IA para Windows usando Qwen3-ASR sin conexión con contexto OCR, corrección por palabra clave y comandos de voz.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Dictado por voz para Windows usando whisper.cpp, Groq o llama.cpp, múltiples estilos y pegado automático a la ventana activa.
- [localflow](https://github.com/sidharth-n/localflow) — Dictado por voz local multiplataforma usando Moonshine STT, pulidor Qwen3-4B, pulsado para hablar y skip-gate.
- [yammer](https://github.com/andynu/yammer) — Voz a texto local para Linux con Whisper y limpieza con LLM, más una interfaz superpuesta en Tauri e inyección xdotool.

### Motores y herramientas STT locales/sin conexión

Motores ASR sin conexión y toolkits de voz para integración en aplicaciones: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech y SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Porte de alto rendimiento en C/C++ de OpenAI Whisper con inferencia CPU/GPU, cuantización y soporte multiplataforma.
- [FunASR](https://github.com/modelscope/FunASR) — Toolkit industrial ASR con Paraformer, SenseVoice, VAD, diarización, streaming y API compatible con OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Toolkit de reconocimiento de voz sin conexión con modelos pequeños solo CPU para más de 20 idiomas y bindings multilenguaje.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Toolkit de voz sin conexión usando Kaldi de siguiente generación y ONNX Runtime para STT, TTS, identificación de hablante, VAD y más.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Toolkit completo de voz con ASR, TTS, huella de voz, diarización, traducción y servicios de streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Modelo de voz con ASR para más de 50 idiomas, emoción, eventos de audio e inferencia no autoregresiva rápida.

### Entrada de voz a nivel del sistema / IME

Soluciones de entrada de voz integradas a nivel del sistema, incluyendo métodos de entrada, extensiones IBus/Fcitx, IME de Android y teclados de iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME de Android y servicio de entrada de voz usando Whisper para reconocimiento de voz sin conexión y traducción al inglés.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Aplicación de dictado por voz sin conexión para Linux con whisper.cpp, Whisper y motores VOSK, GPU Vulkan e interfaz GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Extensión de GNOME Shell para entrada de voz sin conexión mediante whisper.cpp con activación por atajo, soportando X11 y Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Servicio de reconocimiento de voz sin conexión para Android usando Vosk con soporte estándar de RecognitionService API.
- [Dictus](https://github.com/getdictus/dictus-ios) — Teclado de código abierto para iOS con dictado por voz en el dispositivo usando WhisperKit y CoreML, funciona en cualquier app.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Método de entrada de voz a texto IBus para Linux con STT por streaming, refinación opcional con Whisper y aceleración GPU.

### Entrada de voz en chino / IME

Proyectos optimizados para el reconocimiento y la entrada de voz en chino, incluyendo IME y teclados basados en FunASR, Paraformer y SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Entrada de voz china sin conexión para Linux usando FunASR Paraformer, IBus/Fcitx5, atajo PTT y pulido de oraciones.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Método de entrada de voz sin conexión multiplataforma usando FunASR, con corrección por palabra clave, pegado automático y modos GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Teclado de entrada de voz para Android con 11 motores ASR, postprocesamiento con LLM, bola flotante e interfaz Material3.

### Entrada de voz para navegador y web

Entrada de voz basada en navegador mediante extensiones, wrappers WebAssembly o interfaces Web, típicamente requiriendo un backend STT local o en la nube.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Interfaz web Gradio para Whisper para subtítulos desde archivos, YouTube o micrófono, con VAD, separación de BGM y diarización.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Extensión de navegador para voz a texto en tiempo real sin conexión mediante Vosk, con comandos de voz en árabe e inglés.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Librería de reconocimiento de voz sin conexión basada en navegador que empaqueta Vosk como WebAssembly ejecutándose en un WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Extensión de navegador y servidor local Whisper para voz a texto sin conexión en Firefox y Chrome mediante Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Extensión de Chrome que graba voz mediante atajo, transcribe con la API de OpenAI Whisper y pega el texto automáticamente.
- [voico](https://github.com/Kirera-Wainaina/voico) — Extensión de Chrome para entrada de voz a texto en campos web, con backend Node.js usando STT de Google y OpenAI.

### Entrada de voz móvil (no IME)

Aplicaciones independientes de transcripción de voz en Android o iOS, en lugar de teclados de métodos de entrada.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Teclado de reconocimiento de voz privado en el dispositivo para Android usando Whisper mediante whisper.cpp y Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Aplicación de código abierto para iOS de transcripción de voz sin conexión usando Whisper.cpp, con grabación y exportación de audio.
- [seamless](https://github.com/woheller69/seamless) — Aplicación de traducción de voz a texto sin conexión para Android usando Meta Seamless M4T Lite para 5 idiomas con salida TTS.

### Scripts ligeros, CLI y control por voz

Scripts ligeros, herramientas CLI, activadores de bandeja o utilidades adecuadas para integración por desarrolladores o como complementos a cadenas de herramientas existentes.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Herramienta de voz a texto sin conexión para Linux usando Vosk que simula entrada de teclado en cualquier aplicación.
- [voice_typing](https://github.com/themanyone/voice_typing) — Script Bash para dictado de voz sin conexión mediante Whisper para TTY, X11, Wayland y WSL con edición opcional por LLM.
- [hns](https://github.com/primaprashant/hns) — Herramienta CLI para voz a texto local desde micrófono usando faster-whisper, con copia al portapapeles y salida por stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Gestor GUI PyQt6 para nerd-dictation con bandeja del sistema, modelos Vosk, simulación de entrada y atajos KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Herramienta de control por voz y escritura basada en comandos usando Kaldi y Dragonfly para reconocimiento de voz completamente local.

### Otros

Proyectos aún no asignados a una categoría.

- [VoxType](https://github.com/peteonrails/voxtype) — Voz a texto pulsado para Linux y Wayland con siete motores ASR locales, soporte GPU y modo reuniones.

## Código abierto vs. benchmarks

| Proyecto | Precio | Código abierto | Extensible | Sin conexión | Chino |
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

## Cómo elegir

- **Aplicación de escritorio pulida multiplataforma** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 estrellas, Whisper/Parakeet sin conexión.
- **Linux sin conexión mínimo, scriptable** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simula entrada de teclado en cualquier app.
- **Incrustar STT en tu propia app** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Whisper en C/C++, CPU/GPU, embebible.
- **Entrada primero en chino** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; entrada de voz china sin conexión para Linux usando FunASR Paraformer, IBus/Fcitx5, atajo PTT y pulido de oraciones.
- **Autoalojar una API/servidor de transcripción** → [FunASR](https://github.com/modelscope/FunASR) — Toolkit industrial ASR con Paraformer, SenseVoice, VAD, diarización, streaming y API compatible con OpenAI.

## Contribuciones

Las contribuciones son bienvenidas — consulta [CONTRIBUTING.md](CONTRIBUTING.md). Los proyectos deben ser completamente de código abierto, extensibles y ligeros; sigue la guía de estilo de descripción (en inglés, una línea, factual, sin marketing vacío).

## Historial de Estrellas

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Tendencia del crecimiento de estrellas con el tiempo para los proyectos con más estrellas de esta lista, incluido este repositorio.

## Licencia

[MIT](LICENSE).

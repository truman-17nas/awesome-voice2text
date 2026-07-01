# Awesome Voice2Text

> Uma lista curada de softwares de entrada de voz / ditado de código aberto — totalmente aberto, extensível e leve. Comparada com Typeless, Lazytype e Shandianshuo (闪电说), todos de código fechado.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Se esta lista for útil, por favor ⭐ o repositório — isso ajuda outras pessoas a encontrá-lo.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · **Português** · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Conteúdo

- [Referências (Código Fechado)](#referências-código-fechado)
- [Por que esta lista](#por-que-esta-lista)
- [Critérios de inclusão](#critérios-de-inclusão)
- [Principais escolhas](#principais-escolhas)
- [Todos os projetos](#todos-os-projetos)
- [Lista categorizada](#lista-categorizada)
  - [Ditado em tempo real para desktop multiplataforma](#ditado-em-tempo-real-para-desktop-multiplataforma)
  - [Ditado nativo para macOS](#ditado-nativo-para-macos)
  - [Limpeza de fala com IA / Pós-processamento por LLM](#limpeza-de-fala-com-ia-pós-processamento-por-llm)
  - [Motores e kits STT locais/offline](#motores-e-kits-stt-locaisoffline)
  - [Entrada de voz em nível de sistema / IME](#entrada-de-voz-em-nível-de-sistema-ime)
  - [Entrada de fala em chinês / IME](#entrada-de-fala-em-chinês-ime)
  - [Entrada de voz para navegador e web](#entrada-de-voz-para-navegador-e-web)
  - [Entrada de voz para dispositivos móveis (não IME)](#entrada-de-voz-para-dispositivos-móveis-não-ime)
  - [Scripts leves, CLI e controle por voz](#scripts-leves-cli-e-controle-por-voz)
  - [Outros](#outros)
- [Código aberto vs. referências](#código-aberto-vs-referências)
- [Como escolher](#como-escolher)
- [Contribuições](#contribuições)
- [Histórico de Estrelas](#histórico-de-estrelas)
- [Licença](#licença)

## Referências (Código Fechado)

| Produto | Preço | Plataformas | Modelo/Motor | Código aberto |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Por que esta lista

Typeless, Lazytype e Shandianshuo (闪电说) são poderosos, mas de código fechado. Esta lista reúne alternativas de código aberto que atendem a três critérios: o código é totalmente público, a ferramenta pode ser estendida e é leve o suficiente para rodar em uma máquina pessoal. Atualmente cobre **75 projetos em 9 categorias**, todos verificados como totalmente de código aberto.

## Critérios de inclusão

- ✅ **Totalmente de código aberto** — todo o código em uma forja pública (GitHub, GitLab, Codeberg).
- 🔌 **Extensível** — você pode adicionar os recursos, modelos ou integrações que desejar.
- ⚡ **Leve** — mínimo de inchaço, inicialização rápida, pequena pegada.

## Principais escolhas

🏆 **[Handy](https://github.com/cjpais/Handy)** — Ferramenta multiplataforma offline de voz para texto usando Whisper ou Parakeet, com atalhos globais e colar da área de transferência. *Carro-chefe da comunidade — 25.281 estrelas, a oferta mais polida.*

**Fit-5 picks** (atendem a todos os três critérios):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Porte C/C++ de alta performance do OpenAI Whisper com inferência CPU/GPU, quantização e suporte multiplataforma.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Ferramenta Linux offline de fala para texto usando Vosk que simula entrada de teclado em qualquer aplicação.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Voz para texto com push-to-talk no Linux e Wayland, com sete motores ASR locais, suporte a GPU e modo reunião.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Script Bash para digitação por voz offline via Whisper para TTY, X11, Wayland e WSL com edição opcional por LLM.

## Todos os projetos

| Nome | ⭐ Estrelas | Licença | Linguagem | Fit | Aberto | Ext | LW | Chinês |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 51.163 | MIT | C/C++, CMake, Python/Java/C# bindings | 5 | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | 1.882 | GPL-3.0 | Python | 5 | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | 909 | MIT | Rust | 5 | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | 155 | GPL-2.0 | Bash | 5 | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | 25.281 | MIT | Rust, Tauri, React, TypeScript, Tailwind | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | 19.906 | MIT | Python, PyQt6, Whisper, PyTorch, ONNX Runtime | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [FunASR](https://github.com/modelscope/FunASR) | 18.745 | MIT | Python (PyTorch) | 4 | ⚠️ | ✅ | ⚠️ | ✅ |
| [vosk-api](https://github.com/alphacep/vosk-api) | 14.889 | Apache-2.0 | C++ with Python, Java, C#, Node.js, Rust, Go | 4 | ⚠️ | ✅ | ✅ | ✅ |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | 13.280 | Apache-2.0 | C++, Python, Go, Java, Rust, C#, Swift, JS, Dart | 4 | ✅ | ✅ | ⚠️ | ✅ |
| [Vibe](https://github.com/thewh1teagle/vibe) | 6.635 | MIT | Rust, Tauri, TypeScript, React, whisper.cpp | 4 | ✅ | ✅ | ✅ | ✅ |
| [Epicenter](https://github.com/EpicenterHQ/epicenter) | 4.663 | MIT + AGPL-3.0-or-later | — | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) | 2.821 | Apache-2.0 | Python, PyTorch, Gradio, FFmpeg | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) | 1.541 | GPL-3.0 | Swift | 4 | ✅ | ✅ | ✅ | ⚠️ |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) | 1.474 | MIT | Swift, Shell, CMake, C, Ruby | 4 | ✅ | ⚠️ | ⚠️ | ✅ |
| [Amical](https://github.com/amicalhq/amical) | 1.388 | MIT | TypeScript, Electron, Next.js, React | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr) | 1.074 | MIT | Python, C/C++, GTK4, Astro | 4 | ✅ | ✅ | ⚠️ | ⚠️ |
| [whisper-writer](https://github.com/savbell/whisper-writer) | 1.071 | GPL-3.0 | Python | 4 | ✅ | ✅ | ⚠️ | ◐ |
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
| [dsnote (Speech Note)](https://github.com/mkiol/dsnote) | 1.525 | MPL-2.0 | C++17, Qt5/QML, CMake, Python | 3.5 | ✅ | ⚠️ | ⚠️ | ✅ |
| [VoiceFlow](https://github.com/infiniV/VoiceFlow) | 393 | MIT | Python, React, Vite, faster-whisper | 3.5 | ✅ | ⚠️ | ✅ | ◐ |
| [voice-input-method](https://github.com/pofice/voice-input-method) | 38 | GPL-3.0-or-later | Python 3.10+ | 3.5 | ✅ | ✅ | ✅ | ✅ |
| [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) | 0 | MIT | JavaScript (Manifest V3), Python | 3.5 | ⚠️ | ✅ | ✅ | ⚠️ |
| [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) | 12.636 | Apache-2.0 | Python, C++ | 3 | ✅ | ✅ | ⚠️ | ✅ |
| [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) | 8.731 | MIT | Python, C/C++ | 3 | ⚠️ | ✅ | ✅ | ✅ |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) | 5.387 | GPL-3.0 | Swift, whisper.cpp | 3 | ✅ | ⚠️ | ✅ | ◐ |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) | 5.013 | GPL-3.0 | Swift | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) | 4.143 | MIT | TypeScript, React, Electron, Vite, Tailwind CSS | 3 | ✅ | ✅ | ⚠️ | ◐ |
| [Ghost Pepper](https://github.com/matthartman/ghost-pepper) | 2.800 | MIT | Swift | 3 | ✅ | ⚠️ | ⚠️ | ◐ |
| [WhisperBoard](https://github.com/Saik0s/Whisperboard) | 1.040 | GPL-3.0 | Swift, SwiftUI, TCA, whisper.cpp, Tuist | 3 | ✅ | ⚠️ | ✅ | ⚠️ |
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

### Ditado em tempo real para desktop multiplataforma

Aplicativos de desktop baseados em Whisper para ditado no Linux, Windows ou multiplataforma, com push-to-talk, transcrição local e entrada automática.

- [Handy](https://github.com/cjpais/Handy) — Ferramenta multiplataforma offline de voz para texto usando Whisper ou Parakeet, com atalhos globais e colar da área de transferência.
- [Buzz](https://github.com/chidiwilliams/buzz) — GUI desktop multiplataforma para transcrição e tradução offline com Whisper, aceleração por GPU e microfone ao vivo.
- [Vibe](https://github.com/thewh1teagle/vibe) — Aplicativo desktop multiplataforma para transcrição offline de áudio e vídeo usando Whisper, com aceleração por GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Toolkit local-first com armazenamento Markdown/SQLite, sincronização Yjs CRDT e utilitário desktop de fala para texto.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Fala para texto nativo no Linux com Whisper local e modelos ONNX, APIs em nuvem, integração Waybar e visualizador.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Aplicativo de ditado desktop usando Whisper localmente ou via API, acionado por atalho global para digitar na janela ativa.
- [Chirp](https://github.com/Whamp/chirp-stt) — Aplicativo de ditado para Windows usando apenas CPU com ParakeetV3, com alternância por atalho, colar da área de transferência e substituição de palavras.
- [Dabri](https://github.com/AshBuk/dabri) — Aplicativo Linux offline de STT usando whisper.cpp com modos daemon, CLI e WebSocket para desktops X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Aplicativo de anotações offline para Linux e Sailfish OS com STT local, TTS e tradução usando vários motores.
- [voxd](https://github.com/jakovius/voxd) — Ditado por voz desktop no Linux usando whisper.cpp para ASR offline com digitação via ydotool e pós-processamento por IA.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Digitação por voz offline no Linux via Whisper, Parakeet ou Canary ONNX, com suporte X11/Wayland e polimento por LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Assistente de digitação por voz para Windows usando a tecla Caps Lock, com STT multi-provedor e refinamento opcional por LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Aplicativo multiplataforma de ditado offline com distil-whisper, controle por atalho e assistente local opcional por LLM.
- [TalkType](https://github.com/lmacan1/talktype) — Digitação por voz com push-to-talk multiplataforma usando faster-whisper, com atalhos globais e colar inteligente.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Aplicativo multilíngue de ditado offline usando Faster-Whisper, acionado por atalho para transcrever no campo ativo.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Ditado por voz local para NixOS/Wayland usando whisper.cpp com feedback GTK4 e suporte a 99 idiomas.
- [freespeak](https://github.com/Zetaphor/freespeak) — Aplicativo de ditado por voz para Linux Wayland com STT, correção gramatical via LanguageTool e entrada de texto via ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agente desktop de IA local combinando ditado por voz, chat com LLM, geração de imagens e automação por voz.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Fala para texto desktop para Windows usando faster-whisper com simulação de teclado, VAD, PTT e pontuação.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Ditado por voz Whisper para KDE Wayland com daemon em segundo plano, serviço systemd e colar da área de transferência.

### Ditado nativo para macOS

Aplicativos nativos de ditado para macOS feitos com Swift e WhisperKit, com suporte a atalhos globais, barra de menus e aceleração pela Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Aplicativo de transcrição de fala para macOS com motores Whisper e Parakeet, atalhos globais e processamento em lote.
- [Pindrop](https://github.com/watzon/pindrop) — Aplicativo nativo de ditado na barra de menus do macOS usando WhisperKit para STT offline, com atalhos e limpeza opcional por IA.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Ferramenta multilíngue de ditado offline usando Whisper, acionada por atalho para transcrever em qualquer campo de entrada.
- [FnKey](https://github.com/evoleinik/fnkey) — Aplicativo de barra de menus do macOS que transcreve fala via Deepgram Nova-3 enquanto Fn é pressionado e cola o resultado.
- [hush](https://github.com/djmunro/hush) — Aplicativo de ditado push-to-talk para macOS usando Whisper/Parakeet ONNX local com colar automático via atalho.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Aplicativo de ditado na barra de menus do macOS usando Whisper offline com aceleração por GPU Metal e injeção de texto no cursor.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Aplicativo de barra de menus do macOS que grava ao soltar Globe/Fn, transcreve via faster-whisper e cola no cursor.

### Limpeza de fala com IA / Pós-processamento por LLM

Ferramentas de ditado que usam LLMs locais ou em nuvem para polir, formatar, resumir e reestilizar a saída do reconhecimento de fala em texto limpo e formal.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Aplicativo de ditado para macOS com STT local e em nuvem, atalhos globais, fluxos de trabalho de IA, plugins, API REST e CLI.
- [Amical](https://github.com/amicalhq/amical) — Aplicativo local-first de ditado com IA usando Whisper para transcrição offline e Ollama para processamento inteligente de notas.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Ferramenta offline de ditado por voz para macOS/Windows usando Whisper, com atalhos globais e aprimoramento opcional por IA.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Assistente de voz local-first para macOS e Linux com push-to-talk, transcrição e extração por plugins.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Aplicativo de ditado push-to-talk para macOS usando Whisper e limpeza por LLM, colando texto polido via Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Ditado por voz local com polimento por Whisper e LLM, push-to-talk, dicionário e arquitetura cliente-servidor.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Ditado por voz local e gravador de reuniões com faster-whisper, resumos por LLM e captura de áudio em duas faixas.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Aplicativo nativo de voz para texto para macOS usando modelos locais whisper.cpp, com atalhos globais e modos context-aware.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Aplicativo de ditado para macOS com reconhecimento de fala no dispositivo e pós-processamento opcional por IA para formatação.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Aplicativo desktop de transcrição de voz com atalhos, assistente de IA, diarização de reuniões e busca semântica.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Aplicativo de barra de menus do macOS para fala para texto offline e resumos de reuniões usando Whisper e Qwen no Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Aplicativo multiplataforma Tauri de digitação por voz com Whisper local ou Groq, limpeza por IA, glossário e assistente de voz.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Assistente de ditado por voz multiplataforma com formatação por LLM, suportando Whisper local, Ollama ou APIs em nuvem.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Aplicativo Tauri multiplataforma para digitação por voz com IA, reescrita de texto e Q&A por voz com atalhos globais.
- [Aria](https://github.com/Xingxun7777/Aria) — Entrada de voz com IA para Windows usando Qwen3-ASR offline com contexto OCR, correção por palavra-chave e comandos de voz.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Ditado por voz para Windows usando whisper.cpp, Groq ou llama.cpp, vários estilos e colar automático na janela ativa.
- [localflow](https://github.com/sidharth-n/localflow) — Ditado por voz local multiplataforma usando Moonshine STT, polidor Qwen3-4B, push-to-talk e skip-gate.
- [yammer](https://github.com/andynu/yammer) — Fala para texto local no Linux com Whisper e limpeza por LLM, além de overlay UI em Tauri e injeção de entrada via xdotool.

### Motores e kits STT locais/offline

Motores de ASR offline e kits de ferramentas de fala para integração em aplicativos: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech e SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Porte C/C++ de alta performance do OpenAI Whisper com inferência CPU/GPU, quantização e suporte multiplataforma.
- [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industrial com Paraformer, SenseVoice, VAD, diarização, streaming e API compatível com OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Toolkit de reconhecimento de fala offline com modelos pequenos apenas para CPU para 20+ idiomas e bindings multilíngues.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Toolkit de fala offline usando Kaldi de próxima geração e ONNX Runtime para STT, TTS, identificação de locutor, VAD e mais.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Toolkit de fala abrangente com ASR, TTS, voiceprint, diarização, tradução e serviços de streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Modelo de fala com ASR para 50+ idiomas, emoção, eventos de áudio e inferência não-autorregressiva rápida.

### Entrada de voz em nível de sistema / IME

Soluções de entrada de voz integradas em nível de sistema, incluindo métodos de entrada, extensões IBus/Fcitx, IME Android e teclados iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android e serviço de entrada de voz usando Whisper para reconhecimento de fala offline e tradução para inglês.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Aplicativo de ditado por voz offline para Linux com motores whisper.cpp, Whisper e VOSK, GPU Vulkan e GUI GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Extensão do GNOME Shell para entrada de voz offline via whisper.cpp com gatilho por atalho, suportando X11 e Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Serviço Android de reconhecimento de fala offline usando Vosk com suporte à API RecognitionService padrão.
- [Dictus](https://github.com/getdictus/dictus-ios) — Teclado iOS de código aberto para ditado de voz no dispositivo usando WhisperKit e CoreML, funciona em qualquer aplicativo.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Método de entrada de fala para texto IBus no Linux com STT em streaming, refinamento opcional por Whisper e aceleração por GPU.

### Entrada de fala em chinês / IME

Projetos otimizados para reconhecimento e entrada de fala em chinês, incluindo IMEs e teclados baseados em FunASR, Paraformer e SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Entrada de voz chinesa offline para Linux usando FunASR Paraformer, IBus/Fcitx5, atalho PTT e polimento de frases.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Método de entrada de voz offline multiplataforma usando FunASR, com correção por hotword, colar automático e modos GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Teclado de entrada de voz Android com 11 motores ASR, pós-processamento por LLM, bola flutuante e UI Material3.

### Entrada de voz para navegador e web

Entrada de voz baseada em navegador via extensões, wrappers WebAssembly ou Web UIs, normalmente exigindo um backend STT local ou em nuvem.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — WebUI Gradio para Whisper para legendas a partir de arquivos, YouTube ou microfone, com VAD, separação de BGM e diarização.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Extensão de navegador para fala para texto offline em tempo real via Vosk, com comandos de voz em árabe e inglês.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Biblioteca de reconhecimento de fala offline baseada em navegador empacotando Vosk como WebAssembly rodando em WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Extensão de navegador e servidor local Whisper para fala para texto offline no Firefox e Chrome via Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Extensão Chrome que grava voz via atalho, transcreve com a API OpenAI Whisper e cola o texto automaticamente.
- [voico](https://github.com/Kirera-Wainaina/voico) — Extensão Chrome para entrada de voz para texto em campos web, com backend Node.js usando Google e OpenAI STT.

### Entrada de voz para dispositivos móveis (não IME)

Aplicativos autônomos de transcrição de voz no Android ou iOS, em vez de teclados de método de entrada.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Teclado de reconhecimento de fala privado no dispositivo para Android usando Whisper via whisper.cpp e Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Aplicativo iOS de código aberto para transcrição de voz offline usando Whisper.cpp, com gravação e exportação de áudio.
- [seamless](https://github.com/woheller69/seamless) — Aplicativo Android offline de tradução de fala para texto usando Meta Seamless M4T Lite para 5 idiomas com saída TTS.

### Scripts leves, CLI e controle por voz

Scripts leves, ferramentas CLI, gatilhos na bandeja ou utilitários adequados para integração por desenvolvedores ou como complementos a toolchains existentes.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Ferramenta Linux offline de fala para texto usando Vosk que simula entrada de teclado em qualquer aplicação.
- [voice_typing](https://github.com/themanyone/voice_typing) — Script Bash para digitação por voz offline via Whisper para TTY, X11, Wayland e WSL com edição opcional por LLM.
- [hns](https://github.com/primaprashant/hns) — Ferramenta CLI para fala para texto local usando microfone e faster-whisper, com cópia para área de transferência e saída via stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Gerenciador GUI PyQt6 para nerd-dictation com bandeja do sistema, modelos Vosk, simulação de entrada e atalhos KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Ferramenta de controle por voz e digitação baseada em comandos usando Kaldi e Dragonfly para reconhecimento de fala totalmente local.

### Outros

Projetos ainda não atribuídos a uma categoria.

- [VoxType](https://github.com/peteonrails/voxtype) — Voz para texto com push-to-talk no Linux e Wayland, com sete motores ASR locais, suporte a GPU e modo reunião.

## Código aberto vs. referências

| Projeto | Preço | Código aberto | Extensível | Offline | Chinês |
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

## Como escolher

- **Aplicativo desktop multiplataforma polido** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25.281 estrelas, Whisper/Parakeet offline.
- **Linux offline minimal e scriptável** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simula entrada de teclado em qualquer aplicativo.
- **Incorporar STT no seu próprio aplicativo** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, incorporável.
- **Entrada em chinês** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; entrada de voz chinesa offline para Linux usando FunASR Paraformer, IBus/Fcitx5, atalho PTT e polimento de frases.
- **Self-host de API/servidor de transcrição** → [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industrial com Paraformer, SenseVoice, VAD, diarização, streaming e API compatível com OpenAI.

## Contribuições

Contribuições são bem-vindas — veja [CONTRIBUTING.md](CONTRIBUTING.md). Os projetos devem ser totalmente open source, extensíveis e leves; siga o guia de estilo das descrições (em inglês, uma linha, factual, sem linguagem de marketing vazia).

## Histórico de Estrelas

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Crescimento de estrelas ao longo do tempo para os projetos com mais estrelas desta lista, incluindo este repositório.

## Licença

[MIT](LICENSE).
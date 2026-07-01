# Awesome Voice Input

> Una raccolta curata di software open-source per input vocale / dettatura — completamente aperti, estendibili e leggeri. Confrontati con Typeless, Lazytype e Shandianshuo (闪电说), tutti closed-source.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Se questa lista ti è utile, metti una ⭐ al repo — aiuta gli altri a trovarlo.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · **Italiano** · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Contenuti

- [Benchmark (a codice chiuso)](#benchmark-a-codice-chiuso)
- [Perché questa lista](#perché-questa-lista)
- [Criteri di inclusione](#criteri-di-inclusione)
- [Scelti](#scelti)
- [Tutti i progetti](#tutti-i-progetti)
- [Lista categorizzata](#lista-categorizzata)
  - [Dittatura desktop multipiattaforma in tempo reale](#dittatura-desktop-multipiattaforma-in-tempo-reale)
  - [Dittatura nativa per macOS](#dittatura-nativa-per-macos)
  - [Pulizia del parlato con AI / post-elaborazione LLM](#pulizia-del-parlato-con-ai-post-elaborazione-llm)
  - [Motori e toolkit STT locali/offline](#motori-e-toolkit-stt-localioffline)
  - [Input vocale a livello di sistema / IME](#input-vocale-a-livello-di-sistema-ime)
  - [Input vocale cinese / IME](#input-vocale-cinese-ime)
  - [Input vocale per browser e web](#input-vocale-per-browser-e-web)
  - [Input vocale mobile (non IME)](#input-vocale-mobile-non-ime)
  - [Script leggeri, CLI e controllo vocale](#script-leggeri-cli-e-controllo-vocale)
  - [Altro](#altro)
- [Open-source vs benchmark](#open-source-vs-benchmark)
- [Come scegliere](#come-scegliere)
- [Contributi](#contributi)
- [Cronologia delle Stelle](#cronologia-delle-stelle)
- [Licenza](#licenza)

## Benchmark (a codice chiuso)

| Prodotto | Prezzo | Piattaforme | Modello/Motore | Open Source |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Perché questa lista

Typeless, Lazytype e Shandianshuo (闪电说) sono potenti ma closed-source. Questa lista raccoglie alternative open-source che soddisfano tre criteri: il codice è completamente pubblico, lo strumento è estendibile e rimane abbastanza leggero per girare su una macchina personale. Attualmente copre **75 progetti in 9 categorie**, tutti verificati come completamente open-source.

## Criteri di inclusione

- ✅ **Completamente open-source** — tutto il codice su una forge pubblica (GitHub, GitLab, Codeberg).
- 🔌 **Estendibile** — puoi aggiungere le funzionalità, i modelli o le integrazioni che desideri.
- ⚡ **Leggero** — minimo appesantimento, avvio rapido, piccolo impatto sul sistema.

## Scelti

🏆 **[Handy](https://github.com/cjpais/Handy)** — Strumento multipiattaforma offline di riconoscimento vocale in testo che utilizza Whisper o Parakeet, con tasti di scelta rapida globali e incolla dalla clipboard. *Progetto di punta della community — 25,281 stars, l'offerta più rifinita.*

**Scelte Fit-5** (soddisfano tutti e tre i criteri):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Port ad alte prestazioni in C/C++ di OpenAI Whisper con inferenza CPU/GPU, quantizzazione e supporto multipiattaforma.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Strumento offline di riconoscimento vocale per Linux che utilizza Vosk e simula l'input da tastiera in qualsiasi applicazione.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Dittatura vocale push-to-talk per Linux e Wayland con sette motori ASR locali, supporto GPU e modalità riunione.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Script Bash per la digitazione vocale offline tramite Whisper per TTY, X11, Wayland e WSL con modifica LLM opzionale.

## Tutti i progetti

| Nome | ⭐ Stelle | Licenza | Linguaggio | Fit | Open | Ext | LW | Cinese |
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

## Lista categorizzata

### Dittatura desktop multipiattaforma in tempo reale

App desktop di dittatura basate su Whisper per Linux, Windows o multipiattaforma, con push-to-talk, trascrizione locale e input automatico.

- [Handy](https://github.com/cjpais/Handy) — Strumento multipiattaforma offline di riconoscimento vocale in testo che utilizza Whisper o Parakeet, con tasti di scelta rapida globali e incolla dalla clipboard.
- [Buzz](https://github.com/chidiwilliams/buzz) — Interfaccia grafica desktop multipiattaforma per la trascrizione e la traduzione offline con Whisper, accelerazione GPU e microfono in tempo reale.
- [Vibe](https://github.com/thewh1teagle/vibe) — App desktop multipiattaforma per la trascrizione offline di audio e video utilizzando Whisper, con accelerazione GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Toolkit di app local-first con archiviazione Markdown/SQLite, sincronizzazione CRDT Yjs e un'utilità desktop di riconoscimento vocale in testo.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Dittatura vocale nativa per Linux con Whisper locale e modelli ONNX, API cloud, integrazione Waybar e visualizzatore.
- [whisper-writer](https://github.com/savbell/whisper-writer) — App di dittatura desktop che utilizza Whisper localmente o tramite API, attivata da un tasto di scelta rapida globale per digitare nella finestra attiva.
- [Chirp](https://github.com/Whamp/chirp-stt) — App di dittatura per Windows solo CPU che utilizza ParakeetV3, con attivazione tramite tasto di scelta rapida, incolla dalla clipboard e sostituzione di parole.
- [Dabri](https://github.com/AshBuk/dabri) — App STT offline per Linux che utilizza whisper.cpp con modalità daemon, CLI e WebSocket per desktop X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — App di note offline per Linux e Sailfish OS con STT locale, TTS e traduzione utilizzando più motori.
- [voxd](https://github.com/jakovius/voxd) — Dittatura vocale desktop per Linux che utilizza whisper.cpp per ASR offline con digitazione ydotool e post-elaborazione AI.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Digitazione vocale offline per Linux tramite Whisper, Parakeet o Canary ONNX, con supporto X11/Wayland e rifinitura LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Assistente di digitazione vocale per Windows che utilizza il tasto Blocco Maiuscole come scelta rapida, con STT multi-provider e perfezionamento LLM opzionale.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — App di dittatura offline multipiattaforma con distil-whisper, controllo tramite tasti di scelta rapida e assistente LLM locale opzionale.
- [TalkType](https://github.com/lmacan1/talktype) — Digitazione vocale push-to-talk multipiattaforma che utilizza faster-whisper, con tasti di scelta rapida globali e incolla intelligente.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — App di dittatura multilingue offline che utilizza Faster-Whisper, attivata da tasto di scelta rapida per trascrivere nel campo attivo.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Dittatura vocale locale per NixOS/Wayland che utilizza whisper.cpp con feedback GTK4 e supporto per 99 lingue.
- [freespeak](https://github.com/Zetaphor/freespeak) — App di dittatura vocale per Linux Wayland con STT, correzione grammaticale tramite LanguageTool e input di testo ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agente desktop AI locale che combina dittatura vocale, chat LLM, generazione di immagini e automazione guidata dalla voce.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Dittatura vocale desktop per Windows che utilizza faster-whisper con simulazione della tastiera, VAD, PTT e punteggiatura.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dittatura vocale Whisper per KDE Wayland con daemon in background, servizio systemd e incolla dalla clipboard.

### Dittatura nativa per macOS

App di dittatura native per macOS sviluppate con Swift e WhisperKit, che supportano tasti di scelta rapida globali, barra dei menu e accelerazione tramite Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — App di trascrizione vocale per macOS con motori Whisper e Parakeet, tasti di scelta rapida globali ed elaborazione in batch.
- [Pindrop](https://github.com/watzon/pindrop) — App di dittatura nativa per macOS nella barra dei menu che utilizza WhisperKit per STT offline, con tasti di scelta rapida e pulizia AI opzionale.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Strumento di dittatura multilingue offline che utilizza Whisper, attivato da tasto di scelta rapida per trascrivere in qualsiasi campo di input.
- [FnKey](https://github.com/evoleinik/fnkey) — App nella barra dei menu di macOS che trascrive il parlato tramite Deepgram Nova-3 mentre si tiene premuto Fn e incolla il risultato.
- [hush](https://github.com/djmunro/hush) — App di dittatura push-to-talk per macOS che utilizza Whisper/Parakeet ONNX locale con incolla automatico tramite tasto di scelta rapida.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — App di dittatura nella barra dei menu di macOS che utilizza Whisper offline con accelerazione GPU Metal e inserimento del testo al cursore.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — App nella barra dei menu di Apple macOS che registra al rilascio di Globe/Fn, trascrive tramite faster-whisper e incolla al cursore.

### Pulizia del parlato con AI / post-elaborazione LLM

Strumenti di dittatura che utilizzano LLM locali o cloud per lucidare, formattare, riassumere e rielaborare l'output del riconoscimento vocale in testo pulito e formale.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — App di dittatura per macOS con STT su dispositivo e cloud, tasti di scelta rapida globali, flussi di lavoro AI, plugin, REST API e CLI.
- [Amical](https://github.com/amicalhq/amical) — App di dittatura AI local-first che utilizza Whisper per la trascrizione offline e Ollama per l'elaborazione intelligente delle note.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Strumento di dittatura vocale offline per macOS/Windows che utilizza Whisper, con tasti di scelta rapida globali e miglioramento AI opzionale.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Assistente vocale local-first per macOS e Linux con push-to-talk, trascrizione ed estrazione tramite plugin.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — App di dittatura push-to-talk per macOS che utilizza Whisper e pulizia LLM, incollando testo rifinito tramite Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Dittatura vocale locale con rifinitura LLM tramite Whisper, push-to-talk, dizionario e separazione client-server.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Dittatura vocale locale e registratore di riunioni con faster-whisper, riassunti LLM e registrazione audio su due tracce.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — App di riconoscimento vocale in testo nativa per macOS che utilizza modelli whisper.cpp locali, con scorciatoie globali e modalità sensibili al contesto.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — App di dittatura per macOS con riconoscimento vocale su dispositivo e post-elaborazione AI opzionale per la formattazione.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — App desktop di trascrizione vocale con tasti di scelta rapida, assistente AI, diarizzazione di riunioni e ricerca semantica.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — App nella barra dei menu di macOS per il riconoscimento vocale in testo offline e i riassunti di riunioni utilizzando Whisper e Qwen su Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — App di digitazione vocale multipiattaforma basata su Tauri con Whisper locale o Groq, pulizia AI, glossario e assistente vocale.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Assistente di dittatura vocale multipiattaforma con formattazione LLM, che supporta Whisper locale, Ollama o API cloud.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — App multipiattaforma basata su Tauri per la digitazione vocale AI, la riscrittura del testo e domande/risposte vocali con tasti di scelta rapida globali.
- [Aria](https://github.com/Xingxun7777/Aria) — Input vocale AI per Windows che utilizza Qwen3-ASR offline con contesto OCR, correzione di parole chiave e comandi vocali.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Dittatura vocale per Windows che utilizza whisper.cpp, Groq o llama.cpp, più stili e incolla automatico nella finestra attiva.
- [localflow](https://github.com/sidharth-n/localflow) — Dittatura vocale locale multipiattaforma che utilizza Moonshine STT, rifinitore Qwen3-4B, push-to-talk e skip-gate.
- [yammer](https://github.com/andynu/yammer) — Riconoscimento vocale in testo locale per Linux con Whisper e pulizia LLM, più interfaccia overlay Tauri e iniezione di input xdotool.

### Motori e toolkit STT locali/offline

Motori ASR offline e toolkit vocali per l'integrazione nelle app: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech e SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Port ad alte prestazioni in C/C++ di OpenAI Whisper con inferenza CPU/GPU, quantizzazione e supporto multipiattaforma.
- [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industriale con Paraformer, SenseVoice, VAD, diarizzazione, streaming e API compatibile con OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Toolkit di riconoscimento vocale offline con piccoli modelli solo CPU per più di 20 lingue e binding multi-lingua.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Toolkit vocale offline che utilizza Kaldi di nuova generazione e ONNX Runtime per STT, TTS, identificazione dell'altoparlante, VAD e altro.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Toolkit vocale completo con ASR, TTS, impronta vocale, diarizzazione, traduzione e servizi di streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Modello vocale con ASR per più di 50 lingue, emozioni, eventi audio e inferenza non autoregressiva rapida.

### Input vocale a livello di sistema / IME

Soluzioni di input vocale integrate a livello di sistema, tra cui metodi di input, estensioni IBus/Fcitx, IME Android e tastiere iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android e servizio di input vocale che utilizza Whisper per il riconoscimento vocale offline e la traduzione in inglese.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — App di dittatura vocale offline per Linux con motori whisper.cpp, Whisper e VOSK, GPU Vulkan e interfaccia GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Estensione per GNOME Shell per l'input vocale offline tramite whisper.cpp con attivatore da tasto di scelta rapida, che supporta X11 e Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Servizio di riconoscimento vocale offline per Android che utilizza Vosk con supporto per le API standard RecognitionService.
- [Dictus](https://github.com/getdictus/dictus-ios) — Tastiera iOS open-source per la dittatura vocale su dispositivo che utilizza WhisperKit e CoreML, funziona in qualsiasi app.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Metodo di input IBus di riconoscimento vocale in testo per Linux con STT in streaming, perfezionamento Whisper opzionale e accelerazione GPU.

### Input vocale cinese / IME

Progetti ottimizzati per il riconoscimento e l'input vocale cinesi, comprese IME e tastiere cinesi basate su FunASR, Paraformer e SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Input vocale cinese offline per Linux che utilizza FunASR Paraformer, IBus/Fcitx5, tasto di scelta rapida PTT e rifinitura delle frasi.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Metodo di input vocale offline multipiattaforma che utilizza FunASR, con correzione di parole chiave, incolla automatico e modalità GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Tastiera di input vocale per Android con 11 motori ASR, post-elaborazione LLM, pallino fluttuante e interfaccia Material3.

### Input vocale per browser e web

Input vocale basato su browser tramite estensioni, wrapper WebAssembly o interfacce Web, che richiede tipicamente un backend STT locale o cloud.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — WebUI Gradio per Whisper per sottotitoli da file, YouTube o microfono, con VAD, separazione BGM e diarizzazione.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Estensione per browser per il riconoscimento vocale in testo offline in tempo reale tramite Vosk, con comandi vocali in arabo e inglese.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Libreria di riconoscimento vocale offline basata su browser che impacchetta Vosk come WebAssembly eseguito in un WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Estensione per browser e server Whisper locale per il riconoscimento vocale in testo offline in Firefox e Chrome tramite Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Estensione per Chrome che registra la voce tramite tasto di scelta rapida, trascrive con l'API OpenAI Whisper e incolla automaticamente il testo.
- [voico](https://github.com/Kirera-Wainaina/voico) — Estensione per Chrome per l'input vocale in testo nei campi web, con backend Node.js che utilizza STT di Google e OpenAI.

### Input vocale mobile (non IME)

App autonome di trascrizione vocale su Android o iOS, piuttosto che tastiere come metodo di input.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Tastiera privata di riconoscimento vocale su dispositivo per Android che utilizza Whisper tramite whisper.cpp e Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — App iOS open-source per la trascrizione vocale offline che utilizza Whisper.cpp, con registrazione ed esportazione audio.
- [seamless](https://github.com/woheller69/seamless) — App di traduzione offline da parlato a testo per Android che utilizza Meta Seamless M4T Lite per 5 lingue con output TTS.

### Script leggeri, CLI e controllo vocale

Script leggeri, strumenti CLI, trigger nel vassoio o utilità adatti all'integrazione da parte degli sviluppatori o come integrazioni di toolchain esistenti.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Strumento offline di riconoscimento vocale per Linux che utilizza Vosk e simula l'input da tastiera in qualsiasi applicazione.
- [voice_typing](https://github.com/themanyone/voice_typing) — Script Bash per la digitazione vocale offline tramite Whisper per TTY, X11, Wayland e WSL con modifica LLM opzionale.
- [hns](https://github.com/primaprashant/hns) — Strumento CLI per il riconoscimento vocale in testo dal microfono locale che utilizza faster-whisper, con copia negli appunti e piping su stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Gestore GUI PyQt6 per nerd-dictation con vassoio di sistema, modelli Vosk, simulazione di input e tasti di scelta rapida KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Strumento di controllo vocale e digitazione basato su comandi che utilizza Kaldi e Dragonfly per un riconoscimento vocale completamente locale.

### Altro

Progetti non ancora assegnati a una categoria.

- [VoxType](https://github.com/peteonrails/voxtype) — Dittatura vocale push-to-talk per Linux e Wayland con sette motori ASR locali, supporto GPU e modalità riunione.

## Open-source vs benchmark

| Progetto | Prezzo | Open Source | Estendibile | Offline | Cinese |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Free (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Free (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(chiuso)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(chiuso)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(chiuso)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Come scegliere

- **App desktop multipiattaforma rifinita** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 stars, Whisper/Parakeet offline.
- **Linux offline minimale, scriptabile** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simula l'input da tastiera in qualsiasi app.
- **Integra STT nella tua app** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, integrabile.
- **Input orientato al cinese** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; input vocale cinese offline per Linux che utilizza FunASR Paraformer, IBus/Fcitx5, tasto di scelta rapida PTT e rifinitura delle frasi.
- **Self-hosting di un API/server di trascrizione** → [FunASR](https://github.com/modelscope/FunASR) — Toolkit ASR industriale con Paraformer, SenseVoice, VAD, diarizzazione, streaming e API compatibile con OpenAI.

## Contributi

I contributi sono benvenuti — vedi [CONTRIBUTING.md](CONTRIBUTING.md). I progetti devono essere completamente open source, estensibili e leggeri; segui la guida di stile per le descrizioni (in inglese, una riga, oggettiva, senza fronzoli di marketing).

## Cronologia delle Stelle

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Crescita delle stelle nel tempo per i progetti più stellati di questa lista, incluso questo repository.

## Licenza

[MIT](LICENSE).

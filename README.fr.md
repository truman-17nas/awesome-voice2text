# Awesome Voice Input

> Une liste organisée de logiciels open-source de saisie vocale / dictée — entièrement ouverts, extensibles et légers. Évaluée par rapport à Typeless, Lazytype et Shandianshuo (闪电说), toutes propriétaires.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Si cette liste est utile, veuillez ⭐ le dépôt — cela aide les autres à le trouver.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · **Français** · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Table des matières

- [Références (Propriétaires)](#références-propriétaires)
- [Pourquoi cette liste](#pourquoi-cette-liste)
- [Critères d'inclusion](#critères-dinclusion)
- [Sélections principales](#sélections-principales)
- [Tous les projets](#tous-les-projets)
- [Liste catégorisée](#liste-catégorisée)
  - [Dictée en temps réel multiplateforme pour bureau](#dictée-en-temps-réel-multiplateforme-pour-bureau)
  - [Dictée native macOS](#dictée-native-macos)
  - [Nettoyage de la parole par IA et post-traitement LLM](#nettoyage-de-la-parole-par-ia-et-post-traitement-llm)
  - [Moteurs et boîtes à outils STT locaux et hors ligne](#moteurs-et-boîtes-à-outils-stt-locaux-et-hors-ligne)
  - [Saisie vocale au niveau système et IME](#saisie-vocale-au-niveau-système-et-ime)
  - [Saisie vocale chinoise et IME](#saisie-vocale-chinoise-et-ime)
  - [Saisie vocale pour navigateur et Web](#saisie-vocale-pour-navigateur-et-web)
  - [Saisie vocale mobile (non-IME)](#saisie-vocale-mobile-non-ime)
  - [Scripts légers, CLI et contrôle vocal](#scripts-légers-cli-et-contrôle-vocal)
  - [Autres](#autres)
- [Open-source vs références](#open-source-vs-références)
- [Comment choisir](#comment-choisir)
- [Contribuer](#contribuer)
- [Historique des Étoiles](#historique-des-étoiles)
- [Licence](#licence)

## Références (Propriétaires)

| Produit | Tarification | Plateformes | Modèle/Moteur | Open Source |
| --- | --- | --- | --- | --- |
| Typeless | Freemium : 8K mots/semaine gratuits ; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | API IA cloud (propriétaire) | ❌ |
| Lazytype | Personnel €25 one-time (BYOK Groq) ; Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo sur Groq ; whisper.cpp local | ❌ |
| Shandianshuo (闪电说) | Gratuit (local/BYOK) ; Pro ¥29/mo ou ¥238.8/yr | macOS, Windows, Linux ; Android bêta | SenseVoiceSmall (local) + ASR cloud | ❌ |

## Pourquoi cette liste

Typeless, Lazytype et Shandianshuo (闪电说) sont puissants mais propriétaires. Cette liste rassemble des alternatives open-source qui répondent à trois critères : le code est entièrement public, l'outil peut être étendu et il reste suffisamment léger pour fonctionner sur une machine personnelle. Elle couvre actuellement **75 projets dans 9 catégories**, tous vérifiés comme étant entièrement open-source.

## Critères d'inclusion

- ✅ **Entièrement open-source** — tout le code sur une forge publique (GitHub, GitLab, Codeberg).
- 🔌 **Extensible** — vous pouvez ajouter les fonctionnalités, modèles ou intégrations que vous souhaitez.
- ⚡ **Léger** — sans gonflement, démarrage rapide, empreinte réduite.

## Sélections principales

🏆 **[Handy](https://github.com/cjpais/Handy)** — Outil de saisie vocale hors ligne multiplateforme utilisant Whisper ou Parakeet, avec raccourcis globaux et collage dans le presse-papiers. *Vaisseau amiral de la communauté — 25,281 stars, l'offre la plus aboutie.*

**Sélections fit-5** (répondent aux trois critères) :
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Port C/C++ haute performance d'OpenAI Whisper avec inférence CPU/GPU, quantification et prise en charge multiplateforme.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Outil de synthèse vocale hors ligne pour Linux utilisant Vosk, qui simule la saisie clavier dans toute application.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Saisie vocale push-to-talk pour Linux et Wayland avec sept moteurs ASR locaux, prise en charge GPU et mode réunion.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Script Bash pour la saisie vocale hors ligne via Whisper pour TTY, X11, Wayland et WSL avec édition LLM optionnelle.

## Tous les projets

| Nom | ⭐ Étoiles | Licence | Langage | Fit | Open | Ext | LW | Chinois |
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

## Liste catégorisée

### Dictée en temps réel multiplateforme pour bureau

Applications de dictée pour bureau basées sur Whisper pour Linux, Windows ou multiplateforme, avec push-to-talk, transcription locale et saisie automatique.

- [Handy](https://github.com/cjpais/Handy) — Outil de saisie vocale hors ligne multiplateforme utilisant Whisper ou Parakeet, avec raccourcis globaux et collage dans le presse-papiers.
- [Buzz](https://github.com/chidiwilliams/buzz) — Interface graphique de bureau multiplateforme pour la transcription et la traduction Whisper hors ligne avec accélération GPU et micro en direct.
- [Vibe](https://github.com/thewh1teagle/vibe) — Application de bureau multiplateforme pour la transcription audio et vidéo hors ligne utilisant Whisper, avec accélération GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Boîte à outils d'applications local-first avec stockage Markdown/SQLite, synchronisation Yjs CRDT et utilitaire de synthèse vocale pour bureau.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Synthèse vocale native Linux avec Whisper local et modèles ONNX, APIs cloud, intégration Waybar et visualiseur.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Application de dictée pour bureau utilisant Whisper localement ou via API, déclenchée par un raccourci global pour taper dans la fenêtre active.
- [Chirp](https://github.com/Whamp/chirp-stt) — Application de dictée Windows uniquement CPU utilisant ParakeetV3, avec bascule par raccourci, collage dans le presse-papiers et remplacements de mots.
- [Dabri](https://github.com/AshBuk/dabri) — Application STT hors ligne pour Linux utilisant whisper.cpp avec modes daemon, CLI et WebSocket pour bureaux X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Application de prise de notes hors ligne pour Linux et Sailfish OS avec STT local, TTS et traduction utilisant plusieurs moteurs.
- [voxd](https://github.com/jakovius/voxd) — Dictée vocale de bureau Linux utilisant whisper.cpp pour ASR hors ligne avec frappe ydotool et post-traitement IA.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Saisie vocale hors ligne Linux via Whisper, Parakeet ou Canary ONNX, avec prise en charge X11/Wayland et polissage LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Assistant de saisie vocale Windows utilisant le raccourci Verr. Maj., avec STT multi-fournisseurs et affinement LLM optionnel.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Application de dictée hors ligne multiplateforme avec distil-whisper, contrôle par raccourci et assistant LLM local optionnel.
- [TalkType](https://github.com/lmacan1/talktype) — Saisie vocale push-to-talk multiplateforme utilisant faster-whisper, avec raccourcis globaux et collage intelligent.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Application de dictée multilingue hors ligne utilisant Faster-Whisper, déclenchée par raccourci pour transcrire dans le champ actif.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Dictée vocale locale pour NixOS/Wayland utilisant whisper.cpp avec retour visuel GTK4 et prise en charge de 99 langues.
- [freespeak](https://github.com/Zetaphor/freespeak) — Application de dictée vocale Linux Wayland avec STT, correction grammaticale via LanguageTool et saisie de texte ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Agent de bureau IA local combinant dictée vocale, chat LLM, génération d'images et automatisation pilotée par la voix.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Synthèse vocale de bureau Windows utilisant faster-whisper avec simulation clavier, VAD, PTT et ponctuation.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Dictée vocale Whisper pour KDE Wayland avec daemon en arrière-plan, service systemd et collage dans le presse-papiers.

### Dictée native macOS

Applications de dictée natives macOS développées avec Swift et WhisperKit, prenant en charge les raccourcis globaux, la barre de menus et l'accélération par Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Application de transcription vocale macOS avec moteurs Whisper et Parakeet, raccourcis globaux et traitement par lots.
- [Pindrop](https://github.com/watzon/pindrop) — Application de dictée native macOS dans la barre de menus utilisant WhisperKit pour STT hors ligne, avec raccourcis et nettoyage IA optionnel.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Outil de dictée multilingue hors ligne utilisant Whisper, déclenché par raccourci pour transcrire dans n'importe quel champ de saisie.
- [FnKey](https://github.com/evoleinik/fnkey) — Application de barre de menus macOS qui transcrit la parole via Deepgram Nova-3 tant que Fn est maintenu et colle le résultat.
- [hush](https://github.com/djmunro/hush) — Application de dictée push-to-talk macOS utilisant Whisper/Parakeet ONNX locaux avec collage automatique via raccourci.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Application de dictée macOS dans la barre de menus utilisant Whisper hors ligne avec accélération GPU Metal et injection de texte au curseur.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Application macOS dans la barre de menus enregistre au relâchement de Globe/Fn, transcrit via faster-whisper et colle au curseur.

### Nettoyage de la parole par IA et post-traitement LLM

Outils de dictée utilisant des LLM locaux ou cloud pour polir, formater, résumer et restyliser la sortie de reconnaissance vocale en texte propre et formel.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Application de dictée macOS avec STT sur appareil et cloud, raccourcis globaux, workflows IA, plugins, API REST et CLI.
- [Amical](https://github.com/amicalhq/amical) — Application de dictée IA local-first utilisant Whisper pour la transcription hors ligne et Ollama pour le traitement intelligent de notes.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Outil de dictée vocale hors ligne pour macOS/Windows utilisant Whisper, avec raccourcis globaux et amélioration IA optionnelle.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Assistant vocal local-first pour macOS et Linux avec push-to-talk, transcription et extraction par plugins.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Application de dictée push-to-talk macOS utilisant Whisper et nettoyage LLM, collant le texte poli via Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Dictée vocale locale avec Whisper et polissage LLM, push-to-talk, dictionnaire et architecture client-serveur.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Dictée vocale locale et enregistreur de réunions avec faster-whisper, résumés LLM et capture audio double piste.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Application de saisie vocale native macOS utilisant des modèles whisper.cpp locaux, avec raccourcis globaux et modes contextuels.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Application de dictée macOS avec reconnaissance vocale sur appareil et post-traitement IA optionnel pour le formatage.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Application de bureau de transcription vocale avec raccourcis, assistant IA, diarisation de réunions et recherche sémantique.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Application de barre de menus macOS pour la synthèse vocale hors ligne et les résumés de réunions utilisant Whisper et Qwen sur Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Application de saisie vocale multiplateforme Tauri avec Whisper local ou Groq, nettoyage IA, glossaire et assistant vocal.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Assistant de dictée vocale multiplateforme avec formatage LLM, prenant en charge Whisper local, Ollama ou APIs cloud.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Application multiplateforme Tauri pour la saisie vocale IA, la réécriture de texte et les questions-réponses vocales avec raccourcis globaux.
- [Aria](https://github.com/Xingxun7777/Aria) — Saisie vocale IA pour Windows utilisant Qwen3-ASR hors ligne avec contexte OCR, correction de mots-clés et commandes vocales.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Dictée vocale Windows utilisant whisper.cpp, Groq ou llama.cpp, plusieurs styles et collage automatique dans la fenêtre active.
- [localflow](https://github.com/sidharth-n/localflow) — Dictée vocale locale multiplateforme utilisant Moonshine STT, polisseur Qwen3-4B, push-to-talk et skip-gate.
- [yammer](https://github.com/andynu/yammer) — Synthèse vocale locale Linux avec Whisper et nettoyage LLM, plus interface de superposition Tauri et injection de saisie xdotool.

### Moteurs et boîtes à outils STT locaux et hors ligne

Moteurs ASR hors ligne et boîtes à outils vocales pour l'intégration d'applications : Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech et SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Port C/C++ haute performance d'OpenAI Whisper avec inférence CPU/GPU, quantification et prise en charge multiplateforme.
- [FunASR](https://github.com/modelscope/FunASR) — Boîte à outils ASR industrielle avec Paraformer, SenseVoice, VAD, diarisation, streaming et API compatible OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Boîte à outils de reconnaissance vocale hors ligne avec petits modèles CPU uniquement pour plus de 20 langues et bindings multilingues.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Boîte à outils vocale hors ligne utilisant Kaldi de nouvelle génération et ONNX Runtime pour STT, TTS, identification de locuteur, VAD et plus.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Boîte à outils vocale complète avec ASR, TTS, empreinte vocale, diarisation, traduction et services de streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Modèle de parole avec ASR pour plus de 50 langues, émotion, événements audio et inférence non autorégressive rapide.

### Saisie vocale au niveau système et IME

Solutions de saisie vocale intégrées au niveau système, incluant les méthodes de saisie, les extensions IBus/Fcitx, les IME Android et les claviers iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android et service de saisie vocale utilisant Whisper pour la reconnaissance vocale hors ligne et la traduction anglaise.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Application de dictée vocale hors ligne pour Linux avec les moteurs whisper.cpp, Whisper et VOSK, GPU Vulkan et interface GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Extension GNOME Shell pour la saisie vocale hors ligne via whisper.cpp avec déclenchement par raccourci, prenant en charge X11 et Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Service de reconnaissance vocale hors ligne pour Android utilisant Vosk avec prise en charge de l'API RecognitionService standard.
- [Dictus](https://github.com/getdictus/dictus-ios) — Clavier iOS open-source pour la dictée vocale sur appareil utilisant WhisperKit et CoreML, fonctionnant dans toute application.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Méthode de saisie vocale Linux IBus avec STT en streaming, affinement Whisper optionnel et accélération GPU.

### Saisie vocale chinoise et IME

Projets optimisés pour la reconnaissance et la saisie vocales chinoises, incluant les IME et claviers chinois basés sur FunASR, Paraformer et SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Saisie vocale chinoise hors ligne pour Linux utilisant FunASR Paraformer, IBus/Fcitx5, raccourci PTT et polissage de phrases.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Méthode de saisie vocale hors ligne multiplateforme utilisant FunASR, avec correction de mots-clés, collage automatique et modes GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Clavier de saisie vocale Android avec 11 moteurs ASR, post-traitement LLM, boule flottante et interface Material3.

### Saisie vocale pour navigateur et Web

Saisie vocale basée sur navigateur via extensions, wrappers WebAssembly ou interfaces Web, nécessitant généralement un backend STT local ou cloud.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — WebUI Gradio pour Whisper pour les sous-titres à partir de fichiers, YouTube ou micro, avec VAD, séparation BGM et diarisation.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Extension de navigateur pour la synthèse vocale hors ligne en temps réel via Vosk, avec commandes vocales en arabe et en anglais.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Bibliothèque de reconnaissance vocale hors ligne basée sur navigateur, empaquetant Vosk en WebAssembly s'exécutant dans un WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Extension de navigateur et serveur Whisper local pour la synthèse vocale hors ligne dans Firefox et Chrome via Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Extension Chrome qui enregistre la voix via raccourci, transcrit avec l'API OpenAI Whisper et colle automatiquement le texte.
- [voico](https://github.com/Kirera-Wainaina/voico) — Extension Chrome pour la saisie vocale dans les champs Web, avec un backend Node.js utilisant les STT Google et OpenAI.

### Saisie vocale mobile (non-IME)

Applications autonomes de transcription vocale sur Android ou iOS, plutôt que des claviers de méthode de saisie.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Clavier de reconnaissance vocale privée sur appareil pour Android utilisant Whisper via whisper.cpp et Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Application iOS open-source pour la transcription vocale hors ligne utilisant Whisper.cpp, avec enregistrement et export audio.
- [seamless](https://github.com/woheller69/seamless) — Application de traduction de synthèse vocale hors ligne pour Android utilisant Meta Seamless M4T Lite pour 5 langues avec sortie TTS.

### Scripts légers, CLI et contrôle vocal

Scripts légers, outils CLI, déclencheurs de barre d'état ou utilitaires adaptés à l'intégration par les développeurs ou comme compléments aux chaînes d'outils existantes.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Outil de synthèse vocale hors ligne pour Linux utilisant Vosk, qui simule la saisie clavier dans toute application.
- [voice_typing](https://github.com/themanyone/voice_typing) — Script Bash pour la saisie vocale hors ligne via Whisper pour TTY, X11, Wayland et WSL avec édition LLM optionnelle.
- [hns](https://github.com/primaprashant/hns) — Outil CLI pour la synthèse vocale locale depuis microphone utilisant faster-whisper, avec copie dans le presse-papiers et redirection stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Gestionnaire graphique PyQt6 pour nerd-dictation avec barre système, modèles Vosk, simulation de saisie et raccourcis KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Outil de contrôle vocal et de saisie basé sur des commandes utilisant Kaldi et Dragonfly pour une reconnaissance vocale entièrement locale.

### Autres

Projets non encore assignés à une catégorie.

- [VoxType](https://github.com/peteonrails/voxtype) — Saisie vocale push-to-talk pour Linux et Wayland avec sept moteurs ASR locaux, prise en charge GPU et mode réunion.

## Open-source vs références

| Projet | Prix | Open Source | Extensible | Hors ligne | Chinois |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Gratuit (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Gratuit (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Gratuit (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Gratuit (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Gratuit (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Gratuit (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(propriétaire)* | Freemium : 8K mots/semaine gratuits ; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(propriétaire)* | Personnel €25 one-time (BYOK Groq) ; Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(propriétaire)* | Gratuit (local/BYOK) ; Pro ¥29/mo ou ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Comment choisir

- **Application de bureau multiplateforme aboutie** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 stars, Whisper/Parakeet hors ligne.
- **Linux hors ligne minimal et scriptable** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, simule la saisie clavier dans toute application.
- **Intégrer du STT dans votre propre application** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, intégrable.
- **Saisie chinoise prioritaire** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell ; saisie vocale chinoise hors ligne pour Linux utilisant FunASR Paraformer, IBus/Fcitx5, raccourci PTT et polissage de phrases.
- **Héberger une API de transcription/serveur** → [FunASR](https://github.com/modelscope/FunASR) — Boîte à outils ASR industrielle avec Paraformer, SenseVoice, VAD, diarisation, streaming et API compatible OpenAI.

## Contribuer

Les contributions sont les bienvenues — voir [CONTRIBUTING.md](CONTRIBUTING.md). Les projets doivent être entièrement open source, extensibles et légers; veuillez suivre le guide de style des descriptions (en anglais, une ligne, factuel, pas de langage publicitaire superflu).

## Historique des Étoiles

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Évolution des étoiles au fil du temps pour les projets les plus étoilés de cette liste, y compris ce dépôt.

## Licence

[MIT](LICENSE).
# Awesome Voice2Text

> Açık kaynak ses girişi / dikte yazılımlarının özenle seçilmiş bir listesi — tamamen açık, genişletilebilir ve hafif. Typeless, Lazytype ve Shandianshuo (闪电说) ile karşılaştırıldı; bunların hepsi kapalı kaynak.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Bu liste faydalıysa, lütfen repoya ⭐ verin — başkalarının bulmasına yardımcı olur.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · **Türkçe** · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## İçindekiler

- [Benchmarkler (Kapalı Kaynak)](#benchmarkler-kapalı-kaynak)
- [Neden bu liste](#neden-bu-liste)
- [Ekleme kriterleri](#ekleme-kriterleri)
- [En İyi Seçimler](#en-iyi-seçimler)
- [Tüm Projeler](#tüm-projeler)
- [Kategorilenmiş Liste](#kategorilenmiş-liste)
  - [Çapraz Platform Masaüstü Gerçek Zamanlı Dikte](#çapraz-platform-masaüstü-gerçek-zamanlı-dikte)
  - [Yerel macOS Diktesi](#yerel-macos-diktesi)
  - [AI Konuşma Temizliği / LLM Son İşleme](#ai-konuşma-temizliği-llm-son-işleme)
  - [Yerel/Çevrimdışı STT Motorları ve Araç Setleri](#yerelçevrimdışı-stt-motorları-ve-araç-setleri)
  - [Sistem Seviyesi Ses Girişi / IME](#sistem-seviyesi-ses-girişi-ime)
  - [Çince Ses Girişi / IME](#çince-ses-girişi-ime)
  - [Tarayıcı ve Web Ses Girişi](#tarayıcı-ve-web-ses-girişi)
  - [Mobil Ses Girişi (IME Dışı)](#mobil-ses-girişi-ime-dışı)
  - [Hafif Betikler, CLI ve Ses Kontrolü](#hafif-betikler-cli-ve-ses-kontrolü)
  - [Diğer](#diğer)
- [Açık Kaynak vs. Benchmarkler](#açık-kaynak-vs-benchmarkler)
- [Nasıl Seçilir](#nasıl-seçilir)
- [Katkı](#katkı)
- [Yıldız Geçmişi](#yıldız-geçmişi)
- [Lisans](#lisans)

## Benchmarkler (Kapalı Kaynak)

| Ürün | Fiyatlandırma | Platformlar | Model/Motor | Açık Kaynak |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Neden bu liste

Typeless, Lazytype ve Shandianshuo (闪电说) güçlüdür ancak kapalı kaynaktır. Bu liste, üç kriteri karşılayan açık kaynak alternatifleri derler: kod tamamen kamuoyu açık, araç genişletilebilir ve kişisel bir makinede çalışacak kadar hafif kalır. Şu anda **75 projeyi 9 kategoride** kapsamaktadır ve hepsi tamamen açık kaynak olduğu doğrulanmıştır.

## Ekleme kriterleri

- ✅ **Tamamen açık kaynak** — tüm kod bir halka açık platformda (GitHub, GitLab, Codeberg).
- 🔌 **Genişletilebilir** — istediğiniz özellikleri, modelleri veya entegrasyonları ekleyebilirsiniz.
- ⚡ **Hafif** — minimal şişkinlik, hızlı başlangıç, küçük ayak izi.

## En İyi Seçimler

🏆 **[Handy](https://github.com/cjpais/Handy)** — Whisper veya Parakeet kullanan çapraz platform çevrimdışı konuşmadan metine aracı, genel kısayol tuşları ve panoya yapıştırma ile. *Topluluk amiral gemisi — 25,281 yıldız, en cilalı seçenek.*

**fit=5 seçimleri** (tüm üç kriteri karşılar):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Yüksek performanslı OpenAI Whisper C/C++ portu, CPU/GPU çıkarımı, kuantizasyon ve çapraz platform desteği ile.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Vosk kullanan Linux çevrimdışı konuşmadan metine aracı; herhangi bir uygulamaya klavye girişi simüle eder.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux ve Wayland bas-konuş konuşmadan metine, yedi yerel ASR motoru, GPU desteği ve toplantı modu ile.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — TTY, X11, Wayland ve WSL için Whisper ile çevrimdışı sesle yazma Bash betiği; isteğe bağlı LLM düzenleme ile.

## Tüm Projeler

| Ad | ⭐ Yıldız | Lisans | Dil | Uygunluk | Açık | Gen | Hafif | Çince |
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

## Kategorilenmiş Liste

### Çapraz Platform Masaüstü Gerçek Zamanlı Dikte

Whisper tabanlı Linux, Windows veya çapraz platform masaüstü dikte uygulamaları, bas-konuş, yerel transkripsiyon ve otomatik giriş ile.

- [Handy](https://github.com/cjpais/Handy) — Whisper veya Parakeet kullanan çapraz platform çevrimdışı konuşmadan metine aracı, genel kısayol tuşları ve panoya yapıştırma ile.
- [Buzz](https://github.com/chidiwilliams/buzz) — Çapraz platform masaüstü arayüzü, çevrimdışı Whisper transkripsiyonu ve çevirisi, GPU hızlandırması, canlı mikrofon ile.
- [Vibe](https://github.com/thewh1teagle/vibe) — Whisper kullanan çapraz platform masaüstü uygulaması, çevrimdışı ses ve video transkripsiyonu, GPU hızlandırması ile.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Yerel öncelikli uygulama araç seti, Markdown/SQLite depolama, Yjs CRDT senkronizasyonu ve masaüstü konuşmadan metine yardımcı programı ile.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Linux tabanlı konuşmadan metine, yerel Whisper ve ONNX modelleri, bulut API'leri, Waybar entegrasyonu, görselleştirici ile.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Whisper'ı yerel veya API üzerinden kullanan masaüstü dikte uygulaması, etkin pencereye yazmak için genel kısayol tuşu ile tetiklenir.
- [Chirp](https://github.com/Whamp/chirp-stt) — Yalnızca CPU Windows dikte uygulaması, ParakeetV3 kullanır, kısayol tuşu ile aç/kapat, panoya yapıştırma ve kelime geçersiz kılma ile.
- [Dabri](https://github.com/AshBuk/dabri) — whisper.cpp kullanan Linux çevrimdışı STT uygulaması, arka plan hizmeti, CLI ve WebSocket modları ile X11/Wayland masaüstleri için.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux ve Sailfish OS çevrimdışı not alma uygulaması, çoklu motorlar ile yerel STT, TTS ve çeviri.
- [voxd](https://github.com/jakovius/voxd) — whisper.cpp kullanan Linux masaüstü ses dikte, çevrimdışı ASR, ydotool yazma ve AI son işleme ile.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Whisper, Parakeet veya Canary ONNX ile Linux çevrimdışı sesle yazma, X11/Wayland desteği ve LLM düzenleme ile.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Caps Lock kısayol tuşu kullanan Windows sesle yazma asistanı, çok sağlayıcılı STT ve isteğe bağlı LLM iyileştirme ile.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — distil-whisper, kısayol tuşu kontrolü ve isteğe bağlı yerel LLM asistanı ile çapraz platform çevrimdışı dikte uygulaması.
- [TalkType](https://github.com/lmacan1/talktype) — faster-whisper kullanan çapraz platform bas-konuş sesle yazma, genel kısayol tuşları ve akıllı yapıştırma ile.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Faster-Whisper kullanan çevrimdışı çok dilli dikte uygulaması, etkin alana transkripsiyon için kısayol tuşu ile tetiklenir.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — whisper.cpp kullanan NixOS/Wayland yerel ses dikte, GTK4 geri bildirimi ve 99 dil desteği ile.
- [freespeak](https://github.com/Zetaphor/freespeak) — Linux Wayland ses dikte uygulaması, STT, LanguageTool ile dil bilgisi düzeltmesi ve ydotool metin girişi.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Ses dikte, LLM sohbet, görüntü oluşturma ve sesle otomasyonu birleştiren yerel AI masaüstü aracı.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — faster-whisper kullanan Windows masaüstü konuşmadan metine, klavye simülasyonu, VAD, PTT ve noktalama ile.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — KDE Wayland için Whisper ses dikte, arka plan aracı, systemd hizmeti ve panoya yapıştırma ile.

### Yerel macOS Diktesi

Yerel macOS dikte uygulamaları Swift ve WhisperKit ile yapılmıştır, genel kısayol tuşları, menü çubuğu ve Neural Engine hızlandırmasını destekler.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Whisper ve Parakeet motorları, genel kısayol tuşları ve toplu işleme ile macOS konuşma transkripsiyon uygulaması.
- [Pindrop](https://github.com/watzon/pindrop) — WhisperKit kullanan yerel macOS menü çubuğu dikte uygulaması, çevrimdışı STT, kısayol tuşları ve isteğe bağlı AI temizliği ile.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Çevrimdışı çok dilli dikte uygulaması, Whisper kullanır, etkin alana transkripsiyon için kısayol tuşu ile tetiklenir.
- [FnKey](https://github.com/evoleinik/fnkey) — Fn basılı tutulduğunda Deepgram Nova-3 ile konuşmayı transkripsiyon eden ve sonucu yapıştıran macOS menü çubuğu uygulaması.
- [hush](https://github.com/djmunro/hush) — Yerel Whisper/Parakeet ONNX kullanan macOS bas-konuş dikte uygulaması, kısayol tuşu ile otomatik yapıştırma.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Çevrimdışı Whisper kullanan macOS menü çubuğu dikte uygulaması, Metal GPU hızlandırması ve imleç metin enjeksiyonu.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS menü çubuğu uygulaması, Globe/Fn bırakıldığında kaydeder, faster-whisper ile transkripsiyon eder ve imleçte yapıştırır.

### AI Konuşma Temizliği / LLM Son İşleme

Yerel veya bulut LLM'leri kullanan dikte araçları, konuşma tanıma çıktısını temiz, resmi metne parlatmak, biçimlendirmek, özetlemek ve yeniden stilize etmek için.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Cihaz içi ve bulut STT, genel kısayol tuşları, AI iş akışları, eklentiler, REST API ve CLI ile macOS dikte uygulaması.
- [Amical](https://github.com/amicalhq/amical) — Yerel öncelikli AI dikte uygulaması, çevrimdışı transkripsiyon için Whisper ve akıllı not işleme için Ollama kullanır.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Whisper kullanan macOS/Windows için çevrimdışı ses dikte aracı, genel kısayol tuşları ve isteğe bağlı AI geliştirmesi ile.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Yerel öncelikli sesli asistan, macOS ve Linux için bas-konuş, transkripsiyon ve eklenti çıkarma ile.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Whisper ve LLM temizliği kullanan macOS bas-konuş dikte uygulaması, cilalanmış metni Cmd-V ile yapıştırır.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Whisper ve LLM düzenleme ile yerel ses dikte, bas-konuş, sözlük ve istemci-sunucu ayrımı.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — faster-whisper, LLM özetleri ve çift kanallı ses kaydı ile yerel ses dikte ve toplantı kaydedici.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Yerel whisper.cpp modelleri kullanan yerel macOS konuşmadan metine uygulaması, genel kısayollar ve bağlama duyarlı modlar ile.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Cihaz üzerinde konuşma tanıma ve isteğe bağlı AI son işleme ile biçimlendirme için macOS dikte uygulaması.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Kısayol tuşları, AI asistanı, toplantı konuşmacı ayrımı ve anlamsal arama ile masaüstü ses transkripsiyonu uygulaması.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Apple Silicon üzerinde Whisper ve Qwen kullanarak çevrimdışı konuşmadan metine ve toplantı özetleri için macOS menü çubuğu uygulaması.
- [Voquill](https://github.com/voquill/voquill) — Yerel Whisper veya Groq, AI temizliği, sözlük ve sesli asistan ile çapraz platform Tauri sesle yazma uygulaması.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — LLM biçimlendirme ile çapraz platform ses dikte asistanı, yerel Whisper, Ollama veya bulut API'lerini destekler.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — AI sesle yazma, metin yeniden yazma ve sesli soru-cevap için genel kısayol tuşları ile çapraz platform Tauri uygulaması.
- [Aria](https://github.com/Xingxun7777/Aria) — OCR bağlamı, sıcak kelime düzeltmesi ve sesli komutlar ile çevrimdışı Qwen3-ASR kullanan Windows AI ses girişi.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — whisper.cpp, Groq veya llama.cpp kullanan Windows ses dikte, çoklu stiller, etkin pencereye otomatik yapıştırma.
- [localflow](https://github.com/sidharth-n/localflow) — Moonshine STT, Qwen3-4B düzenleyici, bas-konuş ve atlama kapısı ile yerel çapraz platform ses dikte.
- [yammer](https://github.com/andynu/yammer) — Whisper ve LLM temizliği ile Linux yerel konuşmadan metine, ayrıca Tauri bindirmeli arayüz ve xdotool giriş enjeksiyonu.

### Yerel/Çevrimdışı STT Motorları ve Araç Setleri

Çevrimdışı ASR motorları ve uygulama entegrasyonu için konuşma araç setleri: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech ve SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Yüksek performanslı OpenAI Whisper C/C++ portu, CPU/GPU çıkarımı, kuantizasyon ve çapraz platform desteği ile.
- [FunASR](https://github.com/modelscope/FunASR) — Endüstriyel ASR araç seti, Paraformer, SenseVoice, VAD, konuşmacı ayrımı, akış ve OpenAI uyumlu API ile.
- [vosk-api](https://github.com/alphacep/vosk-api) — Çevrimdışı konuşma tanıma araç seti, 20+ dil için yalnızca CPU küçük modelleri ve çok dilli bağlamalar ile.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Çevrimdışı konuşma araç seti, STT, TTS, konuşmacı tanıma, VAD ve daha fazlası için yeni nesil Kaldi ve ONNX Runtime kullanır.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Kapsamlı konuşma araç seti, ASR, TTS, ses izi, konuşmacı ayrımı, çeviri ve akış hizmetleri.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — 50+ dil için ASR, duygu, ses olayları ve hızlı non-autoregressive çıkarım ile konuşma modeli.

### Sistem Seviyesi Ses Girişi / IME

Giriş yöntemleri, IBus/Fcitx eklentileri, Android IME ve iOS klavyeleri dahil sistem seviyesinde entegre ses girişi çözümleri.

- [Whisper IME](https://github.com/woheller69/whisperIME) — Whisper kullanan Android IME ve ses girişi hizmeti, çevrimdışı konuşma tanıma ve İngilizce çeviri ile.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — whisper.cpp, Whisper ve VOSK motorları, Vulkan GPU ve GTK arayüzü ile çevrimdışı Linux ses dikte uygulaması.
- [blurt](https://github.com/QuantiusBenignus/blurt) — whisper.cpp ile çevrimdışı ses girişi için GNOME Shell eklentisi, kısayol tuşu tetikleyicisi, X11 ve Wayland desteği.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Vosk kullanan Android çevrimdışı konuşma tanıma hizmeti, standart RecognitionService API desteği ile.
- [Dictus](https://github.com/getdictus/dictus-ios) — WhisperKit ve CoreML kullanan cihaz üzerinde ses dikte için açık kaynak iOS klavyesi, her uygulamada çalışır.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Akış STT, isteğe bağlı Whisper iyileştirme ve GPU hızlandırması ile Linux IBus konuşmadan metine giriş yöntemi.

### Çince Ses Girişi / IME

Çince konuşma tanıma ve giriş için optimize edilmiş projeler, FunASR, Paraformer ve SenseVoice tabanlı Çince IME'ler ve klavyeler.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — FunASR Paraformer, IBus/Fcitx5, PTT kısayol tuşu ve cümle düzenleme ile çevrimdışı Linux Çince ses girişi.
- [voice-input-method](https://github.com/pofice/voice-input-method) — FunASR kullanan çapraz platform çevrimdışı ses giriş yöntemi, sıcak kelime düzeltme, otomatik yapıştırma ve GUI/CLI modları.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — 11 ASR motoru, LLM son işleme, yüzen top ve Material3 arayüzü ile Android ses girişi klavyesi.

### Tarayıcı ve Web Ses Girişi

Eklentiler, WebAssembly sarmalayıcıları veya Web arayüzleri aracılığıyla tarayıcı tabanlı ses girişi, tipik olarak yerel veya bulut STT arka ucu gerektirir.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Dosyalardan, YouTube'dan veya mikrofondan altyazılar için Gradio Whisper WebUI, VAD, arka plan müziği ayrımı ve konuşmacı ayrımı ile.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Vosk aracılığıyla gerçek zamanlı çevrimdışı konuşmadan metine için tarayıcı eklentisi, Arapça ve İngilizce sesli komutlar.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — WebWorker içinde WebAssembly olarak Vosk paketleyen tarayıcı tabanlı çevrimdışı konuşma tanıma kütüphanesi.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Firefox ve Chrome'da Alt+A ile çevrimdışı konuşmadan metine için tarayıcı eklentisi ve yerel Whisper sunucusu.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Kısayol tuşu ile ses kaydeden, OpenAI Whisper API ile transkripsiyon eden ve metni otomatik yapıştıran Chrome eklentisi.
- [voico](https://github.com/Kirera-Wainaina/voico) — Web alanlarına sesli metin girişi için Chrome eklentisi, Google ve OpenAI STT kullanan Node.js arka ucu ile.

### Mobil Ses Girişi (IME Dışı)

Giriş yöntemi klavyeleri yerine bağımsız Android veya iOS ses transkripsiyon uygulamaları.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — whisper.cpp ve Silero VAD üzerinden Whisper kullanan Android için gizli, cihaz üzerinde konuşma tanıma klavyesi.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Whisper.cpp kullanan çevrimdışı ses transkripsiyonu için açık kaynak iOS uygulaması, kayıt ve ses dışa aktarımı ile.
- [seamless](https://github.com/woheller69/seamless) — Meta Seamless M4T Lite kullanan Android çevrimdışı konuşmadan metine çeviri uygulaması, 5 dil için TTS çıkışı ile.

### Hafif Betikler, CLI ve Ses Kontrolü

Geliştirici entegrasyonu için veya mevcut araç zincirlerine ekleme olarak uygun hafif betikler, CLI araçları, tepsi tetikleyicileri ve yardımcı programlar.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Vosk kullanan Linux çevrimdışı konuşmadan metine aracı; herhangi bir uygulamaya klavye girişi simüle eder.
- [voice_typing](https://github.com/themanyone/voice_typing) — TTY, X11, Wayland ve WSL için Whisper ile çevrimdışı sesle yazma Bash betiği; isteğe bağlı LLM düzenleme ile.
- [hns](https://github.com/primaprashant/hns) — faster-whisper kullanan yerel mikrofon konuşmadan metine CLI aracı, panoya kopyalama ve stdout borulama ile.
- [Elograf](https://github.com/papoteur-mga/elograf) — nerd-dictation için PyQt6 arayüz yöneticisi, sistem tepsisi, Vosk modelleri, giriş simülasyonu ve KDE kısayol tuşları ile.
- [Osprey](https://github.com/osprey-voice/osprey) — Kaldi ve Dragonfly kullanan tamamen yerel konuşma tanıma için komut tabanlı ses kontrolü ve yazma aracı.

### Diğer

Henüz bir kategoriye atanmamış projeler.

- [VoxType](https://github.com/peteonrails/voxtype) — Linux ve Wayland bas-konuş konuşmadan metine, yedi yerel ASR motoru, GPU desteği ve toplantı modu ile.

## Açık Kaynak vs. Benchmarkler

| Proje | Fiyat | Açık Kaynak | Genişletilebilir | Çevrimdışı | Çince |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Ücretsiz (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Nasıl Seçilir

- **Cilalı çapraz platform masaüstü uygulaması** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 stars, Whisper/Parakeet çevrimdışı.
- **Minimal Linux çevrimdışı, betiklenebilir** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, herhangi bir uygulamaya klavye girişi simüle eder.
- **STT'yi kendi uygulamanıza gömün** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, gömülebilir.
- **Önce Çince giriş** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; FunASR Paraformer, IBus/Fcitx5, PTT kısayol tuşu ve cümle düzenleme ile çevrimdışı Linux Çince ses girişi.
- **Bir transkripsiyon API/sunucusu kendiniz barındırın** → [FunASR](https://github.com/modelscope/FunASR) — Endüstriyel ASR araç seti, Paraformer, SenseVoice, VAD, konuşmacı ayrımı, akış ve OpenAI uyumlu API ile.

## Katkı

Katkılar memnuniyetle karşılanır — bkz. [CONTRIBUTING.md](CONTRIBUTING.md). Projeler tamamen açık kaynak, genişletilebilir ve hafif olmalıdır; lütfen açıklama stil kılavuzuna uyun (İngilizce olarak, tek satır, nesnel, pazarlama palavrası yok).

## Yıldız Geçmişi

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

Bu listedeki en çok yıldız alan projelerin zaman içindeki yıldız artışı, bu depo dahil.

## Lisans

[MIT](LICENSE).

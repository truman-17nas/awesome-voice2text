# Awesome Voice Input

> قائمة مختارة من برامج الإدخال الصوتي والإملاء مفتوحة المصدر — مفتوحة بالكامل، قابلة للتوسيع، وخفيفة الوزن. تقاس أداؤها مقابل Typeless و Lazytype و Shandianshuo (闪电说)، وجميعها مغلقة المصدر.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*إذا كانت هذه القائمة مفيدة، يُرجى ⭐ المستودع — فهذا يساعد الآخرين على العثور عليه.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · **العربية** · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## المحتويات

- [المعايير (برامج مغلقة المصدر)](#المعايير-برامج-مغلقة-المصدر)
- [لماذا هذه القائمة](#لماذا-هذه-القائمة)
- [معايير الضم](#معايير-الضم)
- [اختياراتنا المميزة](#اختياراتنا-المميزة)
- [جميع المشاريع](#جميع-المشاريع)
- [القائمة مصنفة](#القائمة-مصنفة)
  - [الإملاء الصوتي عبر منصات سطح المكتب في الوقت الفعلي](#الإملاء-الصوتي-عبر-منصات-سطح-المكتب-في-الوقت-الفعلي)
  - [الإملاء الصوتي الأصيل لنظام macOS](#الإملاء-الصوتي-الأصيل-لنظام-macos)
  - [تنقية الكلام بالذكاء الاصطناعي / المعالجة اللاحقة باستخدام نماذج اللغة الكبيرة](#تنقية-الكلام-بالذكاء-الاصطناعي-المعالجة-اللاحقة-باستخدام-نماذج-اللغة-الكبيرة)
  - [محركات وأدوات التحويل من كلام إلى نص محلي/غير متصل](#محركات-وأدوات-التحويل-من-كلام-إلى-نص-محليغير-متصل)
  - [إدخال الصوت على مستوى النظام / محركات الإدخال](#إدخال-الصوت-على-مستوى-النظام-محركات-الإدخال)
  - [إدخال الكلام الصيني / محركات الإدخال](#إدخال-الكلام-الصيني-محركات-الإدخال)
  - [إدخال الصوت عبر المتصفح والويب](#إدخال-الصوت-عبر-المتصفح-والويب)
  - [إدخال الصوت على الأجهزة المحمولة (غير محركات إدخال)](#إدخال-الصوت-على-الأجهزة-المحمولة-غير-محركات-إدخال)
  - [سكربتات خفيفة، سطر أوامر، والتحكم الصوتي](#سكربتات-خفيفة-سطر-أوامر-والتحكم-الصوتي)
  - [أخرى](#أخرى)
- [البرمجيات مفتوحة المصدر مقابل المعايير](#البرمجيات-مفتوحة-المصدر-مقابل-المعايير)
- [كيفية الاختيار](#كيفية-الاختيار)
- [المساهمة](#المساهمة)
- [تاريخ النجوم](#تاريخ-النجوم)
- [الترخيص](#الترخيص)

## المعايير (برامج مغلقة المصدر)

| المنتج | التسعير | المنصات | النموذج/المحرك | مفتوح المصدر |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## لماذا هذه القائمة

Typeless و Lazytype و Shandianshuo (闪电说) قوية لكنها مغلقة المصدر. تجمع هذه القائمة البدائل مفتوحة المصدر التي تستوفي ثلاثة معايير: الكود عام بالكامل، الأداة قابلة للتوسيع، وتظل خفيفة بما يكفي للعمل على آلة شخصية. تغطي حاليًا **75 مشروعًا في 9 فئات**، تم التحقق من جميعها بأنها مفتوحة المصدر بالكامل.

## معايير الضم

- ✅ **مفتوحة المصدر بالكامل** — كل الكود على منصة عامة (GitHub، GitLab، Codeberg).
- 🔌 **قابلة للتوسيع** — يمكنك إضافة الميزات أو النماذج أو التكاملات التي تريدها.
- ⚡ **خفيفة الوزن** — خالية من التضخم، تشغيل سريع، وآثار بسيطة.

## اختياراتنا المميزة

🏆 **[Handy](https://github.com/cjpais/Handy)** — أداة إدخال صوتي إلى نص غير متصلة تعمل عبر المنصات باستخدام Whisper أو Parakeet، مع مفاتيح اختصار عالمية واللصق من الحافظة. *الراية المجتمعية — 25,281 نجمة، العرض الأكثر تلميعًا.*

**اختيارات Fit-5** (تستوفي المعايير الثلاثة جميعها):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — إصدار C/C++ عالي الأداء من OpenAI Whisper مع استدلال CPU/GPU، التكميم، والدعم عبر المنصات.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — أداة Linux غير متصلة لتحويل الكلام إلى نص باستخدام Vosk تحاكي إدخال لوحة المفاتيح في أي تطبيق.
- **[VoxType](https://github.com/peteonrails/voxtype)** — إدخال صوتي إلى نص بنمط اضغط-وتكلم على Linux و Wayland مع سبع محركات ASR محلية، دعم GPU، ووضع الاجتماعات.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — سكربت Bash للكتابة الصوتية غير المتصلة عبر Whisper لـ TTY و X11 و Wayland و WSL مع تحرير اختياري باستخدام نماذج اللغة الكبيرة.

## جميع المشاريع

| الاسم | ⭐ النجوم | الترخيص | اللغة | Fit | مفتوح | قابل للتوسيع | خفيف | صيني |
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
| [Speechfire](https://github.com/Jejkobb/Speechfire) | 27 | لا يوجد | JavaScript, Python | 3 | ⚠️ | ✅ | ⚠️ | ◐ |
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

## القائمة مصنفة

### الإملاء الصوتي عبر منصات سطح المكتب في الوقت الفعلي

تطبيقات إملاء سطح مكتب مبنية على Whisper لنظام Linux أو Windows أو عبر المنصات، مع خاصية اضغط-وتكلم، والنسخ المحلي، والإدخال التلقائي.

- [Handy](https://github.com/cjpais/Handy) — أداة إدخال صوتي إلى نص غير متصلة تعمل عبر المنصات باستخدام Whisper أو Parakeet، مع مفاتيح اختصار عالمية واللصق من الحافظة.
- [Buzz](https://github.com/chidiwilliams/buzz) — واجهة رسومية لسطح المكتب عبر المنصات لنسخ Whisper وترجمته غير المتصل، مع تسريع GPU وميكروفون مباشر.
- [Vibe](https://github.com/thewh1teagle/vibe) — تطبيق سطح مكتب عبر المنصات لنسخ الصوت والفيديو غير المتصل باستخدام Whisper، مع تسريع GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — مجموعة أدوات تطبيقية محليًا مع تخزين Markdown/SQLite، ومزامنة Yjs CRDT، وأداة إملاء صوتي لسطح المكتب.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — إدخال صوتي إلى نص أصلي لنظام Linux باستخدام Whisper ونماذج ONNX المحلية، وواجهات برمجة التطبيقات السحابية، وتكامل Waybar، والمُصوّر.
- [whisper-writer](https://github.com/savbell/whisper-writer) — تطبيق إملاء سطح مكتب يستخدم Whisper محليًا أو عبر API، يُشغّله مفتاح اختصار عالمي لإدخال النص في النافذة النشطة.
- [Chirp](https://github.com/Whamp/chirp-stt) — تطبيق إملاء لنظام Windows يستخدم ParakeetV3 على CPU فقط، مع تبديل عبر مفتاح اختصار، واللصق من الحافظة، وتجاوز الكلمات.
- [Dabri](https://github.com/AshBuk/dabri) — تطبيق Linux غير متصل لـ STT باستخدام whisper.cpp مع daemon، CLI، ووضع WebSocket لأجهزة سطح المكتب X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — تطبيق Linux و Sailfish OS لتدوين الملاحظات غير المتصل مع STT و TTS وترجمة باستخدام محركات متعددة.
- [voxd](https://github.com/jakovius/voxd) — إملاء صوتي لسطح مكتب Linux باستخدام whisper.cpp لـ ASR غير المتصل مع الكتابة عبر ydotool والمعالجة اللاحقة بالذكاء الاصطناعي.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — كتابة صوتية غير متصلة على Linux عبر Whisper أو Parakeet أو Canary ONNX، مع دعم X11/Wayland وتلميع LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — مساعد كتابة صوتية لنظام Windows يستخدم مفتاح Caps Lock، مع STT متعدد المزودين وتحسين اختياري باستخدام LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — تطبيق إملاء غير متصل عبر المنصات مع distil-whisper، التحكم عبر مفتاح اختصار، ومساعد LLM محلي اختياري.
- [TalkType](https://github.com/lmacan1/talktype) — كتابة صوتية بنمط اضغط-وتكلم عبر المنصات باستخدام faster-whisper، مع مفاتيح اختصار عالمية واللصق الذكي.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — تطبيق إملاء متعدد اللغات غير متصل باستخدام Faster-Whisper، يُشغّله مفتاح اختصار للنسخ في الحقل النشط.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — إملاء صوتي محلي لنظام NixOS/Wayland باستخدام whisper.cpp مع واجهة GTK4 للملاحظات ودعم 99 لغة.
- [freespeak](https://github.com/Zetaphor/freespeak) — تطبيق إملاء صوتي لنظام Linux Wayland مع STT، وتصحيح القواعد عبر LanguageTool، وإدخال النص عبر ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — وكيل مكتبي محلي للذكاء الاصطناعي يجمع بين الإملاء الصوتي، ودردشة LLM، وتوليد الصور، والأتمتة الصوتية.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — إدخال صوتي إلى نص لسطح مكتب Windows باستخدام faster-whisper مع محاكاة لوحة المفاتيح، وVAD، وPTT، والترقيم.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — إملاء صوتي باستخدام Whisper لنظام KDE Wayland مع daemon في الخلفية، وخدمة systemd، واللصق من الحافظة.

### الإملاء الصوتي الأصيل لنظام macOS

تطبيقات إملاء أصيلة لنظام macOS مبنية باستخدام Swift و WhisperKit، تدعم مفاتيح الاختصار العالمية، وشريط القوائم، وتسريع Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — تطبيق macOS لنسخ الكلام باستخدام Whisper و Parakeet، ومفاتيح اختصار عالمية، والمعالجة الدفعة.
- [Pindrop](https://github.com/watzon/pindrop) — تطبيق إملاء أصيل لشريط القوائم في macOS يستخدم WhisperKit لـ STT غير المتصل، مع مفاتيح اختصار وتنظيف AI اختياري.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — أداة إملاء متعددة اللغات غير متصلة باستخدام Whisper، يُشغّلها مفتاح اختصار للنسخ في أي حقل إدخال.
- [FnKey](https://github.com/evoleinik/fnkey) — تطبيق macOS لشريط القوائم ينسخ الكلام عبر Deepgram Nova-3 أثناء الضغط على Fn ويلصق النتيجة.
- [hush](https://github.com/djmunro/hush) — تطبيق macOS بنمط اضغط-وتكلم للإملاء باستخدام Whisper/Parakeet ONNX محلي مع اللصق التلقائي عبر مفتاح اختصار.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — تطبيق macOS لشريط القوائم يستخدم Whisper غير المتصل مع تسريع GPU Metal وإدخال النص عند المؤشر.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — تطبيق macOS لشريط القوائم يسجل عند تحرير Globe/Fn، ينسخ عبر faster-whisper، ويلصق عند المؤشر.

### تنقية الكلام بالذكاء الاصطناعي / المعالجة اللاحقة باستخدام نماذج اللغة الكبيرة

أدوات إملاء تستخدم LLMs محلية أو سحابية لتلميع وتنسيق واختصار وإعادة صياغة مخرجات التعرف على الكلام إلى نص نظيف ورسمي.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — تطبيق macOS للإملاء مع STT على الجهاز وفي السحابة، ومفاتيح اختصار عالمية، وسير عمل AI، وإضافات، وREST API، وCLI.
- [Amical](https://github.com/amicalhq/amical) — تطبيق إملاء AI محلي أولًا يستخدم Whisper للنسخ غير المتصل وOllama لمعالجة الملاحظات الذكية.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — أداة إملاء صوتي غير متصلة لنظام macOS/Windows باستخدام Whisper، مع مفاتيح اختصار عالمية وتحسين AI اختياري.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — مساعد صوتي محلي أولًا لنظام macOS و Linux بنمط اضغط-وتكلم، ونسخ، واستخراج عبر الإضافات.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — تطبيق macOS بنمط اضغط-وتكلم يستخدم Whisper وتنظيف LLM، ويلصق النص المُلمَّع عبر Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — إملاء صوتي محلي مع Whisper وتلميع LLM، واضغط-وتكلم، وقاموس، وتقسيم عميل/خادم.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — إملاء صوتي محلي ومسجل اجتماعات مع faster-whisper، وملخصات LLM، والتقاط الصوت ثنائي المسار.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — تطبيق macOS أصيل لتحويل الصوت إلى نص باستخدام نماذج whisper.cpp محلية، مع اختصارات عالمية وأوضاع حساسة للسياق.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — تطبيق macOS للإملاء مع التعرف على الكلام على الجهاز والمعالجة اللاحقة الاختيارية بالذكاء الاصطناعي للتنسيق.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — تطبيق سطح مكتب لنسخ الصوت مع مفاتيح اختصار، ومساعد AI، وتقسيم المتحدثين في الاجتماعات، والبحث الدلالي.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — تطبيق macOS لشريط القوائم للإملاء الصوتي وملخصات الاجتماعات باستخدام Whisper و Qwen على Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — تطبيق Tauri عبر المنصات للكتابة الصوتية مع Whisper محلي أو Groq، وتنظيف AI، وقاموس، ومساعد صوتي.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — مساعد إملاء صوتي عبر المنصات مع تنسيق LLM، يدعم Whisper محلي، وOllama، أو واجهات API سحابية.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — تطبيق Tauri عبر المنصات للكتابة الصوتية بالذكاء الاصطناعي، وإعادة صياغة النص، وأسئلة/أجوبة صوتية مع مفاتيح اختصار عالمية.
- [Aria](https://github.com/Xingxun7777/Aria) — إدخال صوتي AI لنظام Windows باستخدام Qwen3-ASR غير المتصل مع سياق OCR، وتصحيح الكلمات المفتاحية، وأوامر صوتية.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — إملاء صوتي لنظام Windows باستخدام whisper.cpp، وGroq، أو llama.cpp، وأنماط متعددة، واللصق التلقائي في النافذة النشطة.
- [localflow](https://github.com/sidharth-n/localflow) — إملاء صوتي محلي عبر المنصات باستخدام Moonshine STT، ومُلمِّع Qwen3-4B، واضغط-وتكلم، وبوابة التخطي.
- [yammer](https://github.com/andynu/yammer) — تحويل كلام إلى نص محلي على Linux مع Whisper وتنظيف LLM، وواجهة Tauri فوقية، وإدخال عبر xdotool.

### محركات وأدوات التحويل من كلام إلى نص محلي/غير متصل

محركات ASR غير متصلة وأدوات الكلام للتكامل في التطبيقات: Whisper، Kaldi، ONNX، Vosk، FunASR، PaddleSpeech، و SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — إصدار C/C++ عالي الأداء من OpenAI Whisper مع استدلال CPU/GPU، التكميم، والدعم عبر المنصات.
- [FunASR](https://github.com/modelscope/FunASR) — مجموعة أدوات ASR صناعية مع Paraformer، SenseVoice، VAD، تقسيم المتحدثين، البث، وAPI متوافق مع OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — مجموعة أدوات التعرف على الكلام غير المتصل مع نماذج CPU صغيرة لـ 20+ لغة وروابط متعددة اللغات.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — مجموعة أدوات كلام غير متصلة تستخدم Kaldi الجيل التالي وONNX Runtime لـ STT و TTS ومعرفة المتحدث وVAD وغيرها.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — مجموعة أدوات كلام شاملة مع ASR و TTS وبصمة الصوت وتقسيم المتحدثين والترجمة وخدمات البث.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — نموذج كلام مع ASR لـ 50+ لغة، والعواطف، والأحداث الصوتية، والاستدلال غير التلقائي السريع.

### إدخال الصوت على مستوى النظام / محركات الإدخال

حلول إدخال الصوت المدمجة على مستوى النظام، بما في ذلك طرق الإدخال، وامتدادات IBus/Fcitx، وIME Android، ولوحات مفاتيح iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android وخدمة إدخال صوتي باستخدام Whisper للتعرف على الكلام غير المتصل والترجمة إلى الإنجليزية.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — تطبيق Linux غير متصل للإملاء الصوتي مع whisper.cpp و Whisper و محركات VOSK، وGPU Vulkan، وواجهة GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — امتداد GNOME Shell لإدخال الصوت غير المتصل عبر whisper.cpp مع تشغيل عبر مفتاح اختصار، يدعم X11 و Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — خدمة Android غير متصلة للتعرف على الكلام باستخدام Vosk مع دعم RecognitionService API القياسي.
- [Dictus](https://github.com/getdictus/dictus-ios) — لوحة مفاتيح iOS مفتوحة المصدر للإملاء الصوتي على الجهاز باستخدام WhisperKit و CoreML، تعمل في أي تطبيق.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — طريقة إدخال Linux عبر IBus لتحويل الكلام إلى نص مع بث STT، وتحسين Whisper اختياري، وتسريع GPU.

### إدخال الكلام الصيني / محركات الإدخال

مشاريع محسّنة للتعرف على الكلام الصيني والإدخال، بما في ذلك FunASR، Paraformer، ولوحات المفاتيح الصينية المبنية على SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — إدخال صوتي صيني غير متصل على Linux باستخدام FunASR Paraformer، IBus/Fcitx5، مفتاح اختصار PTT، وتلميع الجمل.
- [voice-input-method](https://github.com/pofice/voice-input-method) — طريقة إدخال صوتي غير متصلة عبر المنصات باستخدام FunASR، مع تصحيح الكلمات المفتاحية، واللصق التلقائي، وأوضاع GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — لوحة مفاتيح إدخال صوتي Android مع 11 محرك ASR، ومعالجة LLM اللاحقة، والكرة العائمة، وواجهة Material3.

### إدخال الصوت عبر المتصفح والويب

إدخال الصوت عبر المتصفح من خلال الإضافات، أو أغلفة WebAssembly، أو واجهات الويب، وعادة ما يتطلب backend STT محلي أو سحابي.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — واجهة Gradio WebUI لـ Whisper لاستخراج الترجمة من الملفات أو YouTube أو الميكروفون، مع VAD، وفصل BGM، وتقسيم المتحدثين.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — إضافة متصفح لتحويل الكلام إلى نص غير المتصل في الوقت الفعلي عبر Vosk، مع أوامر صوتية بالعربية والإنجليزية.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — مكتبة متصفح غير متصلة للتعرف على الكلام تُغلِّف Vosk كـ WebAssembly تعمل في WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — إضافة متصفح وخادم Whisper محلي لتحويل الكلام إلى نص غير المتصل في Firefox و Chrome عبر Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — إضافة Chrome تسجل الصوت عبر مفتاح اختصار، تنسخ عبر OpenAI Whisper API، وتلصق النص تلقائيًا.
- [voico](https://github.com/Kirera-Wainaina/voico) — إضافة Chrome لإدخال صوتي إلى نص في حقول الويب، مع backend Node.js يستخدم Google و OpenAI STT.

### إدخال الصوت على الأجهزة المحمولة (غير محركات إدخال)

تطبيقات نسخ صوتي مستقلة على Android أو iOS، بدلًا من لوحات مفاتيح طرق الإدخال.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — لوحة مفاتيح تعرف صوتي خاصة على الجهاز لنظام Android تستخدم Whisper عبر whisper.cpp و Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — تطبيق iOS مفتوح المصدر لنسخ الصوت غير المتصل باستخدام Whisper.cpp، مع التسجيل وتصدير الصوت.
- [seamless](https://github.com/woheller69/seamless) — تطبيق Android غير متصل لترجمة الكلام إلى نص باستخدام Meta Seamless M4T Lite لـ 5 لغات مع إخراج TTS.

### سكربتات خفيفة، سطر أوامر، والتحكم الصوتي

سكربتات خفيفة، وأدوات CLI، ومشغلات شريط النظام، أو أدوات مساعدة مناسبة للتكامل في التطوير أو كمكملات لسلاسل الأدوات الحالية.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — أداة Linux غير متصلة لتحويل الكلام إلى نص باستخدام Vosk تحاكي إدخال لوحة المفاتيح في أي تطبيق.
- [voice_typing](https://github.com/themanyone/voice_typing) — سكربت Bash للكتابة الصوتية غير المتصلة عبر Whisper لـ TTY و X11 و Wayland و WSL مع تحرير اختياري باستخدام LLM.
- [hns](https://github.com/primaprashant/hns) — أداة CLI لتحويل صوت الميكروفون المحلي إلى نص باستخدام faster-whisper، مع نسخ الحافظة وتوصيل stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — مدير GUI بـ PyQt6 لـ nerd-dictation مع شريط النظام، ونماذج Vosk، ومحاكاة الإدخال، ومفاتيح اختصار KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — أداة تحكم صوتي وكتابة قائمة على الأوامر باستخدام Kaldi و Dragonfly للتعرف على الكلام الكامل محليًا.

### أخرى

مشاريع لم تُضمَّن بعد في فئة.

- [VoxType](https://github.com/peteonrails/voxtype) — إدخال صوتي إلى نص بنمط اضغط-وتكلم على Linux و Wayland مع سبع محركات ASR محلية، دعم GPU، ووضع الاجتماعات.

## البرمجيات مفتوحة المصدر مقابل المعايير

| المشروع | السعر | مفتوح المصدر | قابل للتوسيع | غير متصل | صيني |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Free (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Free (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Free (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(مغلق)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(مغلق)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(مغلق)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## كيفية الاختيار

- **تطبيق سطح مكتب عبر المنصات ومتقن** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri، 25,281 نجمة، Whisper/Parakeet غير متصل.
- **Linux غير متصل بحد أدنى، قابل للبرمجة** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK، يحاكي إدخال لوحة المفاتيح في أي تطبيق.
- **تضمين STT في تطبيقك الخاص** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper، CPU/GPU، قابل للتضمين.
- **إدخال صيني أولًا** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python، C++، Shell؛ إدخال صوتي صيني غير متصل على Linux باستخدام FunASR Paraformer، IBus/Fcitx5، مفتاح اختصار PTT، وتلميع الجمل.
- **استضافة API/خادم نسخ ذاتيًا** → [FunASR](https://github.com/modelscope/FunASR) — مجموعة أدوات ASR صناعية مع Paraformer، SenseVoice، VAD، تقسيم المتحدثين، البث، وAPI متوافق مع OpenAI.

## المساهمة

المساهمات مرحب بها — راجع [CONTRIBUTING.md](CONTRIBUTING.md). يجب أن تكون المشاريع مفتوحة المصدر بالكامل وقابلة للتوسع وخفيفة؛ يرجى اتباع دليل أسلوب الوصف (باللغة الإنجليزية، سطر واحد، واقعي، بدون مبالغات تسويقية).

## تاريخ النجوم

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice-input,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

نمو النجوم مع مرور الوقت للمشاريع الأكثر نجوماً في هذه القائمة، بما في ذلك هذا المستودع.

## الترخيص

[MIT](LICENSE).

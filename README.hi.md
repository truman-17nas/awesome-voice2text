# Awesome Voice2Text

> आवाज़ इनपुट / डिक्टेशन सॉफ्टवेयर का एक चुनिंदा संग्रह — पूरी तरह खुला, विस्तार योग्य और हल्का। Typeless, Lazytype और Shandianshuo (闪电说) से तुलना की गई है, जो सभी बंद-स्रोत हैं।

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice2text) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice2text) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice2text?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*यदि यह सूची उपयोगी है, तो कृपया रेपो को ⭐ दें — इससे दूसरे इसे ढूंढ पाएंगे।*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · **हिन्दी** · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## विषय सूची

- [मानदंड (बंद-स्रोत)](#मनदड-बद-सरत)
- [इस सूची का कारण](#इस-सच-क-करण)
- [शामिल होने के मानदंड](#शमल-हन-क-मनदड)
- [शीर्ष चयन](#शरष-चयन)
- [सभी परियोजनाएँ](#सभ-परयजनए)
- [वर्गीकृत सूची](#वरगकत-सच)
  - [क्रॉस-प्लेटफॉर्म डेस्कटॉप वास्तविक-समय डिक्टेशन](#करस-पलटफरम-डसकटप-वसतवक-समय-डकटशन)
  - [मूल macOS डिक्टेशन](#मल-macos-डकटशन)
  - [कृत्रिम बुद्धिमत्ता भाषण सफाई / LLM पश्च-प्रसंस्करण](#कतरम-बदधमतत-भषण-सफई-llm-पशच-परससकरण)
  - [स्थानीय/ऑफ़लाइन STT इंजन और टूलकिट](#सथनयऑफलइन-stt-इजन-और-टलकट)
  - [सिस्टम-स्तर की आवाज़ इनपुट / IME](#ससटम-सतर-क-आवज-इनपट-ime)
  - [चीनी भाषण इनपुट / IME](#चन-भषण-इनपट-ime)
  - [ब्राउज़र और वेब आवाज़ इनपुट](#बरउजर-और-वब-आवज-इनपट)
  - [मोबाइल आवाज़ इनपुट (गैर-IME)](#मबइल-आवज-इनपट-गर-ime)
  - [हल्के स्क्रिप्ट, CLI और आवाज़ नियंत्रण](#हलक-सकरपट-cli-और-आवज-नयतरण)
  - [अन्य](#अनय)
- [ओपन-स्रोत बनाम मानदंड](#ओपन-सरत-बनम-मनदड)
- [चयन कैसे करें](#चयन-कस-कर)
- [योगदान](#यगदन)
- [Star इतिहास](#star-इतहस)
- [लाइसेंस](#लइसस)

## मानदंड (बंद-स्रोत)

| उत्पाद | मूल्य निर्धारण | प्लेटफॉर्म | मॉडल/इंजन | ओपन-स्रोत |
| --- | --- | --- | --- | --- |
| Typeless | फ्रीमियम: मुफ़्त 8K सप्ताह/सप्ताह; प्रो $12/mo वार्षिक ($30/mo मासिक) | macOS, Windows, iOS, Android | क्लाउड कृत्रिम बुद्धिमत्ता API (मालिकाना) | ❌ |
| Lazytype | व्यक्तिगत €25 एक-बार (BYOK Groq); प्रो €5/mo होस्ट | Windows, macOS | Whisper large-v3-turbo Groq पर; स्थानीय whisper.cpp | ❌ |
| Shandianshuo (闪电说) | मुफ़्त (स्थानीय/BYOK); प्रो ¥29/mo या ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (स्थानीय) + क्लाउड स्वचालित भाषण पहचान | ❌ |

## इस सूची का कारण

Typeless, Lazytype और Shandianshuo (闪电说) शक्तिशाली हैं, लेकिन बंद-स्रोत हैं। यह सूची ओपन-स्रोत विकल्पों को संग्रहीत करती है जो तीन मानदंडों को पूरा करते हैं: कोड पूरी तरह सार्वजनिक है, उपकरण विस्तार योग्य है, और यह एक व्यक्तिगत मशीन पर चलने के लिए काफी हल्का है। इसमें वर्तमान में **9 श्रेणियों में 75 परियोजनाएँ** शामिल हैं, जिन्हें पूरी तरह ओपन-स्रोत होने की पुष्टि के लिए सत्यापित किया गया है।

## शामिल होने के मानदंड

- ✅ **पूरी तरह ओपन-स्रोत** — सभी कोड एक सार्वजनिक प्लेटफॉर्म (GitHub, GitLab, Codeberg) पर।
- 🔌 **विस्तार योग्य** — आप वे सुविधाएँ, मॉडल, या एकीकरण जोड़ सकते हैं जो आप चाहते हैं।
- ⚡ **हल्का** — न्यूनतम अतिरिक्त भार, तेज़ शुरुआत, छोटा आकार।

## शीर्ष चयन

 🏆 **[Handy](https://github.com/cjpais/Handy)** — Whisper या Parakeet का उपयोग करते हुए क्रॉस-प्लेटफॉर्म ऑफ़लाइन ध्वनि-से-पाठ उपकरण, वैश्विक हॉटकी और क्लिपबोर्ड चिपकाने के साथ। *समुदाय का ध्वजवाहक — 25,281 तारे, सबसे परिष्कृत प्रस्ताव।*

**फिट-5 चयन** (तीनों मानदंड पूरे करते हैं):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — OpenAI Whisper का हाई-परफॉरमेंस C/C++ पोर्ट, CPU/GPU अनुमान, क्वांटाइज़ेशन और क्रॉस-प्लेटफॉर्म समर्थन के साथ।
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Linux ऑफ़लाइन भाषण-से-पाठ उपकरण Vosk का उपयोग करते हुए, जो किसी भी अनुप्रयोग में कीबोर्ड इनपुट का अनुकरण करता है।
- **[VoxType](https://github.com/peteonrails/voxtype)** — Linux और Wayland दबाकर-बोलें ध्वनि-से-पाठ, सात स्थानीय स्वचालित भाषण पहचान इंजन, GPU समर्थन, और बैठक मोड के साथ।
- **[voice_typing](https://github.com/themanyone/voice_typing)** — TTY, X11, Wayland, और WSL के लिए Whisper के माध्यम से ऑफ़लाइन आवाज़ टाइपिंग के लिए Bash स्क्रिप्ट, वैकल्पिक LLM संपादन के साथ।

## सभी परियोजनाएँ

| नाम | ⭐ स्टार | लाइसेंस | भाषा | फिट | ओपन | विस्तार | हल्का | चीनी |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | 51,163 | MIT | C/C++, CMake, Python/Java/C# bindings | 5 | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | 1,882 | GPL-3.0 | Python | 5 | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | 909 | MIT | Rust | 5 | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | 155 | GPL-2.0 | Bash | 5 | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | 25,281 | MIT | Rust, Tauri, React, TypeScript, Tailwind | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | 19,906 | MIT | Python, PyQt6, Whisper, PyTorch, ONNX Runtime | 4 | ✅ | ✅ | ⚠️ | ◐ |
| [FunASR](https://github.com/modelscope/FunASR) | 18,745 | MIT | Python (PyTorch) | 4 | ⚠️ | ✅ | ⚠️ | ✅ |
| [vosk-api](https://github.com/alphacep/vosk-api) | 14,889 | Apache-2.0 | C++ सहित Python, Java, C#, Node.js, Rust, Go | 4 | ⚠️ | ✅ | ✅ | ✅ |
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
| [vosk-browser](https://github.com/ccoreilly/vosk-browser) | 520 | Apache-2.0 | TypeScript, JavaScript, वेबअसेंबली | 3 | ✅ | ✅ | ✅ | ◐ |
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

## वर्गीकृत सूची

### क्रॉस-प्लेटफॉर्म डेस्कटॉप वास्तविक-समय डिक्टेशन

Whisper आधारित डेस्कटॉप डिक्टेशन ऐप Linux, Windows, या क्रॉस-प्लेटफॉर्म के लिए, दबाकर-बोलें, स्थानीय प्रतिलेखन, और स्वतः-इनपुट के साथ।

- [Handy](https://github.com/cjpais/Handy) — Whisper या Parakeet का उपयोग करते हुए क्रॉस-प्लेटफॉर्म ऑफ़लाइन ध्वनि-से-पाठ उपकरण, वैश्विक हॉटकी और क्लिपबोर्ड चिपकाने के साथ।
- [Buzz](https://github.com/chidiwilliams/buzz) — GPU त्वरण और प्रत्यक्ष माइक के साथ ऑफ़लाइन Whisper प्रतिलेखन और अनुवाद के लिए क्रॉस-प्लेटफॉर्म डेस्कटॉप ग्राफ़िकल उपयोगकर्ता इंटरफ़ेस।
- [Vibe](https://github.com/thewh1teagle/vibe) — GPU त्वरण के साथ Whisper का उपयोग करते हुए ऑफ़लाइन ऑडियो और वीडियो प्रतिलेखन के लिए क्रॉस-प्लेटफॉर्म डेस्कटॉप ऐप।
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Markdown/SQLite संग्रहण, Yjs CRDT सिंक, और डेस्कटॉप भाषण-से-पाठ उपयोगिता के साथ स्थानीय-प्रथम ऐप टूलकिट।
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — स्थानीय Whisper और ONNX मॉडल, क्लाउड API, Waybar एकीकरण, दृश्यकारी के साथ Linux-मूल भाषण-से-पाठ।
- [whisper-writer](https://github.com/savbell/whisper-writer) — स्थानीय रूप से या API के माध्यम से Whisper का उपयोग करते हुए डेस्कटॉप डिक्टेशन ऐप, सक्रिय विंडो में टाइप करने के लिए वैश्विक हॉटकी द्वारा ट्रिगर किया जाता है।
- [Chirp](https://github.com/Whamp/chirp-stt) — ParakeetV3 का उपयोग करते हुए Windows केवल-CPU डिक्टेशन ऐप, हॉटकी टॉगल, क्लिपबोर्ड चिपकाने, और शब्द ओवरराइड के साथ।
- [Dabri](https://github.com/AshBuk/dabri) — whisper.cpp का उपयोग करते हुए Linux ऑफ़लाइन STT ऐप, X11/Wayland डेस्कटॉप के लिए डेमन, CLI, और वेबसॉकेट मोड के साथ।
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Linux और Sailfish OS ऑफ़लाइन नोट-बनाने वाला ऐप, कई इंजनों का उपयोग करते हुए स्थानीय STT, पाठ-से-ध्वनि, और अनुवाद के साथ।
- [voxd](https://github.com/jakovius/voxd) — whisper.cpp का उपयोग करते हुए Linux डेस्कटॉप आवाज़ डिक्टेशन, ydotool टाइपिंग और कृत्रिम बुद्धिमत्ता पश्च-प्रसंस्करण के साथ ऑफ़लाइन स्वचालित भाषण पहचान के लिए।
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Whisper, Parakeet, या Canary ONNX के माध्यम से Linux ऑफ़लाइन आवाज़ टाइपिंग, X11/Wayland समर्थन और LLM समाशोधन के साथ।
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Caps Lock हॉटकी का उपयोग करते हुए Windows आवाज़-टाइपिंग सहायक, बहु-प्रदाता STT और वैकल्पिक LLM समाशोधन के साथ।
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — distil-whisper, हॉटकी नियंत्रण, और वैकल्पिक स्थानीय LLM सहायक के साथ क्रॉस-प्लेटफॉर्म ऑफ़लाइन डिक्टेशन ऐप।
- [TalkType](https://github.com/lmacan1/talktype) — faster-whisper का उपयोग करते हुए क्रॉस-प्लेटफॉर्म दबाकर-बोलें आवाज़ टाइपिंग, वैश्विक हॉटकी और स्मार्ट चिपकाने के साथ।
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Faster-Whisper का उपयोग करते हुए ऑफ़लाइन बहुभाषी डिक्टेशन ऐप, सक्रिय क्षेत्र में प्रतिलेखन के लिए हॉटकी द्वारा ट्रिगर किया जाता है।
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — GTK4 प्रतिक्रिया और 99-भाषा समर्थन के साथ whisper.cpp का उपयोग करते हुए NixOS/Wayland स्थानीय आवाज़ डिक्टेशन।
- [freespeak](https://github.com/Zetaphor/freespeak) — STT, LanguageTool के माध्यम से व्याकरण संशोधन, और ydotool पाठ इनपुट के साथ Linux Wayland आवाज़ डिक्टेशन ऐप।
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — आवाज़ डिक्टेशन, LLM बातचीत, छवि निर्माण, और आवाज़-चालित स्वचालन को संयोजित करते हुए स्थानीय कृत्रिम बुद्धिमत्ता डेस्कटॉप एजेंट।
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Windows डेस्कटॉप भाषण-से-पाठ faster-whisper का उपयोग करते हुए, कीबोर्ड अनुकरण, आवाज़-सक्रियता पहचान, दबाकर-बोलें, और विराम चिह्न के साथ।
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — KDE Wayland के लिए Whisper आवाज़ डिक्टेशन, पृष्ठभूमि डेमन, systemd सेवा, और क्लिपबोर्ड चिपकाने के साथ।

### मूल macOS डिक्टेशन

Swift और WhisperKit के साथ बने मूल macOS डिक्टेशन ऐप्स, वैश्विक हॉटकी, मेनू पट्टी, और न्यूरल इंजन त्वरण का समर्थन करते हैं।

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — macOS भाषण प्रतिलेखन ऐप Whisper और Parakeet इंजन, वैश्विक हॉटकी, और बैच प्रसंस्करण के साथ।
- [Pindrop](https://github.com/watzon/pindrop) — मूल macOS मेनू-पट्टी डिक्टेशन ऐप WhisperKit का उपयोग करते हुए, हॉटकी और वैकल्पिक कृत्रिम बुद्धिमत्ता सफाई के साथ।
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Whisper का उपयोग करते हुए ऑफ़लाइन बहुभाषी डिक्टेशन उपकरण, हॉटकी से किसी भी इनपुट क्षेत्र में प्रतिलेखन करता है।
- [FnKey](https://github.com/evoleinik/fnkey) — macOS मेनू-पट्टी ऐप Deepgram Nova-3 के माध्यम से Fn दबाए रखने पर भाषण प्रतिलेखन करता है और परिणाम चिपकाता है।
- [hush](https://github.com/djmunro/hush) — स्थानीय Whisper/Parakeet ONNX का उपयोग करते हुए macOS दबाकर-बोलें डिक्टेशन ऐप, हॉटकी के माध्यम से स्वतः-चिपकाने के साथ।
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — ऑफ़लाइन Whisper का उपयोग करते हुए macOS मेनू-पट्टी डिक्टेशन ऐप, Metal GPU त्वरण और कर्सर पाठ इंजेक्शन के साथ।
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Apple macOS मेनू-पट्टी ऐप Globe/Fn रिलीज़ पर रिकॉर्ड करता है, faster-whisper से प्रतिलेखन करता है, और कर्सर पर चिपकाता है।

### कृत्रिम बुद्धिमत्ता भाषण सफाई / LLM पश्च-प्रसंस्करण

डिक्टेशन उपकरण जो स्थानीय या क्लाउड LLMs का उपयोग करते हैं, भाषण पहचान आउटपुट को समाशोधन, स्वरूपण, सारांश, और स्वच्छ, औपचारिक पाठ में पुनर्शैली करने के लिए।

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — macOS डिक्टेशन ऐप डिवाइस-पर और क्लाउड STT, वैश्विक हॉटकी, कृत्रिम बुद्धिमत्ता कार्यप्रवाह, प्लगइन, REST API, और CLI के साथ।
- [Amical](https://github.com/amicalhq/amical) — स्थानीय-प्रथम कृत्रिम बुद्धिमत्ता डिक्टेशन ऐप Whisper ऑफ़लाइन प्रतिलेखन और Ollama स्मार्ट नोट प्रसंस्करण के लिए।
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — macOS/Windows के लिए ऑफ़लाइन आवाज़ डिक्टेशन उपकरण Whisper का उपयोग करते हुए, वैश्विक हॉटकी और वैकल्पिक कृत्रिम बुद्धिमत्ता संवर्धन के साथ।
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — स्थानीय-प्रथम आवाज़ सहायक macOS और Linux के लिए, दबाकर-बोलें, प्रतिलेखन, और प्लगइन निष्कर्षण के साथ।
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Whisper और LLM सफाई का उपयोग करते हुए macOS दबाकर-बोलें डिक्टेशन ऐप, Cmd-V के माध्यम से संवारित पाठ चिपकाता है।
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Whisper और LLM समाशोधन के साथ स्थानीय आवाज़ डिक्टेशन, दबाकर-बोलें, शब्दकोश, और क्लाइंट-सर्वर विभाजन।
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — स्थानीय आवाज़ डिक्टेशन और बैठक रिकॉर्डर faster-whisper, LLM सारांश, और दोहरी-ट्रैक ऑडियो कैप्चर के साथ।
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — मूल macOS ध्वनि-से-पाठ ऐप स्थानीय whisper.cpp मॉडल का उपयोग करते हुए, वैश्विक शॉर्टकट और संदर्भ-जागरूक मोड के साथ।
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — macOS डिक्टेशन ऐप डिवाइस-पर भाषण पहचान और स्वरूपण के लिए वैकल्पिक कृत्रिम बुद्धिमत्ता पश्च-प्रसंस्करण के साथ।
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — डेस्कटॉप आवाज़ प्रतिलेखन ऐप हॉटकी, कृत्रिम बुद्धिमत्ता सहायक, बैठक वक्ता पहचान, और अर्थपूर्ण खोज के साथ।
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — macOS मेनू-पट्टी ऐप ऑफ़लाइन भाषण-से-पाठ और बैठक सारांश के लिए Whisper और Qwen का उपयोग Apple Silicon पर।
- [Voquill](https://github.com/voquill/voquill) — क्रॉस-प्लेटफॉर्म Tauri आवाज़ टाइपिंग ऐप स्थानीय Whisper या Groq, कृत्रिम बुद्धिमत्ता सफाई, शब्दावली, और आवाज़ सहायक के साथ।
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — क्रॉस-प्लेटफॉर्म आवाज़ डिक्टेशन सहायक LLM स्वरूपण के साथ, स्थानीय Whisper, Ollama या क्लाउड API का समर्थन करता है।
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — क्रॉस-प्लेटफॉर्म Tauri ऐप कृत्रिम बुद्धिमत्ता आवाज़ टाइपिंग, पाठ पुनर्लेखन, और आवाज़ प्रश्नोत्तर के लिए, वैश्विक हॉटकी के साथ।
- [Aria](https://github.com/Xingxun7777/Aria) — Windows कृत्रिम बुद्धिमत्ता आवाज़ इनपुट ऑफ़लाइन Qwen3-ASR का उपयोग करते हुए वर्ण पहचान संदर्भ, हॉट-शब्द संशोधन, और आवाज़ कमांड के साथ।
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Windows आवाज़ डिक्टेशन whisper.cpp, Groq या llama.cpp का उपयोग करते हुए, कई शैलियाँ, सक्रिय विंडो में स्वतः-चिपकाना।
- [localflow](https://github.com/sidharth-n/localflow) — स्थानीय क्रॉस-प्लेटफॉर्म आवाज़ डिक्टेशन Moonshine STT, Qwen3-4B पॉलिशर, दबाकर-बोलें, और छोड़ने-का-गेट के साथ।
- [yammer](https://github.com/andynu/yammer) — Linux स्थानीय भाषण-से-पाठ Whisper और LLM सफाई के साथ, साथ ही Tauri ओवरले उपयोगकर्ता इंटरफ़ेस और xdotool इनपुट इंजेक्शन।

### स्थानीय/ऑफ़लाइन STT इंजन और टूलकिट

ऐप एकीकरण के लिए ऑफ़लाइन स्वचालित भाषण पहचान इंजन और भाषण टूलकिट: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech, और SenseVoice।

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — OpenAI Whisper का हाई-परफॉरमेंस C/C++ पोर्ट, CPU/GPU अनुमान, क्वांटाइज़ेशन और क्रॉस-प्लेटफॉर्म समर्थन के साथ।
- [FunASR](https://github.com/modelscope/FunASR) — औद्योगिक स्वचालित भाषण पहचान टूलकिट Paraformer, SenseVoice, आवाज़-सक्रियता पहचान, वक्ता पहचान, स्ट्रीमिंग, और OpenAI-संगत API के साथ।
- [vosk-api](https://github.com/alphacep/vosk-api) — ऑफ़लाइन भाषण पहचान टूलकिट छोटे केवल-CPU मॉडल के साथ 20+ भाषाओं के लिए और बहु-भाषा बाइंडिंग।
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — ऑफ़लाइन भाषण टूलकिट अगली पीढ़ी Kaldi और ONNX Runtime का उपयोग करते हुए STT, पाठ-से-ध्वनि, वक्ता पहचान, आवाज़-सक्रियता पहचान, और अधिक के लिए।
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — व्यापक भाषण टूलकिट स्वचालित भाषण पहचान, पाठ-से-ध्वनि, आवाज़-चित्र, वक्ता पहचान, अनुवाद, और स्ट्रीमिंग सेवाओं के साथ।
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — भाषण मॉडल स्वचालित भाषण पहचान 50+ भाषाओं, भाव, ऑडियो घटनाओं, और तेज़ गैर-स्वतंत्र अनुमान के साथ।

### सिस्टम-स्तर की आवाज़ इनपुट / IME

सिस्टम स्तर पर एकीकृत आवाज़ इनपुट समाधान, इनपुट विधियाँ, IBus/Fcitx एक्सटेंशन, Android IME, और iOS कीबोर्ड सहित।

- [Whisper IME](https://github.com/woheller69/whisperIME) — Android IME और आवाज़ इनपुट सेवा Whisper का उपयोग करते हुए ऑफ़लाइन भाषण पहचान और अंग्रेजी अनुवाद के लिए।
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — ऑफ़लाइन Linux आवाज़ डिक्टेशन ऐप whisper.cpp, Whisper, और VOSK इंजन, Vulkan GPU, और GTK ग्राफ़िकल उपयोगकर्ता इंटरफ़ेस के साथ।
- [blurt](https://github.com/QuantiusBenignus/blurt) — GNOME Shell एक्सटेंशन ऑफ़लाइन आवाज़ इनपुट के लिए whisper.cpp का उपयोग करते हुए, हॉटकी ट्रिगर के साथ, X11 और Wayland का समर्थन।
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Android ऑफ़लाइन भाषण पहचान सेवा Vosk का उपयोग करते हुए, मानक RecognitionService API समर्थन के साथ।
- [Dictus](https://github.com/getdictus/dictus-ios) — ओपन-स्रोत iOS कीबोर्ड डिवाइस-पर आवाज़ डिक्टेशन के लिए WhisperKit और CoreML का उपयोग करते हुए, किसी भी ऐप में काम करता है।
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Linux IBus भाषण-से-पाठ इनपुट विधि स्ट्रीमिंग STT, वैकल्पिक Whisper समाशोधन, और GPU त्वरण के साथ।

### चीनी भाषण इनपुट / IME

चीनी भाषण पहचान और इनपुट के लिए अनुकूलित परियोजनाएँ, FunASR, Paraformer, और SenseVoice आधारित चीनी IME और कीबोर्ड सहित।

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — ऑफ़लाइन Linux चीनी आवाज़ इनपुट FunASR Paraformer, IBus/Fcitx5, PTT हॉटकी, और वाक्य समाशोधन का उपयोग करते हुए।
- [voice-input-method](https://github.com/pofice/voice-input-method) — FunASR का उपयोग करते हुए क्रॉस-प्लेटफॉर्म ऑफ़लाइन आवाज़ इनपुट विधि, हॉटवर्ड संशोधन, स्वतः-चिपकाने और ग्राफ़िकल/कमांड-लाइन मोड के साथ।
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Android आवाज़ इनपुट कीबोर्ड 11 स्वचालित भाषण पहचान इंजन, LLM पश्च-प्रसंस्करण, तैरता गोला, और Material3 उपयोगकर्ता इंटरफ़ेस के साथ।

### ब्राउज़र और वेब आवाज़ इनपुट

ब्राउज़र आधारित आवाज़ इनपुट एक्सटेंशन, वेबअसेंबली रैपर, या वेब उपयोगकर्ता इंटरफ़ेस के माध्यम से उपलब्ध होता है, आमतौर पर एक स्थानीय या क्लाउड STT पृष्ठभाग की आवश्यकता होती है।

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI फ़ाइलों, YouTube, या माइक से उपशीर्षक के लिए, आवाज़-सक्रियता पहचान, पृष्ठभूमि संगीत पृथक्करण, और वक्ता पहचान के साथ।
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Vosk के माध्यम से वास्तविक-समय ऑफ़लाइन भाषण-से-पाठ के लिए ब्राउज़र एक्सटेंशन, अरबी और अंग्रेजी आवाज़ कमांड के साथ।
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — ब्राउज़र-आधारित ऑफ़लाइन भाषण पहचान लाइब्रेरी Vosk को वेबअसेंबली में पैक करते हुए वेब कार्यकर्ता में चलाता है।
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Firefox और Chrome में ऑफ़लाइन भाषण-से-पाठ के लिए ब्राउज़र एक्सटेंशन और स्थानीय Whisper सर्वर, Alt+A के माध्यम से।
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Chrome एक्सटेंशन जो हॉटकी से आवाज़ रिकॉर्ड करता है, OpenAI Whisper API से प्रतिलेखन करता है, और पाठ स्वतः-चिपकाता है।
- [voico](https://github.com/Kirera-Wainaina/voico) — वेब क्षेत्रों में ध्वनि-से-पाठ इनपुट के लिए Chrome एक्सटेंशन, Node.js पृष्ठभाग Google और OpenAI STT का उपयोग करते हुए।

### मोबाइल आवाज़ इनपुट (गैर-IME)

Android या iOS पर स्वतंत्र आवाज़ प्रतिलेखन ऐप, इनपुट विधि कीबोर्ड के बजाय।

- [Transcribro](https://github.com/soupslurpr/Transcribro) — निजी डिवाइस-पर भाषण पहचान कीबोर्ड Android के लिए Whisper द्वारा whisper.cpp और Silero आवाज़-सक्रियता पहचान का उपयोग करते हुए।
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — ओपन-स्रोत iOS ऐप ऑफ़लाइन आवाज़ प्रतिलेखन whisper.cpp का उपयोग करते हुए, रिकॉर्डिंग और ऑडियो निर्यात के साथ।
- [seamless](https://github.com/woheller69/seamless) — Android ऑफ़लाइन भाषण-से-पाठ अनुवाद ऐप Meta Seamless M4T Lite का उपयोग करते हुए 5 भाषाओं के लिए पाठ-से-ध्वनि आउटपुट के साथ।

### हल्के स्क्रिप्ट, CLI और आवाज़ नियंत्रण

हल्के स्क्रिप्ट, CLI उपकरण, ट्रे ट्रिगर, या उपयोगिताएँ जो डेवलपर एकीकरण या मौजूदा टूलचेन के पूरक के रूप में उपयुक्त होते हैं।

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Linux ऑफ़लाइन भाषण-से-पाठ उपकरण Vosk का उपयोग करते हुए, जो किसी भी अनुप्रयोग में कीबोर्ड इनपुट का अनुकरण करता है।
- [voice_typing](https://github.com/themanyone/voice_typing) — TTY, X11, Wayland, और WSL के लिए Whisper के माध्यम से ऑफ़लाइन आवाज़ टाइपिंग के लिए Bash स्क्रिप्ट, वैकल्पिक LLM संपादन के साथ।
- [hns](https://github.com/primaprashant/hns) — स्थानीय माइक्रोफ़ोन भाषण-से-पाठ के लिए CLI उपकरण faster-whisper का उपयोग करते हुए, क्लिपबोर्ड कॉपी और stdout पाइपिंग के साथ।
- [Elograf](https://github.com/papoteur-mga/elograf) — nerd-dictation के लिए PyQt6 ग्राफ़िकल उपयोगकर्ता इंटरफ़ेस प्रबंधक सिस्टम ट्रे, Vosk मॉडल, इनपुट अनुकरण, और KDE हॉटकी के साथ।
- [Osprey](https://github.com/osprey-voice/osprey) — कमांड-आधारित आवाज़ नियंत्रण और टाइपिंग उपकरण Kaldi और Dragonfly का उपयोग करते हुए पूरी तरह स्थानीय भाषण पहचान के लिए।

### अन्य

अभी तक किसी श्रेणी में नहीं रखी गई परियोजनाएँ।

- [VoxType](https://github.com/peteonrails/voxtype) — Linux और Wayland दबाकर-बोलें ध्वनि-से-पाठ सात स्थानीय स्वचालित भाषण पहचान इंजन, GPU समर्थन, और बैठक मोड के साथ।

## ओपन-स्रोत बनाम मानदंड

| परियोजना | मूल्य | ओपन-स्रोत | विस्तार योग्य | ऑफ़लाइन | चीनी |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | निःशुल्क (ओपन-स्रोत) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(बंद)* | फ्रीमियम: मुफ़्त 8K सप्ताह/सप्ताह; प्रो $12/mo वार्षिक ($30/mo मासिक) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(बंद)* | व्यक्तिगत €25 एक-बार (BYOK Groq); प्रो €5/mo होस्ट | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(बंद)* | मुफ़्त (स्थानीय/BYOK); प्रो ¥29/mo या ¥238.8/वर्ष | ❌ | ❌ | ◐ | ◐ |

## चयन कैसे करें

- **संवारित क्रॉस-प्लेटफॉर्म डेस्कटॉप ऐप** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 तारे, Whisper/Parakeet ऑफ़लाइन.
- **न्यूनतम Linux ऑफ़लाइन, स्क्रिप्टयोग्य** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, किसी भी ऐप में कीबोर्ड इनपुट का अनुकरण करता है।
- **अपने ऐप में STT एम्बेड करें** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, एम्बेड करने योग्य.
- **चीनी-प्रथम इनपुट** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; ऑफ़लाइन Linux चीनी आवाज़ इनपुट FunASR Paraformer, IBus/Fcitx5, PTT हॉटकी, और वाक्य समाशोधन का उपयोग करते हुए।
- **प्रतिलेखन API/सर्वर स्व-होस्ट करें** → [FunASR](https://github.com/modelscope/FunASR) — औद्योगिक स्वचालित भाषण पहचान टूलकिट Paraformer, SenseVoice, आवाज़-सक्रियता पहचान, वक्ता पहचान, स्ट्रीमिंग, और OpenAI-संगत API के साथ।

## योगदान

योगदान स्वागत योग्य हैं — देखें [CONTRIBUTING.md](CONTRIBUTING.md). परियोजनाएं पूर्ण रूप से ओपन-सोर्स, विस्तारयोग्य और हल्की होनी चाहिए; कृपया विवरण शैली मार्गदर्शिका का पालन करें (अंग्रेजी में, एक पंक्ति, तथ्यपरक, बिना मार्केटिंग बकवास के).

## Star इतिहास

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=dark">
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date&theme=light">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=Lxcardoza993/awesome-voice2text,cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date">
</picture>

इस लिस्ट में सबसे ज़्यादा स्टार वाली प्रोजेक्ट्स के समय के साथ स्टार वृद्धि का रुझान, इस रिपॉजिटरी को शामिल करके।

## लाइसेंस

[MIT](LICENSE).

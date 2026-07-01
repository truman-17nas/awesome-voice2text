# Awesome Voice Input

> รายการคัดสรรของซอฟต์แวร์ป้อนเสียง/พิมพ์ด้วยเสียงโอเพนซอร์ส — เปิดเต็มรูปแบบ ขยายได้ และเบา เปรียบเทียบกับ Typeless, Lazytype และ Shandianshuo (闪电说) ซึ่งทั้งหมดเป็นซอร์สปิด

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*ถ้ารายการนี้มีประโยชน์ โปรด ⭐ ให้ repo — จะช่วยให้ผู้อื่นค้นพบได้*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · [Tiếng Việt](README.vi.md) · **ไทย** · [Українська](README.uk.md) · [Català](README.ca.md)

## สารบัญ

- [มาตรวัด (ปิดซอร์ส)](#มาตรวด-ปดซอรส)
- [ทำไมถึงเลือกรายการนี้](#ทำไมถงเลอกรายการน)
- [เกณฑ์การคัดเลือก](#เกณฑการคดเลอก)
- [คัดเลือกเด่น](#คดเลอกเดน)
- [โครงการทั้งหมด](#โครงการทงหมด)
- [รายการตามหมวดหมู่](#รายการตามหมวดหม)
  - [การพิมพ์ด้วยเสียงแบบเรียลไทม์บนเดสก์ท็อปข้ามแพลตฟอร์ม](#การพมพดวยเสยงแบบเรยลไทมบนเดสกทอปขามแพลตฟอรม)
  - [การพิมพ์ด้วยเสียงดั้งเดิมบน macOS](#การพมพดวยเสยงดงเดมบน-macos)
  - [การปรับแต่งเสียงด้วย AI / หลังประมวลผลด้วย LLM](#การปรบแตงเสยงดวย-ai-หลงประมวลผลดวย-llm)
  - [เครื่องมือ STT แบบออฟไลน์/ในเครื่องและชุดเครื่องมือ](#เครองมอ-stt-แบบออฟไลนในเครองและชดเครองมอ)
  - [การป้อนเสียงระดับระบบ / IME](#การปอนเสยงระดบระบบ-ime)
  - [การป้อนเสียงภาษาจีน / IME](#การปอนเสยงภาษาจน-ime)
  - [การป้อนเสียงบนเบราว์เซอร์และเว็บ](#การปอนเสยงบนเบราวเซอรและเวบ)
  - [การป้อนเสียงบนมือถือ (ไม่ใช่ IME)](#การปอนเสยงบนมอถอ-ไมใช-ime)
  - [สคริปต์เบา ๆ CLI และการควบคุมด้วยเสียง](#สครปตเบา-ๆ-cli-และการควบคมดวยเสยง)
  - [อื่น ๆ](#อน-ๆ)
- [โอเพนซอร์สเทียบกับมาตรวัด](#โอเพนซอรสเทยบกบมาตรวด)
- [วิธีเลือก](#วธเลอก)
- [การมีส่วนร่วม](#การมสวนรวม)
- [ประวัติ Star](#ประวต-star)
- [สัญญาอนุญาต](#สญญาอนญาต)

## มาตรวัด (ปิดซอร์ส)

| ผลิตภัณฑ์ | ราคา | แพลตฟอร์ม | โมเดล/เครื่องยนต์ | โอเพนซอร์ส |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: ฟรี 8K คำ/สัปดาห์; โปร $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (กรรมสิทธิ์) | ❌ |
| Lazytype | ส่วนตัว €25 one-time (BYOK Groq); โปร €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | ฟรี (ในเครื่อง/BYOK); โปร ¥29/mo หรือ ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (ในเครื่อง) + ASR คลาวด์ | ❌ |

## ทำไมถึงเลือกรายการนี้

Typeless, Lazytype และ Shandianshuo (闪电说) มีประสิทธิภาพแต่เป็นซอร์สปิด รายการนี้รวบรวมทางเลือกโอเพนซอร์สที่ตรงเกณฑ์สามข้อ: โค้ดเปิดเผยสู่สาธารณะอย่างเต็มที่ เครื่องมือขยายได้ และเบาพอที่จะรันบนเครื่องส่วนตัว ปัจจุบันครอบคลุม **75 โครงการใน 9 หมวดหมู่** ทั้งหมดตรวจสอบแล้วว่าเป็นโอเพนซอร์สอย่างแท้จริง

## เกณฑ์การคัดเลือก

- ✅ **โอเพนซอร์สอย่างแท้จริง** — โค้ดทั้งหมดอยู่บน forge สาธารณะ (GitHub, GitLab, Codeberg).
- 🔌 **ขยายได้** — คุณสามารถเพิ่มฟีเจอร์ โมเดล หรือการผนวกรวมที่ต้องการได้
- ⚡ **เบา** — ไม่อืดอาด เปิดเร็ว ใช้ทรัพยากรน้อย

## คัดเลือกเด่น

🏆 **[Handy](https://github.com/cjpais/Handy)** — เครื่องมือแปลงเสียงเป็นข้อความแบบออฟไลน์ข้ามแพลตฟอร์ม ใช้ Whisper หรือ Parakeet พร้อมคีย์ลัดสากลและแปะคลิปบอร์ด *ธงประจำชุมชน — 25,281 ดาว ตัวเลือกที่ขัดเกลาที่สุด*

**คัดเลือก Fit-5** (ตรงเกณฑ์ทั้งสามข้อ):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — พอร์ต C/C++ ประสิทธิภาพสูงของ OpenAI Whisper พร้อมการอนุมาน CPU/GPU การลดความละเอียด และรองรับข้ามแพลตฟอร์ม
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — เครื่องมือแปลงเสียงเป็นข้อความแบบออฟไลน์บน Linux ใช้ Vosk จำลองการป้อนคีย์บอร์ดเข้าแอปใด ๆ
- **[VoxType](https://github.com/peteonrails/voxtype)** — แปลงเสียงเป็นข้อความแบบกดพูดบน Linux และ Wayland ด้วยเครื่องยนต์ ASR ในเครื่องเจ็ดตัว รองรับ GPU และโหมดประชุม
- **[voice_typing](https://github.com/themanyone/voice_typing)** — สคริปต์ Bash พิมพ์ด้วยเสียงแบบออฟไลน์ผ่าน Whisper สำหรับ TTY, X11, Wayland และ WSL พร้อมการแก้ไขด้วย LLM แบบเลือกได้

## โครงการทั้งหมด

| ชื่อ | ⭐ ดาว | สัญญาอนุญาต | ภาษา | คะแนน Fit | เปิด | ขยาย | เบา | จีน |
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

## รายการตามหมวดหมู่

### การพิมพ์ด้วยเสียงแบบเรียลไทม์บนเดสก์ท็อปข้ามแพลตฟอร์ม

แอปพิมพ์ด้วยเสียงบนเดสก์ท็อปที่ใช้ Whisper สำหรับ Linux, Windows หรือข้ามแพลตฟอร์ม พร้อมกดพูด ถอดเสียงในเครื่อง และป้อนข้อความอัตโนมัติ

- [Handy](https://github.com/cjpais/Handy) — เครื่องมือแปลงเสียงเป็นข้อความแบบออฟไลน์ข้ามแพลตฟอร์ม ใช้ Whisper หรือ Parakeet พร้อมคีย์ลัดสากลและแปะคลิปบอร์ด
- [Buzz](https://github.com/chidiwilliams/buzz) — GUI เดสก์ท็อปข้ามแพลตฟอร์มสำหรับถอดเสียงและแปลภาษาด้วย Whisper แบบออฟไลน์ พร้อมการเร่ง GPU และไมค์สด
- [Vibe](https://github.com/thewh1teagle/vibe) — แอปเดสก์ท็อปข้ามแพลตฟอร์มสำหรับถอดเสียงและวิดีโอแบบออฟไลน์ด้วย Whisper พร้อมการเร่ง GPU
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — ชุดเครื่องมือแอปแบบ local-first ด้วย Markdown/SQLite storage, ซิงก์ Yjs CRDT และเครื่องมือแปลงเสียงเป็นข้อความบนเดสก์ท็อป
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — แปลงเสียงเป็นข้อความดั้งเดิมบน Linux ด้วย Whisper และโมเดล ONNX ในเครื่อง APIs คลาวด์ การผนวกรวม Waybar และตัวแสดงภาพ
- [whisper-writer](https://github.com/savbell/whisper-writer) — แอปพิมพ์ด้วยเสียงบนเดสก์ท็อปใช้ Whisper ในเครื่องหรือผ่าน API ทริกเกอร์ด้วยคีย์ลัดสากลเพื่อพิมพ์ลงหน้าต่างที่ใช้งานอยู่
- [Chirp](https://github.com/Whamp/chirp-stt) — แอปพิมพ์ด้วยเสียงบน Windows ใช้ CPU เท่านั้นด้วย ParakeetV3 พร้อมสวิตช์คีย์ลัด แปะคลิปบอร์ด และการแทนที่คำ
- [Dabri](https://github.com/AshBuk/dabri) — แอป STT แบบออฟไลน์บน Linux ใช้ whisper.cpp ด้วยโหมด daemon, CLI และ WebSocket สำหรับเดสก์ท็อป X11/Wayland
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — แอปจดบันทึกแบบออฟไลน์บน Linux และ Sailfish OS ด้วย STT, TTS และการแปลในเครื่องโดยใช้หลายเครื่องยนต์
- [voxd](https://github.com/jakovius/voxd) — การพิมพ์ด้วยเสียงบนเดสก์ท็อป Linux ใช้ whisper.cpp สำหรับ ASR แบบออฟไลน์ พร้อมการพิมพ์ด้วย ydotool และหลังประมวลผลด้วย AI
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — พิมพ์ด้วยเสียงแบบออฟไลน์บน Linux ผ่าน Whisper, Parakeet หรือ Canary ONNX รองรับ X11/Wayland และปัดฝุ่นด้วย LLM
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — ผู้ช่วยพิมพ์ด้วยเสียงบน Windows ใช้คีย์ลัด Caps Lock พร้อม STT หลายผู้ให้บริการและการปรับแต่ง LLM แบบเลือกได้
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — แอปพิมพ์ด้วยเสียงแบบออฟไลน์ข้ามแพลตฟอร์ม ด้วย distil-whisper ควบคุมด้วยคีย์ลัด และผู้ช่วย LLM ในเครื่องแบบเลือกได้
- [TalkType](https://github.com/lmacan1/talktype) — พิมพ์ด้วยเสียงแบบกดพูดข้ามแพลตฟอร์ม ใช้ faster-whisper พร้อมคีย์ลัดสากลและแปะอัจฉริยะ
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — แอปพิมพ์ด้วยเสียงหลายภาษาแบบออฟไลน์ ใช้ Faster-Whisper ทริกเกอร์ด้วยคีย์ลัดเพื่อถอดเสียงลงช่องที่ใช้งานอยู่
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — การพิมพ์ด้วยเสียงในเครื่องบน NixOS/Wayland ใช้ whisper.cpp พร้อมฟีดแบ็ก GTK4 และรองรับ 99 ภาษา
- [freespeak](https://github.com/Zetaphor/freespeak) — แอปพิมพ์ด้วยเสียงบน Linux Wayland ด้วย STT การแก้ไขไวยากรณ์ผ่าน LanguageTool และการป้อนข้อความด้วย ydotool
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — ตัวแทน AI เดสก์ท็อปในเครื่องที่ผสมการพิมพ์ด้วยเสียง แชท LLM การสร้างภาพ และระบบอัตโนมัติขับเคลื่อนด้วยเสียง
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — แปลงเสียงเป็นข้อความบนเดสก์ท็อป Windows ใช้ faster-whisper พร้อมการจำลองคีย์บอร์ด, VAD, PTT และวรรคตอน
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — การพิมพ์ด้วยเสียง Whisper สำหรับ KDE Wayland พร้อม daemon ในพื้นหลัง บริการ systemd และแปะคลิปบอร์ด

### การพิมพ์ด้วยเสียงดั้งเดิมบน macOS

แอปพิมพ์ด้วยเสียงดั้งเดิมบน macOS สร้างด้วย Swift และ WhisperKit รองรับคีย์ลัดสากล แถบเมนู และการเร่ง Neural Engine

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — แอปถอดเสียงเป็นข้อความบน macOS ด้วยเครื่องยนต์ Whisper และ Parakeet คีย์ลัดสากล และการประมวลผลแบบ batch
- [Pindrop](https://github.com/watzon/pindrop) — แอปพิมพ์ด้วยเสียงแถบเมนูดั้งเดิมบน macOS ใช้ WhisperKit สำหรับ STT แบบออฟไลน์ พร้อมคีย์ลัดและการปัดฝุ่นด้วย AI แบบเลือกได้
- [whisper-dictation](https://github.com/foges/whisper-dictation) — เครื่องมือพิมพ์ด้วยเสียงหลายภาษาแบบออฟไลน์ ใช้ Whisper ทริกเกอร์ด้วยคีย์ลัดเพื่อถอดเสียงลงช่องป้อนข้อมูลใด ๆ
- [FnKey](https://github.com/evoleinik/fnkey) — แอปแถบเมนูบน macOS ถอดเสียงเป็นข้อความผ่าน Deepgram Nova-3 ขณะกด Fn และแปะผลลัพธ์
- [hush](https://github.com/djmunro/hush) — แอปพิมพ์ด้วยเสียงแบบกดพูดบน macOS ใช้ Whisper/Parakeet ONNX ในเครื่อง พร้อมแปะอัตโนมัติผ่านคีย์ลัด
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — แอปพิมพ์ด้วยเสียงแถบเมนูบน macOS ใช้ Whisper แบบออฟไลน์ พร้อมการเร่ง GPU Metal และการฉีดข้อความที่เคอร์เซอร์
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — แอปแถบเมนูบน Apple macOS อัดเสียงเมื่อปล่อย Globe/Fn ถอดเสียงผ่าน faster-whisper และแปะที่เคอร์เซอร์

### การปรับแต่งเสียงด้วย AI / หลังประมวลผลด้วย LLM

เครื่องมือพิมพ์ด้วยเสียงที่ใช้ LLM ในเครื่องหรือคลาวด์เพื่อปัดฝุ่น จัดรูปแบบ สรุป และเปลี่ยนสไตล์ผลลัพธ์การรู้จำเสียงให้เป็นข้อความสะอาดและเป็นทางการ

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — แอปพิมพ์ด้วยเสียงบน macOS ด้วย STT บนอุปกรณ์และคลาวด์ คีย์ลัดสากล เวิร์กโฟลว์ AI ปลั๊กอิน REST API และ CLI
- [Amical](https://github.com/amicalhq/amical) — แอปพิมพ์ด้วยเสียง AI แบบ local-first ใช้ Whisper สำหรับถอดเสียงแบบออฟไลน์ และ Ollama สำหรับประมวลผลโน้ตอัจฉริยะ
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — เครื่องมือพิมพ์ด้วยเสียงแบบออฟไลน์สำหรับ macOS/Windows ใช้ Whisper พร้อมคีย์ลัดสากลและการเสริม AI แบบเลือกได้
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — ผู้ช่วยเสียงแบบ local-first สำหรับ macOS และ Linux พร้อมกดพูด ถอดเสียง และการแยกสาระด้วยปลั๊กอิน
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — แอปพิมพ์ด้วยเสียงแบบกดพูดบน macOS ใช้ Whisper และหลังประมวลผลด้วย LLM แปะข้อความที่ปัดฝุ่นแล้วผ่าน Cmd-V
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — การพิมพ์ด้วยเสียงในเครื่องด้วย Whisper และการปัดฝุ่นด้วย LLM กดพูด พจนานุกรม และแยกไคลเอนต์-เซิร์ฟเวอร์
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — การพิมพ์ด้วยเสียงในเครื่องและเครื่องบันทึกประชุม ใช้ faster-whisper สรุปด้วย LLM และบันทึกเสียงสองแทร็ก
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — แอปแปลงเสียงเป็นข้อความดั้งเดิมบน macOS ใช้โมเดล whisper.cpp ในเครื่อง พร้อมทางลัดสากลและโหมดตามบริบท
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — แอปพิมพ์ด้วยเสียงบน macOS ด้วยการรู้จำเสียงบนอุปกรณ์ และหลังประมวลผลด้วย AI แบบเลือกได้เพื่อจัดรูปแบบ
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — แอปถอดเสียงเป็นข้อความบนเดสก์ท็อป พร้อมคีย์ลัด ผู้ช่วย AI แยกลำดับผู้พูดในประชุม และการค้นหาเชิงความหมาย
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — แอปแถบเมนูบน macOS สำหรับแปลงเสียงเป็นข้อความแบบออฟไลน์และสรุปประชุม ใช้ Whisper และ Qwen บน Apple Silicon
- [Voquill](https://github.com/voquill/voquill) — แอปพิมพ์ด้วยเสียงข้ามแพลตฟอร์มด้วย Tauri ใช้ Whisper ในเครื่องหรือ Groq ปัดฝุ่นด้วย AI คำศัพท์เฉพาะ และผู้ช่วยเสียง
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — ผู้ช่วยพิมพ์ด้วยเสียงข้ามแพลตฟอร์ม พร้อมการจัดรูปแบบด้วย LLM รองรับ Whisper ในเครื่อง Ollama หรือ APIs คลาวด์
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — แอปข้ามแพลตฟอร์มด้วย Tauri สำหรับพิมพ์ด้วยเสียงด้วย AI การเขียนข้อความใหม่ และถาม-ตอบด้วยเสียง พร้อมคีย์ลัดสากล
- [Aria](https://github.com/Xingxun7777/Aria) — การป้อนเสียง AI บน Windows ใช้ Qwen3-ASR แบบออฟไลน์พร้อมบริบท OCR การแก้ไขคำกระตุ้น และคำสั่งด้วยเสียง
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — การพิมพ์ด้วยเสียงบน Windows ใช้ whisper.cpp, Groq หรือ llama.cpp หลายสไตล์ แปะอัตโนมัติลงหน้าต่างที่ใช้งานอยู่
- [localflow](https://github.com/sidharth-n/localflow) — การพิมพ์ด้วยเสียงข้ามแพลตฟอร์มในเครื่อง ใช้ Moonshine STT, Qwen3-4B polisher, กดพูด และ skip-gate
- [yammer](https://github.com/andynu/yammer) — แปลงเสียงเป็นข้อความในเครื่องบน Linux ด้วย Whisper และการปัดฝุ่นด้วย LLM พร้อม Tauri overlay UI และการฉีดอินพุตด้วย xdotool

### เครื่องมือ STT แบบออฟไลน์/ในเครื่องและชุดเครื่องมือ

เครื่องยนต์ ASR และชุดเครื่องมือด้านเสียงแบบออฟไลน์สำหรับผนวกรวมในแอป: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech และ SenseVoice

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — พอร์ต C/C++ ประสิทธิภาพสูงของ OpenAI Whisper พร้อมการอนุมาน CPU/GPU การลดความละเอียด และรองรับข้ามแพลตฟอร์ม
- [FunASR](https://github.com/modelscope/FunASR) — ชุดเครื่องมือ ASR อุตสาหกรรมด้วย Paraformer, SenseVoice, VAD, diarization, streaming และ API ที่เข้ากันได้กับ OpenAI
- [vosk-api](https://github.com/alphacep/vosk-api) — ชุดเครื่องมือรู้จำเสียงแบบออฟไลน์ด้วยโมเดลขนาดเล็กใช้ CPU เท่านั้นสำหรับ 20+ ภาษาและ binding หลายภาษา
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — ชุดเครื่องมือด้านเสียงแบบออฟไลน์ใช้ Kaldi รุ่นถัดไปและ ONNX Runtime สำหรับ STT, TTS, speaker ID, VAD และอื่น ๆ
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — ชุดเครื่องมือด้านเสียงครบวงจรด้วย ASR, TTS, voiceprint, diarization, การแปล และบริการ streaming
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — โมเดลเสียงด้วย ASR สำหรับ 50+ ภาษา อารมณ์ เหตุการณ์เสียง และการอนุมานแบบ non-autoregressive ที่รวดเร็ว

### การป้อนเสียงระดับระบบ / IME

โซลูชันการป้อนเสียงที่ผนวกรวมในระดับระบบ รวมถึงวิธีการป้อน ส่วนขยาย IBus/Fcitx Android IME และคีย์บอร์ด iOS

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android และบริการป้อนเสียงใช้ Whisper สำหรับการรู้จำเสียงแบบออฟไลน์และการแปลเป็นภาษาอังกฤษ
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — แอปพิมพ์ด้วยเสียงแบบออฟไลน์บน Linux ด้วยเครื่องยนต์ whisper.cpp, Whisper และ VOSK GPU Vulkan และ GTK GUI
- [blurt](https://github.com/QuantiusBenignus/blurt) — ส่วนขยาย GNOME Shell สำหรับป้อนเสียงแบบออฟไลน์ผ่าน whisper.cpp ด้วยคีย์ลัดทริกเกอร์ รองรับ X11 และ Wayland
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — บริการรู้จำเสียงแบบออฟไลน์บน Android ใช้ Vosk พร้อมรองรับ RecognitionService API มาตรฐาน
- [Dictus](https://github.com/getdictus/dictus-ios) — คีย์บอร์ด iOS โอเพนซอร์สสำหรับพิมพ์ด้วยเสียงบนอุปกรณ์ ใช้ WhisperKit และ CoreML ทำงานในแอปใด ๆ
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — วิธีการป้อนข้อความจากเสียงแบบ IBus บน Linux ด้วย streaming STT การปรับแต่ง Whisper แบบเลือกได้ และการเร่ง GPU

### การป้อนเสียงภาษาจีน / IME

โครงการที่ปรับให้เหมาะกับการรู้จำและป้อนข้อความเสียงภาษาจีน รวมถึง IME และคีย์บอร์ดจีนที่ใช้ FunASR, Paraformer และ SenseVoice

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — การป้อนเสียงภาษาจีนแบบออฟไลน์บน Linux ใช้ FunASR Paraformer, IBus/Fcitx5, คีย์ลัด PTT และการปัดฝุ่นประโยค
- [voice-input-method](https://github.com/pofice/voice-input-method) — วิธีการป้อนเสียงแบบออฟไลน์ข้ามแพลตฟอร์ม ใช้ FunASR พร้อมการแก้ไขคำกระตุ้น แปะอัตโนมัติ และโหมด GUI/CLI
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — คีย์บอร์ดป้อนเสียงบน Android ด้วยเครื่องยนต์ ASR 11 ตัว หลังประมวลผลด้วย LLM ลูกลอย และ UI Material3

### การป้อนเสียงบนเบราว์เซอร์และเว็บ

การป้อนเสียงบนเบราว์เซอร์ผ่านส่วนขยาย ตัวห่อ WebAssembly หรือ Web UI โดยทั่วไปต้องการ backend STT ในเครื่องหรือคลาวด์

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Gradio Whisper WebUI สำหรับคำบรรยายจากไฟล์ YouTube หรือไมค์ พร้อม VAD การแยก BGM และ diarization
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — ส่วนขยายเบราว์เซอร์สำหรับแปลงเสียงเป็นข้อความแบบออฟไลน์แบบเรียลไทม์ผ่าน Vosk พร้อมคำสั่งด้วยเสียงภาษาอาหรับและอังกฤษ
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — ไลบรารีรู้จำเสียงแบบออฟไลน์บนเบราว์เซอร์ แพ็ก Vosk เป็น WebAssembly ทำงานใน WebWorker
- [Speechfire](https://github.com/Jejkobb/Speechfire) — ส่วนขยายเบราว์เซอร์และเซิร์ฟเวอร์ Whisper ในเครื่อง สำหรับแปลงเสียงเป็นข้อความแบบออฟไลน์ใน Firefox และ Chrome ผ่าน Alt+A
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — ส่วนขยาย Chrome บันทึกเสียงผ่านคีย์ลัด ถอดเสียงด้วย OpenAI Whisper API และแปะข้อความอัตโนมัติ
- [voico](https://github.com/Kirera-Wainaina/voico) — ส่วนขยาย Chrome สำหรับป้อนข้อความจากเสียงลงฟิลด์เว็บ พร้อม backend Node.js ใช้ Google และ OpenAI STT

### การป้อนเสียงบนมือถือ (ไม่ใช่ IME)

แอปถอดเสียงเป็นข้อความแบบสแตนด์อโลนบน Android หรือ iOS ไม่ใช่คีย์บอร์ดวิธีการป้อน

- [Transcribro](https://github.com/soupslurpr/Transcribro) — คีย์บอร์ดรู้จำเสียงแบบส่วนตัวบนอุปกรณ์ Android ใช้ Whisper ผ่าน whisper.cpp และ Silero VAD
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — แอป iOS โอเพนซอร์สสำหรับถอดเสียงแบบออฟไลน์ด้วย Whisper.cpp พร้อมการอัดเสียงและส่งออกเสียง
- [seamless](https://github.com/woheller69/seamless) — แอปแปลงเสียงเป็นข้อความและแปลภาษาแบบออฟไลน์บน Android ใช้ Meta Seamless M4T Lite สำหรับ 5 ภาษา พร้อมเอาท์พุต TTS

### สคริปต์เบา ๆ CLI และการควบคุมด้วยเสียง

สคริปต์เบา ๆ เครื่องมือ CLI ตัวทริกเกอร์ถาดระบบ หรือยูทิลิตี้ที่เหมาะสำหรับการผนวกรวมของนักพัฒนาหรือเสริม toolchain ที่มีอยู่

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — เครื่องมือแปลงเสียงเป็นข้อความแบบออฟไลน์บน Linux ใช้ Vosk จำลองการป้อนคีย์บอร์ดเข้าแอปใด ๆ
- [voice_typing](https://github.com/themanyone/voice_typing) — สคริปต์ Bash พิมพ์ด้วยเสียงแบบออฟไลน์ผ่าน Whisper สำหรับ TTY, X11, Wayland และ WSL พร้อมการแก้ไขด้วย LLM แบบเลือกได้
- [hns](https://github.com/primaprashant/hns) — เครื่องมือ CLI สำหรับแปลงเสียงจากไมโครโฟนในเครื่องเป็นข้อความ ใช้ faster-whisper พร้อมคัดลอกคลิปบอร์ดและ piping ไป stdout
- [Elograf](https://github.com/papoteur-mga/elograf) — ตัวจัดการ GUI ด้วย PyQt6 สำหรับ nerd-dictation พร้อมถาดระบบ โมเดล Vosk การจำลองอินพุต และคีย์ลัด KDE
- [Osprey](https://github.com/osprey-voice/osprey) — เครื่องมือควบคุมด้วยเสียงและพิมพ์ตามคำสั่ง ใช้ Kaldi และ Dragonfly สำหรับการรู้จำเสียงแบบในเครื่องอย่างเต็มรูปแบบ

### อื่น ๆ

โครงการที่ยังไม่ได้จัดหมวดหมู่

- [VoxType](https://github.com/peteonrails/voxtype) — แปลงเสียงเป็นข้อความแบบกดพูดบน Linux และ Wayland ด้วยเครื่องยนต์ ASR ในเครื่องเจ็ดตัว รองรับ GPU และโหมดประชุม

## โอเพนซอร์สเทียบกับมาตรวัด

| โครงการ | ราคา | โอเพนซอร์ส | ขยายได้ | ออฟไลน์ | จีน |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | ฟรี (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | ฟรี (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | ฟรี (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | ฟรี (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | ฟรี (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | ฟรี (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: ฟรี 8K คำ/สัปดาห์; โปร $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | ส่วนตัว €25 one-time (BYOK Groq); โปร €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | ฟรี (ในเครื่อง/BYOK); โปร ¥29/mo หรือ ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## วิธีเลือก

- **แอปเดสก์ท็อปข้ามแพลตฟอร์มที่ขัดเกลา** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 ดาว, Whisper/Parakeet แบบออฟไลน์
- **Linux ออฟไลน์ขั้นต่ำ สคริปต์ได้** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, จำลองการป้อนคีย์บอร์ดเข้าแอปใด ๆ
- **ฝัง STT ในแอปของคุณเอง** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, ฝังได้
- **ป้อนข้อความภาษาจีนเป็นหลัก** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; การป้อนเสียงภาษาจีนแบบออฟไลน์บน Linux ด้วย FunASR Paraformer, IBus/Fcitx5, คีย์ลัด PTT และการปัดฝุ่นประโยค
- **โฮสต์ API/เซิร์ฟเวอร์ถอดเสียงเอง** → [FunASR](https://github.com/modelscope/FunASR) — ชุดเครื่องมือ ASR อุตสาหกรรมด้วย Paraformer, SenseVoice, VAD, diarization, streaming และ API ที่เข้ากันได้กับ OpenAI

## การมีส่วนร่วม

ยินดีรับการมีส่วนร่วม — ดูที่ [CONTRIBUTING.md](CONTRIBUTING.md). โครงการต้องเป็นโอเพนซอร์สอย่างสมบูรณ์ ขยายได้ และเบา; โปรดปฏิบัติตามคู่มือรูปแบบคำอธิบาย (เป็นภาษาอังกฤษ หนึ่งบรรทัด ตามข้อเท็จจริง ไม่มีการโฆษณาเกินจริง)

## ประวัติ Star

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

การเติบโตของ star ตลอดเวลาสำหรับโครงการที่ได้รับ star มากที่สุดในรายการนี้ ตัว repo เองอยู่ในโหมดส่วนตัวระหว่างการตรวจสอบ; ประวัติ star ของ repo เองจะถูกเพิ่มที่นี่เมื่อเปิดเป็นสาธารณะ

## สัญญาอนุญาต

[MIT](LICENSE).

# Awesome Voice Input

> Danh sách tuyển chọn các phần mềm nhập liệu bằng giọng nói / nhận dạng giọng nói mã nguồn mở — hoàn toàn mở, có thể mở rộng và nhẹ. Được so sánh với Typeless, Lazytype và Shandianshuo (闪电说), tất cả đều là mã nguồn đóng.

![License](https://img.shields.io/github/license/Lxcardoza993/awesome-voice-input) ![Last Commit](https://img.shields.io/github/last-commit/Lxcardoza993/awesome-voice-input) ![Stars](https://img.shields.io/github/stars/Lxcardoza993/awesome-voice-input?style=social) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

*Nếu danh sách này hữu ích, hãy ⭐ repo để giúp người khác tìm thấy nó.*

[English](README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [العربية](README.ar.md) · [हिन्दी](README.hi.md) · [Nederlands](README.nl.md) · [Polski](README.pl.md) · [Türkçe](README.tr.md) · [Bahasa Indonesia](README.id.md) · **Tiếng Việt** · [ไทย](README.th.md) · [Українська](README.uk.md) · [Català](README.ca.md)

## Mục lục

- [Sản phẩm tham chiếu (Mã nguồn đóng)](#sản-phẩm-tham-chiếu-mã-nguồn-đóng)
- [Tại sao có danh sách này](#tại-sao-có-danh-sách-này)
- [Tiêu chí chọn lọc](#tiêu-chí-chọn-lọc)
- [Lựa chọn hàng đầu](#lựa-chọn-hàng-đầu)
- [Tất cả dự án](#tất-cả-dự-án)
- [Danh sách phân loại](#danh-sách-phân-loại)
  - [Nhập liệu bằng giọng nói để bàn đa nền tảng theo thời gian thực](#nhập-liệu-bằng-giọng-nói-để-bàn-đa-nền-tảng-theo-thời-gian-thực)
  - [Nhập liệu bằng giọng nói cho macOS](#nhập-liệu-bằng-giọng-nói-cho-macos)
  - [Làm sạch giọng nói bằng AI / Xử lý hậu kỳ LLM](#làm-sạch-giọng-nói-bằng-ai-xử-lý-hậu-kỳ-llm)
  - [Công cụ STT cục bộ, ngoại tuyến và bộ công cụ](#công-cụ-stt-cục-bộ-ngoại-tuyến-và-bộ-công-cụ)
  - [Nhập liệu bằng giọng nói cấp hệ thống / IME](#nhập-liệu-bằng-giọng-nói-cấp-hệ-thống-ime)
  - [Nhập liệu bằng giọng nói tiếng Trung / IME](#nhập-liệu-bằng-giọng-nói-tiếng-trung-ime)
  - [Nhập liệu bằng giọng nói trên trình duyệt và web](#nhập-liệu-bằng-giọng-nói-trên-trình-duyệt-và-web)
  - [Nhập liệu bằng giọng nói trên di động (không phải IME)](#nhập-liệu-bằng-giọng-nói-trên-di-động-không-phải-ime)
  - [Tập lệnh nhẹ, CLI và điều khiển bằng giọng nói](#tập-lệnh-nhẹ-cli-và-điều-khiển-bằng-giọng-nói)
  - [Khác](#khác)
- [Mã nguồn mở so với sản phẩm tham chiếu](#mã-nguồn-mở-so-với-sản-phẩm-tham-chiếu)
- [Cách chọn](#cách-chọn)
- [Đóng góp](#đóng-góp)
- [Lịch sử Star](#lịch-sử-star)
- [Giấy phép](#giấy-phép)

## Sản phẩm tham chiếu (Mã nguồn đóng)

| Sản phẩm | Giá | Nền tảng | Mô hình/Công cụ | Mã nguồn mở |
| --- | --- | --- | --- | --- |
| Typeless | Freemium: Miễn phí 8K từ/tuần; Pro $12/mo yrly ($30/mo monthly) | macOS, Windows, iOS, Android | Cloud AI API (proprietary) | ❌ |
| Lazytype | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | Windows, macOS | Whisper large-v3-turbo on Groq; local whisper.cpp | ❌ |
| Shandianshuo (闪电说) | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | macOS, Windows, Linux; Android beta | SenseVoiceSmall (local) + cloud ASR | ❌ |

## Tại sao có danh sách này

Typeless, Lazytype và Shandianshuo (闪电说) đều mạnh mẽ nhưng là mã nguồn đóng. Danh sách này tập hợp các lựa chọn thay thế mã nguồn mở đáp ứng ba tiêu chí: mã nguồn hoàn toàn công khai, công cụ có thể mở rộng và đủ nhẹ để chạy trên máy cá nhân. Hiện tại danh sách bao gồm **75 dự án trên 9 danh mục**, tất cả đều được xác minh là hoàn toàn mã nguồn mở.

## Tiêu chí chọn lọc

- ✅ **Hoàn toàn mã nguồn mở** — toàn bộ mã nguồn trên nền tảng công khai (GitHub, GitLab, Codeberg).
- 🔌 **Có thể mở rộng** — bạn có thể thêm tính năng, mô hình hoặc tích hợp mong muốn.
- ⚡ **Nhẹ** — ít phần thừa, khởi động nhanh, chiếm ít tài nguyên.

## Lựa chọn hàng đầu

🏆 **[Handy](https://github.com/cjpais/Handy)** — Công cụ nhận dạng giọng nói ngoại tuyến đa nền tảng sử dụng Whisper hoặc Parakeet, với phím nóng toàn cục và dán từ khay nhớ tạm. *Đại diện cộng đồng — 25,281 sao, sản phẩm hoàn thiện nhất.*

**Lựa chọn Fit-5** (đáp ứng cả ba tiêu chí):
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** — Bản port C/C++ hiệu năng cao của OpenAI Whisper với suy luận CPU/GPU, lượng tử hóa và hỗ trợ đa nền tảng.
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** — Công cụ nhận dạng giọng nói ngoại tuyến trên Linux sử dụng Vosk, mô phỏng đầu vào bàn phím vào bất kỳ ứng dụng nào.
- **[VoxType](https://github.com/peteonrails/voxtype)** — Nhập liệu bằng giọng nói nhấn để nói trên Linux và Wayland với bảy công cụ ASR cục bộ, hỗ trợ GPU và chế độ họp.
- **[voice_typing](https://github.com/themanyone/voice_typing)** — Tập lệnh Bash để nhập liệu bằng giọng nói ngoại tuyến qua Whisper cho TTY, X11, Wayland và WSL với tùy chọn chỉnh sửa bằng LLM.

## Tất cả dự án

| Tên | ⭐ Sao | Giấy phép | Ngôn ngữ | Fit | Mở | Mở rộng | Nhẹ | Tiếng Trung |
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

## Danh sách phân loại

### Nhập liệu bằng giọng nói để bàn đa nền tảng theo thời gian thực

Các ứng dụng nhập liệu bằng giọng nói trên máy tính để bàn dựa trên Whisper cho Linux, Windows hoặc đa nền tảng, với nhấn để nói, phiên âm cục bộ và tự động nhập liệu.

- [Handy](https://github.com/cjpais/Handy) — Công cụ nhận dạng giọng nói ngoại tuyến đa nền tảng sử dụng Whisper hoặc Parakeet, với phím nóng toàn cục và dán từ khay nhớ tạm.
- [Buzz](https://github.com/chidiwilliams/buzz) — Giao diện để bàn đa nền tảng cho phiên âm và dịch Whisper ngoại tuyến với tăng tốc GPU, mic trực tiếp.
- [Vibe](https://github.com/thewh1teagle/vibe) — Ứng dụng để bàn đa nền tảng để phiên âm âm thanh và video ngoại tuyến sử dụng Whisper, với tăng tốc GPU.
- [Epicenter](https://github.com/EpicenterHQ/epicenter) — Bộ công cụ ứng dụng ưu tiên cục bộ với lưu trữ Markdown/SQLite, đồng bộ Yjs CRDT và tiện ích nhận dạng giọng nói để bàn.
- [hyprwhspr](https://github.com/goodroot/hyprwhspr) — Nhận dạng giọng nói bản địa trên Linux với mô hình Whisper và ONNX cục bộ, API đám mây, tích hợp Waybar và trực quan hóa.
- [whisper-writer](https://github.com/savbell/whisper-writer) — Ứng dụng nhập liệu bằng giọng nói để bàn sử dụng Whisper cục bộ hoặc qua API, được kích hoạt bằng phím nóng toàn cục để nhập vào cửa sổ đang hoạt động.
- [Chirp](https://github.com/Whamp/chirp-stt) — Ứng dụng nhập liệu bằng giọng nói trên Windows chỉ dùng CPU sử dụng ParakeetV3, với chuyển đổi phím nóng, dán khay nhớ tạm và ghi đè từ.
- [Dabri](https://github.com/AshBuk/dabri) — Ứng dụng STT ngoại tuyến trên Linux sử dụng whisper.cpp với chế độ daemon, CLI và WebSocket cho màn hình X11/Wayland.
- [dsnote (Speech Note)](https://github.com/mkiol/dsnote) — Ứng dụng ghi chú ngoại tuyến cho Linux và Sailfish OS với STT cục bộ, TTS và dịch thuật sử dụng nhiều công cụ.
- [voxd](https://github.com/jakovius/voxd) — Nhập liệu bằng giọng nói để bàn trên Linux sử dụng whisper.cpp cho ASR ngoại tuyến với nhập liệu ydotool và xử lý hậu kỳ bằng AI.
- [Speed of Sound](https://github.com/zugaldia/speedofsound) — Nhập liệu bằng giọng nói ngoại tuyến trên Linux qua Whisper, Parakeet hoặc Canary ONNX, với hỗ trợ X11/Wayland và làm mượt bằng LLM.
- [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) — Trợ lý nhập liệu bằng giọng nói trên Windows sử dụng phím nóng Caps Lock, với STT đa nhà cung cấp và tùy chọn tinh chỉnh bằng LLM.
- [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) — Ứng dụng nhập liệu bằng giọng nói ngoại tuyến đa nền tảng với distil-whisper, điều khiển phím nóng và trợ lý LLM cục bộ tùy chọn.
- [TalkType](https://github.com/lmacan1/talktype) — Nhập liệu bằng giọng nói nhấn để nói đa nền tảng sử dụng faster-whisper, với phím nóng toàn cục và dán thông minh.
- [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) — Ứng dụng nhập liệu bằng giọng nói đa ngữ ngoại tuyến sử dụng Faster-Whisper, được kích hoạt bằng phím nóng để phiên âm vào trường đang hoạt động.
- [whisper-dictation](https://github.com/jacopone/whisper-dictation) — Nhập liệu bằng giọng nói cục bộ cho NixOS/Wayland sử dụng whisper.cpp với phản hồi GTK4 và hỗ trợ 99 ngôn ngữ.
- [freespeak](https://github.com/Zetaphor/freespeak) — Ứng dụng nhập liệu bằng giọng nói trên Wayland Linux với STT, sửa ngữ pháp qua LanguageTool và nhập liệu văn bản ydotool.
- [whisper_dictation](https://github.com/themanyone/whisper_dictation) — Tác nhân để bàn AI cục bộ kết hợp nhập liệu bằng giọng nói, trò chuyện LLM, tạo ảnh và tự động hóa điều khiển bằng giọng nói.
- [OmniDictate](https://github.com/gurjar1/OmniDictate) — Nhận dạng giọng nói để bàn trên Windows sử dụng faster-whisper với mô phỏng bàn phím, VAD, PTT và dấu câu.
- [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) — Nhập liệu bằng giọng nói Whisper cho KDE Wayland với daemon nền, dịch vụ systemd và dán từ khay nhớ tạm.

### Nhập liệu bằng giọng nói cho macOS

Các ứng dụng nhập liệu bằng giọng nói bản địa cho macOS được xây dựng bằng Swift và WhisperKit, hỗ trợ phím nóng toàn cục, thanh menu và tăng tốc Neural Engine.

- [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) — Ứng dụng phiên âm giọng nói cho macOS với các công cụ Whisper và Parakeet, phím nóng toàn cục và xử lý hàng loạt.
- [Pindrop](https://github.com/watzon/pindrop) — Ứng dụng nhập liệu bằng giọng nói bản địa trên thanh menu macOS sử dụng WhisperKit cho STT ngoại tuyến, với phím nóng và làm sạch AI tùy chọn.
- [whisper-dictation](https://github.com/foges/whisper-dictation) — Công cụ nhập liệu bằng giọng nói đa ngữ ngoại tuyến sử dụng Whisper, được kích hoạt bằng phím nóng để phiên âm vào bất kỳ trường nhập liệu nào.
- [FnKey](https://github.com/evoleinik/fnkey) — Ứng dụng thanh menu macOS phiên âm giọng nói qua Deepgram Nova-3 trong khi giữ phím Fn và dán kết quả.
- [hush](https://github.com/djmunro/hush) — Ứng dụng nhập liệu bằng giọng nói nhấn để nói trên macOS sử dụng Whisper/Parakeet ONNX cục bộ với tự động dán qua phím nóng.
- [WhisperDictation](https://github.com/sam-pop/WhisperDictation) — Ứng dụng nhập liệu bằng giọng nói trên thanh menu macOS sử dụng Whisper ngoại tuyến với tăng tốc GPU Metal và chèn văn bản tại con trỏ.
- [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) — Ứng dụng thanh menu macOS ghi âm khi thả phím Globe/Fn, phiên âm qua faster-whisper và dán tại con trỏ.

### Làm sạch giọng nói bằng AI / Xử lý hậu kỳ LLM

Các công cụ nhập liệu bằng giọng nói sử dụng LLM cục bộ hoặc đám mây để chỉnh sửa, định dạng, tóm tắt và làm mới đầu ra nhận dạng giọng nói thành văn bản sạch, trang trọng.

- [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) — Ứng dụng nhập liệu bằng giọng nói cho macOS với STT trên thiết bị và đám mây, phím nóng toàn cục, luồng công việc AI, plugin, REST API và CLI.
- [Amical](https://github.com/amicalhq/amical) — Ứng dụng nhập liệu bằng giọng nói ưu tiên cục bộ sử dụng Whisper để phiên âm ngoại tuyến và Ollama để xử lý ghi chú thông minh.
- [VoiceTypr](https://github.com/moinulmoin/voicetypr) — Công cụ nhập liệu bằng giọng nói ngoại tuyến cho macOS/Windows sử dụng Whisper, với phím nóng toàn cục và tăng cường AI tùy chọn.
- [HoldSpeak](https://github.com/karolswdev/HoldSpeak) — Trợ lý giọng nói ưu tiên cục bộ cho macOS và Linux với nhấn để nói, phiên âm và trích xuất plugin.
- [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) — Ứng dụng nhập liệu bằng giọng nói nhấn để nói trên macOS sử dụng Whisper và làm sạch LLM, dán văn bản đã chỉnh sửa qua Cmd-V.
- [Voicisst](https://github.com/lucyfromnaarm/voicisst) — Nhập liệu bằng giọng nói cục bộ với Whisper và làm mượt LLM, nhấn để nói, từ điển và phân chia client-server.
- [VoiceFlow](https://github.com/infiniV/VoiceFlow) — Nhập liệu bằng giọng nói cục bộ và ghi âm cuộc họp với faster-whisper, tóm tắt LLM và ghi âm hai track.
- [VoiceInk](https://github.com/Beingpax/VoiceInk) — Ứng dụng chuyển giọng nói thành văn bản bản địa cho macOS sử dụng mô hình whisper.cpp cục bộ, với phím tắt toàn cục và chế độ theo ngữ cảnh.
- [FluidVoice](https://github.com/altic-dev/FluidVoice) — Ứng dụng nhập liệu bằng giọng nói cho macOS với nhận dạng giọng nói trên thiết bị và xử lý hậu kỳ AI tùy chọn cho định dạng.
- [OpenWhispr](https://github.com/OpenWhispr/openwhispr) — Ứng dụng phiên âm giọng nói để bàn với phím nóng, trợ lý AI, phân tích người nói cuộc họp và tìm kiếm ngữ nghĩa.
- [Ghost Pepper](https://github.com/matthartman/ghost-pepper) — Ứng dụng thanh menu macOS để nhận dạng giọng nói ngoại tuyến và tóm tắt cuộc họp sử dụng Whisper và Qwen trên Apple Silicon.
- [Voquill](https://github.com/voquill/voquill) — Ứng dụng nhập liệu bằng giọng nói đa nền tảng Tauri với Whisper cục bộ hoặc Groq, làm sạch AI, thuật ngữ và trợ lý giọng nói.
- [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) — Trợ lý nhập liệu bằng giọng nói đa nền tảng với định dạng LLM, hỗ trợ Whisper cục bộ, Ollama hoặc API đám mây.
- [OpenTypeless](https://github.com/tover0314-w/opentypeless) — Ứng dụng Tauri đa nền tảng để nhập liệu bằng giọng nói AI, viết lại văn bản và hỏi đáp bằng giọng nói với phím nóng toàn cục.
- [Aria](https://github.com/Xingxun7777/Aria) — Nhập liệu bằng giọng nói AI ngoại tuyến trên Windows sử dụng Qwen3-ASR với ngữ cảnh OCR, sửa từ khóa nóng và lệnh thoại.
- [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) — Nhập liệu bằng giọng nói trên Windows sử dụng whisper.cpp, Groq hoặc llama.cpp, nhiều phong cách, tự động dán vào cửa sổ đang hoạt động.
- [localflow](https://github.com/sidharth-n/localflow) — Nhập liệu bằng giọng nói cục bộ đa nền tảng sử dụng Moonshine STT, Qwen3-4B làm mượt, nhấn để nói và skip-gate.
- [yammer](https://github.com/andynu/yammer) — Nhận dạng giọng nói cục bộ trên Linux với Whisper và làm sạch LLM, cùng giao diện overlay Tauri và xdotool nhập liệu.

### Công cụ STT cục bộ, ngoại tuyến và bộ công cụ

Công cụ ASR ngoại tuyến và bộ công cụ xử lý giọng nói để tích hợp vào ứng dụng: Whisper, Kaldi, ONNX, Vosk, FunASR, PaddleSpeech và SenseVoice.

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — Bản port C/C++ hiệu năng cao của OpenAI Whisper với suy luận CPU/GPU, lượng tử hóa và hỗ trợ đa nền tảng.
- [FunASR](https://github.com/modelscope/FunASR) — Bộ công cụ ASR công nghiệp với Paraformer, SenseVoice, VAD, diarization, streaming và API tương thích OpenAI.
- [vosk-api](https://github.com/alphacep/vosk-api) — Bộ công cụ nhận dạng giọng nói ngoại tuyến với mô hình CPU nhỏ cho 20+ ngôn ngữ và đa ngôn ngữ binding.
- [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) — Bộ công cụ giọng nói ngoại tuyến sử dụng Kaldi thế hệ mới và ONNX Runtime cho STT, TTS, nhận diện người nói, VAD và hơn thế.
- [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) — Bộ công cụ giọng nói toàn diện với ASR, TTS, vân giọng, diarization, dịch thuật và dịch vụ streaming.
- [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) — Mô hình giọng nói với ASR cho 50+ ngôn ngữ, cảm xúc, sự kiện âm thanh và suy luận không tự hồi quy nhanh.

### Nhập liệu bằng giọng nói cấp hệ thống / IME

Các giải pháp nhập liệu bằng giọng nói tích hợp ở cấp hệ thống, bao gồm phương thức nhập liệu, tiện ích mở rộng IBus/Fcitx, IME Android và bàn phím iOS.

- [Whisper IME](https://github.com/woheller69/whisperIME) — IME Android và dịch vụ nhập liệu bằng giọng nói sử dụng Whisper để nhận dạng giọng nói ngoại tuyến và dịch sang tiếng Anh.
- [Vocalinux](https://github.com/jatinkrmalik/vocalinux) — Ứng dụng nhập liệu bằng giọng nói ngoại tuyến trên Linux với các công cụ whisper.cpp, Whisper và VOSK, GPU Vulkan và giao diện GTK.
- [blurt](https://github.com/QuantiusBenignus/blurt) — Tiện ích mở rộng GNOME Shell để nhập liệu bằng giọng nói ngoại tuyến qua whisper.cpp với kích hoạt phím nóng, hỗ trợ X11 và Wayland.
- [Vosk Android Service](https://github.com/alphacep/vosk-android-service) — Dịch vụ nhận dạng giọng nói ngoại tuyến trên Android sử dụng Vosk với hỗ trợ API RecognitionService chuẩn.
- [Dictus](https://github.com/getdictus/dictus-ios) — Bàn phím iOS mã nguồn mở để nhập liệu bằng giọng nói trên thiết bị sử dụng WhisperKit và CoreML, hoạt động trong bất kỳ ứng dụng nào.
- [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) — Phương thức nhập liệu bằng giọng nói IBus trên Linux với streaming STT, tùy chọn tinh chỉnh Whisper và tăng tốc GPU.

### Nhập liệu bằng giọng nói tiếng Trung / IME

Các dự án được tối ưu hóa cho nhận dạng và nhập liệu giọng nói tiếng Trung, bao gồm các IME và bàn phím tiếng Trung dựa trên FunASR, Paraformer và SenseVoice.

- [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Nhập liệu bằng giọng nói tiếng Trung ngoại tuyến trên Linux sử dụng FunASR Paraformer, IBus/Fcitx5, phím nóng PTT và chỉnh sửa câu.
- [voice-input-method](https://github.com/pofice/voice-input-method) — Phương thức nhập liệu bằng giọng nói ngoại tuyến đa nền tảng sử dụng FunASR, với sửa từ khóa, tự động dán và chế độ GUI/CLI.
- [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) — Bàn phím nhập liệu bằng giọng nói trên Android với 11 công cụ ASR, xử lý hậu kỳ LLM, bong bóng nổi và giao diện Material3.

### Nhập liệu bằng giọng nói trên trình duyệt và web

Nhập liệu bằng giọng nói trên trình duyệt qua tiện ích mở rộng, bao bọc WebAssembly hoặc giao diện web, thường yêu cầu backend STT cục bộ hoặc đám mây.

- [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) — Giao diện web Gradio cho Whisper để tạo phụ đề từ file, YouTube hoặc mic, với VAD, tách BGM và diarization.
- [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) — Tiện ích mở rộng trình duyệt để nhận dạng giọng nói thành văn bản ngoại tuyến theo thời gian thực qua Vosk, với lệnh thoại tiếng Ả Rập và tiếng Anh.
- [vosk-browser](https://github.com/ccoreilly/vosk-browser) — Thư viện nhận dạng giọng nói ngoại tuyến trên trình duyệt đóng gói Vosk dưới dạng WebAssembly chạy trong WebWorker.
- [Speechfire](https://github.com/Jejkobb/Speechfire) — Tiện ích mở rộng trình duyệt và máy chủ Whisper cục bộ để nhận dạng giọng nói thành văn bản ngoại tuyến trong Firefox và Chrome qua Alt+A.
- [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) — Tiện ích mở rộng Chrome ghi âm giọng nói qua phím nóng, phiên âm bằng OpenAI Whisper API và tự động dán văn bản.
- [voico](https://github.com/Kirera-Wainaina/voico) — Tiện ích mở rộng Chrome để nhập liệu bằng giọng nói vào các trường web, với backend Node.js sử dụng STT của Google và OpenAI.

### Nhập liệu bằng giọng nói trên di động (không phải IME)

Các ứng dụng phiên âm giọng nói độc lập trên Android hoặc iOS, thay vì bàn phím phương thức nhập liệu.

- [Transcribro](https://github.com/soupslurpr/Transcribro) — Bàn phím nhận dạng giọng nói riêng tư trên thiết bị Android sử dụng Whisper qua whisper.cpp và Silero VAD.
- [WhisperBoard](https://github.com/Saik0s/Whisperboard) — Ứng dụng iOS mã nguồn mở để phiên âm giọng nói ngoại tuyến sử dụng Whisper.cpp, với ghi âm và xuất âm thanh.
- [seamless](https://github.com/woheller69/seamless) — Ứng dụng dịch thuật ngoại tuyến giọng nói sang văn bản trên Android sử dụng Meta Seamless M4T Lite cho 5 ngôn ngữ với đầu ra TTS.

### Tập lệnh nhẹ, CLI và điều khiển bằng giọng nói

Các tập lệnh nhẹ, công cụ CLI, trình kích hoạt khay hệ thống hoặc tiện ích phù hợp để tích hợp cho nhà phát triển hoặc bổ sung cho chuỗi công cụ hiện có.

- [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — Công cụ nhận dạng giọng nói ngoại tuyến trên Linux sử dụng Vosk, mô phỏng đầu vào bàn phím vào bất kỳ ứng dụng nào.
- [voice_typing](https://github.com/themanyone/voice_typing) — Tập lệnh Bash để nhập liệu bằng giọng nói ngoại tuyến qua Whisper cho TTY, X11, Wayland và WSL với tùy chọn chỉnh sửa bằng LLM.
- [hns](https://github.com/primaprashant/hns) — Công cụ CLI để nhận dạng giọng nói từ mic cục bộ sử dụng faster-whisper, với sao chép khay nhớ tạm và đổ ra stdout.
- [Elograf](https://github.com/papoteur-mga/elograf) — Trình quản lý giao diện PyQt6 cho nerd-dictation với khay hệ thống, mô hình Vosk, mô phỏng đầu vào và phím nóng KDE.
- [Osprey](https://github.com/osprey-voice/osprey) — Công cụ điều khiển bằng giọng nói và nhập liệu dựa trên lệnh sử dụng Kaldi và Dragonfly cho nhận dạng giọng nói hoàn toàn cục bộ.

### Khác

Các dự án chưa được xếp vào danh mục.

- [VoxType](https://github.com/peteonrails/voxtype) — Nhập liệu bằng giọng nói nhấn để nói trên Linux và Wayland với bảy công cụ ASR cục bộ, hỗ trợ GPU và chế độ họp.

## Mã nguồn mở so với sản phẩm tham chiếu

| Dự án | Giá | Mã nguồn mở | Có thể mở rộng | Ngoại tuyến | Tiếng Trung |
| --- | --- | --- | --- | --- | --- |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ◐ |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ◐ |
| [VoxType](https://github.com/peteonrails/voxtype) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ✅ |
| [voice_typing](https://github.com/themanyone/voice_typing) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ⚠️ |
| [Handy](https://github.com/cjpais/Handy) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ◐ |
| [Buzz](https://github.com/chidiwilliams/buzz) | Miễn phí (OSS) | ✅ | ✅ | ✅ | ◐ |
| Typeless *(closed)* | Freemium: Free 8K wks/wk; Pro $12/mo yrly ($30/mo monthly) | ❌ | ❌ | ⚠️ | ⚠️ |
| Lazytype *(closed)* | Personal €25 one-time (BYOK Groq); Pro €5/mo hosted | ❌ | ❌ | ◐ | ⚠️ |
| Shandianshuo (闪电说) *(closed)* | Free (local/BYOK); Pro ¥29/mo or ¥238.8/yr | ❌ | ❌ | ◐ | ◐ |

## Cách chọn

- **Ứng dụng để bàn đa nền tảng hoàn thiện** → [Handy](https://github.com/cjpais/Handy) — Rust/Tauri, 25,281 sao, Whisper/Parakeet ngoại tuyến.
- **Linux ngoại tuyến tối giản, có thể viết script** → [nerd-dictation](https://github.com/ideasman42/nerd-dictation) — VOSK, mô phỏng đầu vào bàn phím vào bất kỳ ứng dụng nào.
- **Nhúng STT vào ứng dụng của bạn** → [whisper.cpp](https://github.com/ggml-org/whisper.cpp) — C/C++ Whisper, CPU/GPU, có thể nhúng.
- **Ưu tiên nhập liệu tiếng Trung** → [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) — Python, C++, Shell; Nhập liệu giọng nói tiếng Trung ngoại tuyến trên Linux sử dụng FunASR Paraformer, IBus/Fcitx5, phím nóng PTT và chỉnh sửa câu.
- **Tự lưu trữ API/server phiên âm** → [FunASR](https://github.com/modelscope/FunASR) — Bộ công cụ ASR công nghiệp với Paraformer, SenseVoice, VAD, diarization, streaming và API tương thích OpenAI.

## Đóng góp

Mọi đóng góp đều được hoan nghênh — xem [CONTRIBUTING.md](CONTRIBUTING.md). Các dự án phải hoàn toàn mã nguồn mở, có thể mở rộng và nhẹ; vui lòng tuân thủ hướng dẫn phong cách mô tả (bằng tiếng Anh, một dòng, mang tính thực tế, không quảng cáo thổi phồng).

## Lịch sử Star

![Star History](https://api.star-history.com/svg?repos=cjpais/Handy,ggml-org/whisper.cpp,FunAudioLLM/SenseVoice,mkiol/dsnote,ideasman42/nerd-dictation,peteonrails/voxtype&type=Date)

Sự tăng trưởng star theo thời gian đối với các dự án được gắn sao nhiều nhất trong danh sách này. Repo chính được giữ ở chế độ riêng tư trong quá trình kiểm duyệt; lịch sử star của chính nó sẽ được thêm vào đây sau khi công khai.

## Giấy phép

[MIT](LICENSE).

# Awesome Voice Input · 开源语音输入软件精选

> 一份精选的**完全开源**语音输入 / 听写 / AI 语音转写工具清单。对标 Typeless、Lazytype、闪电说,聚焦三大收录标准:**完全开源 · 可扩展 · 轻量**。

## 为什么有这份清单

Typeless / Lazytype / 闪电说 都是优秀的商业语音输入产品,但都**闭源 / 付费**。如果你想要"代码全公开、能自己加功能、装上就能跑"的开源替代,这份清单给你一张地图。所有项目均经 `gh api` 实测核验仓库真实存在,并经对抗验证复核开源/轻量/可扩展三项声明。

## 收录标准

| 标准 | 含义 |
|---|---|
| ✅ 完全开源 | OSI 认证许可证,代码全公开,非 open-core / 云增值收费 |
| 🔌 可扩展 | 插件 / API / 配置 / 模块化架构,能加自己的功能 |
| ⚡ 轻量 | 依赖少、安装简单;纯 CPU 可跑优先(GPU 仅加速) |

## 对标产品速览

| 产品 | 开源 | 定价 | 定位 | 技术栈 |
|---|---|---|---|---|
| Typeless | ❌ | 免费 8000 词/周;Pro $12/月起(年付) | macOS/Win/iOS/And AI 听写,深度 OS 集成+上下文感知 | Electron+React+Swift native;云端 AI API |
| Lazytype | ❌ | Personal €25 买断(BYOK);Pro €5/月 | Win/macOS 按住即说,Whisper+Groq,本地 whisper.cpp 可离线 | Python+PyInstaller;Whisper large-v3-turbo |
| 闪电说 | ❌ | Basic 免费(本地/BYOK);Pro ¥29/月 | 中文 AI 语音输入法+沟通 Agent,本地 SenseVoice,长按唤起 Agent | SenseVoiceSmall 本地+OpenAI 兼容 LLM;跨平台桌面 |

三款均闭源,故以下开源清单即为你可自主掌控的替代。

## 🏆 精选推荐(Top Picks)

综合三标准最优:

> 🌟 **社区旗舰:[Handy](https://github.com/cjpais/Handy)** ⭐25281 — 25k+ stars、跨平台(Win/Mac/Linux)、完全离线、可扩展(Tauri+Rust,支持 Raycast 扩展 / CLI 远程控制 / 自定义 Whisper GGML 模型 / 多 ASR 引擎),至今仍活跃更新。fit_score=4(构建需 Rust 工具链、GPU 仅加速项,轻量略减分),但综合社区规模与实用完整度,是绝大多数用户的首选。

- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** ⭐1882 — 基于 VOSK-API 的 Linux 离线语音转文字工具。通过手动 begin/end 命令激活，可将识别结果模拟成键盘输入注入到任意应用，也可输出到 stdout。核心定位是"为任何应用输入文字"，脚本化程度高，支持自定义文本后处理。。推荐依据:fit_score=5, 开源/可扩展/轻量=✅/✅/✅。
- **[voice_typing](https://github.com/themanyone/voice_typing)** ⭐155 — 基于 OpenAI Whisper/Whisper.cpp 的轻量 Shell 脚本，实现 Linux TTY、X/Wayland 或 Windows WSL 环境下的离线语音打字。通过 sox 录音、ydotool 模拟键盘输入，把语音实时转换为文本并键入任意活动文本域；同时提供 voice_client/voice_client_local 客户端/服务端模式，以及可选的 llama_edit 流式编辑。。推荐依据:fit_score=5, 开源/可扩展/轻量=✅/✅/✅。
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** ⭐51163 — OpenAI Whisper 自动语音识别（ASR）模型的高性能 C/C++ 移植实现，支持纯 CPU、量化及多种 GPU（Metal/CUDA/Vulkan/ROCm/OpenVINO/Ascend 等）加速推理，可作为实时语音转文字引擎嵌入其他应用。。推荐依据:fit_score=5, 开源/可扩展/轻量=✅/✅/✅。
- **[VoxType](https://github.com/peteonrails/voxtype)** ⭐909 — Local push-to-talk voice-to-text for Linux/Wayland (and macOS), running multiple ASR engines (Whisper, Parakeet, Moonshine, SenseVoice, Paraformer, Dolphin, Omnilingual) locally on CPU or optional GPU (Vulkan/CUDA/Metal/ROCm).。推荐依据:fit_score=5, 开源/可扩展/轻量=✅/✅/✅。
- **[Dabri](https://github.com/AshBuk/dabri)** ⭐110 — Linux 原生离线语音转文字（STT）应用，基于 whisper.cpp 构建，支持隐私优先的本地语音识别。可作为后台守护进程运行并集成系统托盘，也可作为 CLI 工具调用，还提供 WebSocket 服务器用于外部集成。支持 X11/Wayland、GNOME/KDE 等桌面环境，输出支持自动键入活动窗口或写入剪贴板。。推荐依据:fit_score=4, 开源/可扩展/轻量=✅/✅/✅。

## 全部项目速查表

| 名称 | 类别 | 开源 | 可扩展 | 轻量 | GPU需求 | 中文 | 平台 | ⭐ | License | Fit |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| [whisper-dictation](https://github.com/ashwin-pc/whisper-dictation) | 语音识别/生产力工具 | ✅ | ⚠️ | ⚠️ | 无 | 否 | Mac | 25 | MIT | 2 |
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | AI / Machine Learning - Speech Recognition (ASR) | ✅ | ✅ | ✅ | 可选 | 部分 | Mac/iOS/Android/Linux/Win | 51163 | MIT | 5 |
| [nerd-dictation](https://github.com/ideasman42/nerd-dictation) | Speech-to-Text Utility | ✅ | ✅ | ✅ | 无 | 部分 | Linux | 1882 | GPL-3.0 | 5 |
| [VoxType](https://github.com/peteonrails/voxtype) | 语音转文字工具 | ✅ | ✅ | ✅ | 可选 | 是 | Linux/Mac | 909 | MIT | 5 |
| [voice_typing](https://github.com/themanyone/voice_typing) | voice typing / accessibility / productivity tool | ✅ | ✅ | ✅ | 可选 | 否 | Linux/Win | 155 | GPL-2.0 | 5 |
| [Buzz](https://github.com/chidiwilliams/buzz) | Audio / Speech / Desktop Application | ✅ | ✅ | ⚠️ | 可选 | 部分 | Win/Mac/Linux | 19906 | MIT | 4 |
| [FunASR](https://github.com/modelscope/FunASR) | Speech Recognition / ASR Toolkit | ⚠️ | ✅ | ⚠️ | 无 | 是 | Linux/Mac/Win/Web/Android/iOS | 18745 | MIT | 4 |
| [vosk-api](https://github.com/alphacep/vosk-api) | Speech Recognition (STT) | ⚠️ | ✅ | ✅ | 无 | 否 | Win/Mac/Linux/Web/Android/iOS | 14889 | Apache-2.0 | 4 |
| [sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx) | 离线语音工具包 | ✅ | ✅ | ⚠️ | 无 | 是 | Android/iOS/Win/Mac/Linux | 13280 | Apache-2.0 | 4 |
| [Vibe](https://github.com/thewh1teagle/vibe) | Audio/Video Transcription | ✅ | ✅ | ✅ | 无 | 是 | Win/Mac/Linux | 6635 | MIT | 4 |
| [Epicenter](https://github.com/EpicenterHQ/epicenter) | Productivity / Local-first Developer Toolkit | ✅ | ✅ | ⚠️ | 无 | 部分 | Win/Mac/Linux/Web | 4663 | MIT + AGPL-3.0-or-later | 4 |
| [Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI) | 语音转写 / 字幕生成工具 | ✅ | ✅ | ⚠️ | 可选 | 部分 | Win/Mac/Linux/Web | 2821 | Apache-2.0 | 4 |
| [typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac) | Speech-to-text / AI dictation | ✅ | ✅ | ✅ | 无 | 否 | Mac | 1541 | GPL-3.0 | 4 |
| [OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper) | 语音转录/生产力工具 | ✅ | ⚠️ | ⚠️ | 无 | 是 | Mac | 1474 | MIT | 4 |
| [Amical](https://github.com/amicalhq/amical) | AI 语音/听写工具 | ✅ | ✅ | ⚠️ | 无 | 否 | Win/Mac/Linux/Web/Android/iOS | 1388 | MIT | 4 |
| [hyprwhspr](https://github.com/goodroot/hyprwhspr) | Speech-to-Text | ✅ | ✅ | ⚠️ | 可选 | 否 | Linux | 1074 | MIT | 4 |
| [whisper-writer](https://github.com/savbell/whisper-writer) | Speech-to-text desktop application | ✅ | ✅ | ⚠️ | 可选 | 部分 | Win/Mac/Linux | 1071 | GPL-3.0 | 4 |
| [Transcribro](https://github.com/soupslurpr/Transcribro) | Speech Recognition / Android Utility | ✅ | ✅ | ✅ | 无 | 否 | Android | 723 | ISC | 4 |
| [Whisper IME](https://github.com/woheller69/whisperIME) | Speech Recognition / Android Input Method | ✅ | ✅ | ✅ | 无 | 部分 | Android | 603 | MIT | 4 |
| [Vocalinux](https://github.com/jatinkrmalik/vocalinux) | Voice dictation / accessibility | ✅ | ✅ | ✅ | 可选 | 否 | Linux | 404 | GPL-3.0 | 4 |
| [VoiceTypr](https://github.com/moinulmoin/voicetypr) | 语音转文字 / 生产力工具 | ✅ | ✅ | ✅ | 可选 | 部分 | Mac/Win | 389 | AGPL-3.0 | 4 |
| [HoldSpeak](https://github.com/karolswdev/HoldSpeak) | 本地语音助手 / 会议转写 | ✅ | ✅ | ⚠️ | 无 | 部分 | Mac/Linux/Web | 277 | Apache-2.0 | 4 |
| [Chirp](https://github.com/Whamp/chirp-stt) | Speech-to-Text | ✅ | ✅ | ✅ | 无 | 否 | Win | 191 | MIT | 4 |
| [VocoType-linux](https://github.com/LeonardNJU/VocoType-linux) | 开源输入法/语音输入项目评估 | ✅ | ✅ | ✅ | 无 | 是 | Linux | 163 | GPL-3.0 | 4 |
| [Dabri](https://github.com/AshBuk/dabri) | Speech-to-Text / Voice Tools | ✅ | ✅ | ✅ | 无 | 否 | Linux | 110 | MIT | 4 |
| [hns](https://github.com/primaprashant/hns) | 语音转文本 CLI 工具 | ✅ | ✅ | ✅ | 可选 | 部分 | Linux/Mac/Win | 107 | MIT | 4 |
| [QuickDictate](https://github.com/kristian-dott-42/QuickDictate) | macOS 语音听写工具 | ✅ | ✅ | ✅ | 无 | 否 | Mac | 1 | MIT | 4 |
| [Handy](https://github.com/cjpais/Handy) | Desktop Speech-to-Text / Voice Input | ✅ | ✅ | ⚠️ | 可选 | 部分 | Win/Mac/Linux | 25281 | MIT | 4 |
| [Voicisst](https://github.com/lucyfromnaarm/voicisst) | AI Voice Dictation / Local Speech-to-Text | ✅ | ✅ | ⚠️ | 无 | 部分 | Linux/Mac/Win/Web | 0 | MIT | 4 |
| [Elograf](https://github.com/papoteur-mga/elograf) | Desktop Utility / Voice Recognition | ✅ | ✅ | ✅ | 无 | 否 | Linux | 82 | GPL-3.0 | 4 |
| [VoiceFlow](https://github.com/infiniV/VoiceFlow) | productivity | ✅ | ⚠️ | ✅ | 可选 | 部分 | Win/Linux | 393 | MIT | 3.5 |
| [voice-input-method](https://github.com/pofice/voice-input-method) | Speech Recognition / Input Method | ✅ | ✅ | ✅ | 无 | 是 | Linux/Win/Mac | 38 | GPL-3.0-or-later | 3.5 |
| [dsnote (Speech Note)](https://github.com/mkiol/dsnote) | desktop-application | ✅ | ⚠️ | ⚠️ | 可选 | 否 | Linux | 1525 | MPL-2.0 | 3.5 |
| [Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension) | Browser Extension | ⚠️ | ✅ | ✅ | 无 | 否 | Web/Linux/Mac/Win | 0 | MIT | 3.5 |
| [PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech) | Speech/Audio AI Toolkit | ✅ | ✅ | ⚠️ | 无 | 是 | Linux/Win/Mac/Web/Android | 12636 | Apache-2.0 | 3 |
| [VoiceInk](https://github.com/Beingpax/VoiceInk) | 语音转写工具 | ✅ | ⚠️ | ✅ | 无 | 部分 | Mac | 5387 | GPL-3.0 | 3 |
| [FluidVoice](https://github.com/altic-dev/FluidVoice) | Voice-to-Text Dictation / Speech Recognition | ⚠️ | ✅ | ⚠️ | 无 | 部分 | Mac | 5013 | GPL-3.0 | 3 |
| [OpenWhispr](https://github.com/OpenWhispr/openwhispr) | voice-to-text | ✅ | ✅ | ⚠️ | 无 | 部分 | Mac/Win/Linux | 4143 | MIT | 3 |
| [Ghost Pepper](https://github.com/matthartman/ghost-pepper) | 语音识别/本地 AI 转录工具 | ✅ | ⚠️ | ⚠️ | 无 | 部分 | Mac | 2800 | MIT | 3 |
| [WhisperBoard](https://github.com/Saik0s/Whisperboard) | Voice transcription / Mobile app | ✅ | ⚠️ | ✅ | 无 | 否 | iOS | 1040 | GPL-3.0 | 3 |
| [BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard) | mobile voice input method / Android keyboard | ⚠️ | ✅ | ⚠️ | 无 | 是 | Android | 695 | Apache-2.0 | 3 |
| [Pindrop](https://github.com/watzon/pindrop) | Voice / Productivity | ✅ | ✅ | ⚠️ | 无 | 否 | Mac | 546 | MIT | 3 |
| [vosk-browser](https://github.com/ccoreilly/vosk-browser) | Browser speech recognition / WebAssembly | ✅ | ✅ | ✅ | 无 | 部分 | Web | 520 | Apache-2.0 | 3 |
| [Tambourine Voice](https://github.com/kstonekuan/tambourine-voice) | AI Voice Dictation / 语音输入工具 | ✅ | ⚠️ | ⚠️ | 可选 | 否 | Win/Mac/Linux | 366 | AGPL-3.0 | 3 |
| [OpenTypeless](https://github.com/tover0314-w/opentypeless) | Desktop AI Voice Input / Productivity | ✅ | ⚠️ | ✅ | 无 | 是 | Win/Mac/Linux | 308 | MIT | 3 |
| [voxd](https://github.com/jakovius/voxd) | 语音听写/语音识别 | ✅ | ⚠️ | ⚠️ | 无 | 部分 | Linux | 266 | MIT | 3 |
| [whisper-dictation](https://github.com/foges/whisper-dictation) | Productivity / Speech-to-Text | ✅ | ⚠️ | ✅ | 可选 | 部分 | Mac/Linux | 219 | MIT | 3 |
| [blurt](https://github.com/QuantiusBenignus/blurt) | Desktop utility / GNOME Shell extension | ✅ | ⚠️ | ⚠️ | 无 | 部分 | Linux | 107 | GPL-3.0 | 3 |
| [better-voice-typing](https://github.com/Elevate-Code/better-voice-typing) | voice typing / speech-to-text desktop app | ✅ | ✅ | ✅ | 无 | 否 | Win | 77 | MIT | 3 |
| [Aria](https://github.com/Xingxun7777/Aria) | AI 语音输入工具 / 语音输入法 | ✅ | ✅ | ⚠️ | 无 | 是 | Win | 71 | Apache-2.0 | 3 |
| [Vosk Android Service](https://github.com/alphacep/vosk-android-service) | Android 离线语音识别服务 | ✅ | ✅ | ✅ | 无 | 部分 | Android | 64 | Apache-2.0 | 3 |
| [speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant) | 语音转文字 / 桌面应用 | ✅ | ✅ | ⚠️ | 可选 | 否 | Linux/Win | 59 | MIT | 3 |
| [TalkType](https://github.com/lmacan1/talktype) | Developer Tool / Voice Input | ✅ | ⚠️ | ⚠️ | 无 | 部分 | Linux/Win/Mac | 54 | MIT | 3 |
| [FnKey](https://github.com/evoleinik/fnkey) | productivity | ✅ | ⚠️ | ✅ | 无 | 否 | Mac | 45 | GPL-3.0 | 3 |
| [faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation) | 语音转文字/听写工具 | ✅ | ⚠️ | ✅ | 无 | 部分 | Win/Mac/Linux | 29 | MIT | 3 |
| [Speechfire](https://github.com/Jejkobb/Speechfire) | Browser Extension / Speech-to-Text Tool | ⚠️ | ✅ | ⚠️ | 可选 | 部分 | Win/Linux/Web | 27 | None | 3 |
| [Osprey](https://github.com/osprey-voice/osprey) | Voice Control / Accessibility | ✅ | ✅ | ⚠️ | 无 | 部分 | Linux/Mac | 26 | MIT | 3 |
| [whisper-dictation](https://github.com/jacopone/whisper-dictation) | 语音听写 / 生产力工具 | ✅ | ✅ | ✅ | 可选 | 否 | Linux | 18 | MIT | 3 |
| [OpenFlow](https://github.com/SadmanMahi67/OpenFlow) | AI 语音转写 / 桌面生产力工具 | ✅ | ⚠️ | ⚠️ | 无 | 否 | Win | 15 | MIT | 3 |
| [Whisper-Paste](https://github.com/redocrepus/Whisper-Paste) | Browser Extension / Voice-to-Text | ✅ | ✅ | ✅ | 无 | 否 | Web/Win/Mac/Linux | 13 | MIT | 3 |
| [Dictus](https://github.com/getdictus/dictus-ios) | iOS Voice Dictation Keyboard | ✅ | ✅ | ✅ | 无 | 否 | iOS | 12 | MIT | 3 |
| [voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux) | input-method/speech-recognition | ⚠️ | ✅ | ⚠️ | 可选 | 否 | Linux | 11 | MIT | 3 |
| [hush](https://github.com/djmunro/hush) | Productivity | ✅ | ✅ | ⚠️ | 无 | 否 | Mac | 6 | MIT | 3 |
| [freespeak](https://github.com/Zetaphor/freespeak) | voice typing / accessibility | ✅ | ✅ | ⚠️ | 无 | 否 | Linux | 6 | MIT | 3 |
| [Speed of Sound](https://github.com/zugaldia/speedofsound) | 语音识别/桌面辅助工具 | ✅ | ✅ | ⚠️ | 无 | 部分 | Linux | 171 | MIT | 3 |
| [WhisperDictation](https://github.com/sam-pop/WhisperDictation) | Voice / Speech-to-Text | ✅ | ⚠️ | ✅ | 可选 | 否 | Mac | 1 | MIT | 3 |
| [localflow](https://github.com/sidharth-n/localflow) | AI voice dictation tool | ⚠️ | ✅ | ✅ | 可选 | 部分 | Linux | 0 | Apache-2.0 | 3 |
| [yammer](https://github.com/andynu/yammer) | voice input / productivity tool | ✅ | ✅ | ⚠️ | 可选 | 否 | Linux | 0 | MIT | 3 |
| [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) | Speech Recognition / ASR | ⚠️ | ✅ | ✅ | 可选 | 是 | Linux/Win/Mac/Web/Android/iOS | 8731 | MIT（通过引用 FunASR 的 MIT 许可证；GitHub API 自身显示 NOASSERTION） | 3 |
| [voico](https://github.com/Kirera-Wainaina/voico) | Browser Extension / Speech-to-Text | ✅ | ⚠️ | ⚠️ | 无 | 否 | Win/Mac/Linux/Web | 1 | MIT（仅 package.json 声明，无根目录 LICENSE 文件） | 3 |
| [Voquill](https://github.com/voquill/voquill) | Open source voice dictation/AI typing assistant | ⚠️ | ✅ | ⚠️ | 可选 | 否 | Mac/Win/Linux/Web/iOS/Android | 977 | AGPL-3.0 (with enterprise-directory exception) | 3 |
| [whisper_dictation](https://github.com/themanyone/whisper_dictation) | Voice AI / Desktop Automation | ✅ | ✅ | ⚠️ | 可选 | 部分 | Linux/Win | 291 | GPL-2.0 | 2 |
| [OmniDictate](https://github.com/gurjar1/OmniDictate) | Real-time AI Dictation / Speech-to-Text Desktop App | ⚠️ | ⚠️ | ⚠️ | 可选 | 部分 | Win | 141 | CC BY-NC 4.0 | 2 |
| [seamless](https://github.com/woheller69/seamless) | Android App | ⚠️ | ⚠️ | ⚠️ | 无 | 否 | Android | 84 | MIT | 2 |
| [Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation) | voice dictation tool | ✅ | ⚠️ | ⚠️ | 无 | 部分 | Linux | 9 | GPL-3.0 | 2 |

## 分类清单

### 跨平台/Linux/Windows 桌面实时听写
以 Whisper / faster-whisper / whisper.cpp 为核心的桌面听写应用，覆盖 Linux、Windows 或跨平台，主打“按住说话 → 本地转写 → 自动输入”。部分项目可选 GPU 加速，多数 CPU 可跑。
- **[Handy](https://github.com/cjpais/Handy)** ⭐25281 · MIT · Rust + Tauri, React + TypeScript, Tailwind CSS · Win/Mac/Linux · 中文 部分
  跨平台桌面端离线语音输入/转文字工具，按下快捷键录音，本地 Whisper 或 Parakeet 模型转录后直接粘贴到当前文本框。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(可选 GPU 加速，Parakeet V3 CPU-only 在中端 CPU 上约 5 倍实时；提供 Homebrew cask、winget 与 GitHub…) | 活跃度:active(2026-06-30)
  - 核心特性:完全离线运行，音频/模型均本地、支持 Whisper (Small/Medium/Turbo/Large) 与 Parakeet V3、GPU 仅用于加速，Parakeet 可纯 CPU 运行、全局快捷键 / 按键对讲 (push-to-talk)、自动语言检测 (Parakeet)
- **[Buzz](https://github.com/chidiwilliams/buzz)** ⭐19906 · MIT · Python 3.12, PyQt6, OpenAI Whisper, Faster-Whisper, Whisper.cpp, PyTorch, transformers, ONNX Runtime · Windows/macOS/Linux · 中文 部分
  Cross-platform desktop GUI for offline audio transcription and translation, powered by OpenAI Whisper.
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Python + Qt GUI, but depends on PyTorch, OpenAI Whisper, Faster-Whisper, transfo…) | 活跃度:active(2026-06-30)
  - 核心特性:Offline audio/video transcription and translation、Live microphone transcription with presentation window、Multiple Whisper backends (OpenAI Whisper, Faster-Whisper, Whisper.cpp, stable-ts)、GPU acceleration: CUDA, Apple Silicon, Vulkan、Export to TXT, SRT, VTT
  - ⚠️ 注意:Heavy ML dependency stack; first model download can be large; CPU transcription is slower than GPU. No mobile or web version.
- **[Vibe](https://github.com/thewh1teagle/vibe)** ⭐6635 · MIT · Rust（Tauri 后端 / whisper.cpp 绑定）、TypeScript（React/Vite 前端）、Python（构建脚本 / 辅助工具）、whisper.cpp · Windows/macOS/Linux · 中文 是
  Vibe 是一款跨平台桌面语音/视频转录应用，基于 OpenAI Whisper 模型实现本地离线音频/视频转写，支持 SRT/VTT/TXT/HTML/PDF/JSON/DOCX 等多种输出格式、说话人分离、系统/麦克风录音、实时预览、批量处理、字幕长度优化，并可通过 Claude/Ollama 对转录结果进行总结。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-05-01)
  - 核心特性:离线音频/视频转录、多语言识别（含中文 UI 与中文语音识别）、SRT/VTT/TXT/HTML/PDF/JSON/DOCX 导出、说话人分离、系统音频与麦克风录制
  - ⚠️ 注意:模型文件本身较大（tiny 到 large-v3-turbo 等级），首次使用需下载; GPU 为可选项，CPU 亦可运行但速度较慢; iOS/Android 支持仍在规划中; 可选 Aptabase 分析仅在构建时开启，不影响核心功能。
- **[Epicenter](https://github.com/EpicenterHQ/epicenter)** ⭐4663 · MIT + AGPL-3.0-or-later · 未知 · Win/Mac/Linux/Web · 中文 部分
  Local-first apps toolkit and a desktop speech-to-text app (Whispering). Data lives on the user's machine as plain Markdown and SQLite; apps sync via Yjs CRDTs and can project state to Markdown/SQLite…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(End users can install Whispering via `brew install --cask whispering` or OS inst…) | 活跃度:active(2026-07-01)
- **[hyprwhspr](https://github.com/goodroot/hyprwhspr)** ⭐1074 · MIT · Python; C/C++ bindings through pywhispercpp/onnxruntime; optional GTK4/PyCairo visualizer; Astro website. · Linux · 中文 否
  Native speech-to-text for Linux. Provides system-wide dictation using local/on-device models (Whisper, Parakeet, Cohere Transcribe via ONNX) and optional cloud or realtime APIs (OpenAI, Groq, Regolo,…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(The core package is small Python, but it depends on audio/ML libraries (numpy, s…) | 活跃度:active(2026-07-01)
  - 核心特性:System-wide speech-to-text on Linux、Local/on-device transcription (Whisper, Parakeet, Cohere via ONNX)、Cloud/realtime backend options (OpenAI, Groq, Google Gemini, ElevenLabs, Regolo)、Themed mic OSD visualizer with auto-theme matching、Waybar status integration
- **[whisper-writer](https://github.com/savbell/whisper-writer)** ⭐1071 · GPL-3.0 · Python · Windows/Mac/Linux · 中文 部分
  A desktop speech-to-text app that records from the microphone when a global hotkey is pressed and transcribes the audio into the currently active window using OpenAI Whisper, either via a local…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Python 3.11 项目，requirements.txt 包含 76 项依赖（faster-whisper、PyQt5、openai、numpy、onnx…) | 活跃度:maintenance(2024-08-24)
  - 核心特性:Global hotkey-triggered dictation to the active window、Local transcription with faster-whisper (multiple model sizes)、Optional OpenAI API transcription with configurable base URL、Continuous / VAD / press-to-toggle / hold-to-record modes、PyQt5 settings/status windows and system tray icon
  - ⚠️ 注意:本地模型首次运行需下载 Whisper 模型文件（体积从几十 MB 到 GB 不等）; GPU 加速需额外安装 NVIDIA cuBLAS/cuDNN; 依赖 PyQt5 与大量 Python 包，安装复杂度中等; UI 与文档为英文，仅能通过 language 配置支持中文转写; 最近一次提交为 2024-08-24，更新节奏已放缓。
- **[Chirp](https://github.com/Whamp/chirp-stt)** ⭐191 · MIT · Python · Windows · 中文 否
  Windows dictation app that runs fully locally using ParakeetV3 STT. CPU-only, no GPU required, with global hotkey toggle, clipboard paste injection, configurable word overrides, audio feedback, and…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-02-27)
  - 核心特性:Local CPU-only STT with ParakeetV3、Global hotkey toggle、Clipboard paste injection / text typing、Configurable word overrides、Optional int8 quantization
  - ⚠️ 注意:Windows-centric; while config mentions non-Windows paste behavior, config paths and setup are Windows-specific, so cross-platform use is not guaranteed.
- **[Dabri](https://github.com/AshBuk/dabri)** ⭐110 · MIT · Go + whisper.cpp (CGO), YAML 配置 · Linux · 中文 否
  Linux 原生离线语音转文字（STT）应用，基于 whisper.cpp 构建，支持隐私优先的本地语音识别。可作为后台守护进程运行并集成系统托盘，也可作为 CLI 工具调用，还提供 WebSocket 服务器用于外部集成。支持 X11/Wayland、GNOME/KDE 等桌面环境，输出支持自动键入活动窗口或写入剪贴板。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-23)
  - 核心特性:离线本地语音识别、whisper.cpp 后端、X11/Wayland 兼容、系统托盘与 CLI 双模式、WebSocket / Unix socket 双 API
  - ⚠️ 注意:官方仅支持 Linux; README 与文档均为英文，UI 中文支持未体现; 依赖 whisper.cpp 模型文件，首次使用需下载模型。
- **[dsnote (Speech Note)](https://github.com/mkiol/dsnote)** ⭐1525 · MPL-2.0 · C++17, Qt5/QML, CMake, Python (optional components) · Linux/Sailfish OS · 中文 是
  Linux desktop and Sailfish OS app for offline note-taking, reading and translating via local Speech-to-Text, Text-to-Speech and Machine Translation. Integrates multiple engine choices (Vosk, Whisper,…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(Not lightweight in default configuration: depends on Qt5, Python (optional), CUD…) | 活跃度:active(2026-06-28)
  - 核心特性:Offline STT via Vosk / Whisper / Faster-Whisper / April-ASR / Coqui STT、Offline TTS via Piper / RHVoice / espeak / MBROLA / Coqui / Mimic3 / Kokoro / F5-TTS / Parler-TTS / WhisperSpeech / S.A.M.、Offline machine translation via Bergamot、Custom model support through config/models.json、CLI actions and global keyboard shortcuts for desktop integration
  - ⚠️ 注意:Default base Flatpak is large (1.2 GB download / 3.6 GB unpacked) due to bundled ML libraries; a 'Tiny' variant (48 MB / 170 MB) exists but drops many features. GPU acceleration requires separate NVIDIA or AMD add-ons. No native Windows, macOS, Android, or iOS builds. The actual license is MPL-2.0, not GPL.
- **[voxd](https://github.com/jakovius/voxd)** ⭐266 · MIT · Python · Linux · 中文 部分
  Linux desktop speech-to-text / voice dictation application. Runs in the background and types transcribed text into any focused input window using whisper.cpp for offline ASR, ydotool for simulated…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(README explicitly states 'Runs fine even on older CPUs. No GPU required.'; defau…) | 活跃度:active(2025-10-22)
  - 核心特性:Whisper.cpp offline/local ASR、Simulated typing via ydotool on Wayland/X11、Clipboard auto-copy、99+ spoken languages、AI post-processing with local or cloud LLMs
  - ⚠️ 注意:Linux-only; relies on native dependencies (whisper.cpp, ydotool, PyQt6) and downloads ASR/LLM models separately. Last upstream push ~9 months ago (as of 2026-07-01).
- **[Speed of Sound](https://github.com/zugaldia/speedofsound)** ⭐171 · MIT · Kotlin / JVM，GTK/GNOME 通过 Java-GI 绑定，Sherpa ONNX 运行 ASR 模型 · Linux · 中文 部分
  Linux 桌面级离线语音打字工具，通过全局快捷键或系统托盘触发，将语音直接输入到任意获得焦点的应用（X11/Wayland 均通过 XDG Desktop Portals 支持）。核心使用 Whisper/Parakeet/Canary 等 ONNX 模型在本地完成语音识别，可选接入 Anthropic/Google/OpenAI/自托管（Ollama/vLLM/llama.cpp）LLM…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(无需 GPU，CPU 即可本地推理；提供 Flathub/Snap 一键安装，也提供 AppImage/Deb/RPM；核心功能不依赖网络，可选 LLM 才需要…) | 活跃度:active(2026-06-06)
  - 核心特性:离线语音识别（Whisper/Parakeet/Canary）、全局快捷键/系统托盘/应用内按钮多种触发方式、通过 Desktop Portals 支持 X11/Wayland、多语言切换与内置多语言 Whisper 模型、可选本地或云端 LLM 润色
  - ⚠️ 注意:仅支持 Linux; 首次使用需下载额外语音识别模型（Whisper 等多语言模型体积较大）; 可选 LLM 润色若使用云服务会产生网络流量和 API 费用; JVM/GTK 栈对系统内存有一定要求。
- **[better-voice-typing](https://github.com/Elevate-Code/better-voice-typing)** ⭐77 · MIT · Python 3.10-3.12, tkinter, uv, LiteLLM · Windows · 中文 否
  A lightweight Windows desktop voice-typing assistant. Press Caps Lock to record audio, then send it to a configurable speech-to-text provider (OpenAI GPT-4o/Whisper, Google Cloud, or a custom/local…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2025-12-12)
  - 核心特性:Caps Lock hotkey recording toggle、System tray indicator with audio level、Multi-provider STT (OpenAI, Google Cloud, custom/local)、Optional LLM transcript cleaning/refinement、Recent transcription history
  - ⚠️ 注意:Windows-only and targets Python 3.10-3.12. The default STT path relies on cloud APIs (OpenAI GPT-4o-transcribe); local/offline use is supported but requires configuring a custom STT server endpoint. The prompt's mention of faster-whisper is not reflected in the current default implementation—local faster-whisper would be consumed through the custom STT provider.
- **[speech-assistant](https://github.com/Mohamad-Hussein/speech-assistant)** ⭐59 · MIT · Python 3.11 + PyTorch 2.3 + Transformers + customtkinter；可选 Ollama + Chainlit + LangChain · Linux/Windows · 中文 否
  一个面向 Linux 和 Windows 的桌面实时离线语音听写应用。默认使用 Hugging Face distil-whisper 模型（distil-small.en）将语音转写为文字并直接输入到光标处，同时可选集成 Ollama 本地 LLM 提供对话助手功能。所有处理在本地完成，无需 OpenAI API。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(默认 distil-small.en 约 166M 参数、运行时约 600 MB GPU/显存；提供 CPU-only 的 conda 环境（env-gener…) | 活跃度:maintenance(2025-10-16)
  - 核心特性:实时离线语音转文字（distil-whisper / Whisper）、按住 Win+Shift 热键开始/停止录音、支持多模型切换（tiny / small / medium / large）、可选英文翻译模式（Whisper-Large）、可选 Ollama 本地 LLM 助手对话
  - ⚠️ 注意:distil-whisper 系列目前主要是英语模型，多语言支持有限（仅 whisper-large 提供翻译）; 仅支持 Linux/Windows，无 macOS/Android/iOS; 助手功能依赖 Ollama; 最后一次代码更新在 2025-10-16，约 9 个月前，活跃度一般; 安装依赖 conda 和 pip，对新手有一定门槛。
- **[TalkType](https://github.com/lmacan1/talktype)** ⭐54 · MIT · Python · Linux/Windows/macOS · 中文 部分
  Push-to-talk voice typing for terminal/IDE. Press a hotkey, speak, press again; transcribes locally with faster-whisper and pastes text into the focused window. Works with any terminal, IDE, browser,…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(Installed as a single Python package with pip install -e .; system dependencies …) | 活跃度:active(2026-03-16)
  - 核心特性:Push-to-talk global hotkey (default F9)、Local Whisper transcription via faster-whisper、Cross-platform Linux/Windows/macOS、OpenAI-compatible API support、Configurable hotkeys, model sizes, and language
  - ⚠️ 注意:No formal plugin SDK; extensibility mainly comes from OpenAI-compatible API endpoints and YAML configuration. Large Whisper models (up to 3GB / ~10GB VRAM) can be heavy, though tiny/base models keep resource use modest.
- **[faster-whisper-dictation](https://github.com/doctorguile/faster-whisper-dictation)** ⭐29 · MIT · Python; faster-whisper; CTranslate2; onnxruntime; pyaudio; pynput · Windows/macOS/Linux · 中文 部分
  A multilingual, offline dictation application based on Faster-Whisper/CTranslate2. It runs in the background and is triggered by a global keyboard shortcut to record speech, transcribe it locally,…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:abandoned(2023-12-14)
  - 核心特性:Offline speech-to-text dictation、Global hotkey trigger、Multiple Whisper model sizes (tiny to large-v2)、CPU-first with optional GPU/CUDA、Cross-platform desktop (Windows/macOS/Linux)
  - ⚠️ 注意:Last pushed in Dec 2023, so the project appears unmaintained. Requires PortAudio system library and Hugging Face model download. No plugin/API architecture for extension.
- **[whisper-dictation](https://github.com/jacopone/whisper-dictation)** ⭐18 · MIT · Python 3.12 + Nix · Linux · 中文 是（依赖 Whisper 多语言模型，界面与文档为英文）
  基于 whisper.cpp 的 NixOS/Wayland 本地隐私语音听写工具，支持 Super+Period 按键触发、GTK4 实时状态窗口、99 语言自动检测/手动选择，并将转写文本自动粘贴到当前 Wayland 应用。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:maintenance(2026-02-15)
  - 核心特性:100% 本地处理，无云端/无遥测、Super+Period 按键触发听写、GTK4 浮动窗口实时反馈、99 语言自动检测或手动选择、模型尺寸可选（tiny 到 large）
  - ⚠️ 注意:仅支持 NixOS 或带 Nix 的 Linux + Wayland; 需将用户加入 input 组并手动下载 Whisper 模型; 首次配置还涉及 ydotoold、ffmpeg、PulseAudio/PipeWire 等系统依赖。作者活跃度一般（18 stars，最近一次提交 4 个月前）。
- **[freespeak](https://github.com/Zetaphor/freespeak)** ⭐6 · MIT · Python (PyQt6 overlay, DBus, torch/transformers/nemo-based STT) with a JavaScript/HTML/CSS web overlay UI · Linux · 中文 否
  A simple voice dictation application for Linux/Wayland that captures audio, transcribes it, corrects grammar via a local LanguageTool server, and types the result into the currently active window…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Not lightweight. pyproject.toml depends on PyQt6, PyQt6-WebEngine, torch, transf…) | 活跃度:maintenance(2025-04-11)
  - ⚠️ 注意:Despite GitHub classifying the repo as JavaScript, the core application is Python; the web/ directory appears to be a front-end overlay for the PyQt6 WebEngine view. The project is Linux/Wayland-only, has heavy deep-learning dependencies, involves non-trivial system configuration, and has been quiet for about 15 months (6 stars).
- **[whisper_dictation](https://github.com/themanyone/whisper_dictation)** ⭐291 · GPL-2.0 · Python, with C/C++ local AI servers (whisper.cpp, llama.cpp) and GStreamer audio pipeline · Linux/Windows · 中文 部分
  A private, local voice keyboard and desktop agent that combines speech-to-text (via whisper.cpp), LLM chat (via llama.cpp), image generation (via Stable Diffusion WebUI), webcam/audio capture, and…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Although the project itself is a small set of Python scripts, it depends on larg…) | 活跃度:active(2026-06-16)
  - 核心特性:Local speech-to-text dictation anywhere via whisper.cpp、AI chat via llama.cpp (local) or optional ChatGPT/Gemini (cloud)、Image generation via Stable Diffusion WebUI、Webcam capture and audio recording via voice commands、Voice-controlled app launching and desktop automation (X11/Wayland)
  - ⚠️ 注意:Requires >=4 GiB VRAM/GPU for the full feature set. Setup is Linux-centric (Arch/Fedora instructions, CUDA, GStreamer, udev rules for Wayland). Windows is mentioned only for terminal ANSI support; macOS is not documented. Running full AI stack locally is resource-intensive.
- **[OmniDictate](https://github.com/gurjar1/OmniDictate)** ⭐141 · CC BY-NC 4.0 · 未知 · Windows · 中文 部分
  Windows 桌面端的本地实时 AI 语音转文字工具，基于 faster-whisper/Whisper 模型，通过 PySide6 GUI 录制语音并直接模拟键盘输入到当前活动窗口，支持 VAD、按键说话、 spoken punctuation 与幻觉词过滤。
  - 开源 ⚠️ | 可扩展 ⚠️ | 轻量 ⚠️(依赖 torch、torchvision、torchaudio、faster-whisper、ctranslate2、transformers、PySide6 …) | 活跃度:active(2025-12-12)
  - 核心特性:Local real-time speech-to-text using faster-whisper、PySide6 slate/glass-style GUI、Voice Activity Detection (VAD) and Push-to-Talk (PTT)、Global hotkey support、Spoken punctuation commands
  - ⚠️ 注意:许可证为非商业 CC BY-NC 4.0，商业使用需授权; 仅支持 Windows（依赖 pywin32、pywinauto）; 预构建安装包未签名，会触发 Windows SmartScreen; 需要较大模型下载与 NVIDIA GPU/CUDA 才能达到可用性能。
- **[Whisper-Dictation](https://github.com/LumenYoung/Whisper-Dictation)** ⭐9 · GPL-3.0 · Python 3.10+ (Poetry 构建) · Linux · 中文 部分
  Linux 下基于 OpenAI Whisper 的语音听写工具，采用后台 daemon + 客户端触发架构。用户按下快捷键即可录音，停止后自动将转写文本写入剪贴板并通过 kdialog 弹出通知。专为 KDE Wayland 设计，提供 systemd 用户服务文件。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(Python 项目，核心依赖为 click、pyaudio 和 openai-whisper。虽然 `pip install whisper_dictation…) | 活跃度:maintenance(2023-04-11)
  - 核心特性:后台 Whisper daemon 避免重复加载模型、客户端 socket 触发录音/停止、剪贴板自动写入转写结果、kdialog 通知反馈、systemd 用户服务集成

### macOS 原生听写
专为 macOS 设计的原生听写/语音输入应用，多基于 Swift + whisper.cpp / WhisperKit / Parakeet，支持全局热键、菜单栏、Core ML / Neural Engine 加速。
- **[OpenSuperWhisper](https://github.com/Starmel/OpenSuperWhisper)** ⭐1474 · MIT · Swift (主), Shell, CMake, C, Ruby · macOS · 中文 是
  macOS 实时语音转录应用，支持 Whisper 与 Parakeet 双引擎，提供全局快捷键、按住录音、拖拽文件队列转录、麦克风选择和多语言自动检测。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(主要语言 Swift（约 402KB）并包含 whisper.cpp C/C++ 代码与 Rust autocorrect 子模块；本地构建需要 Xcode、c…) | 活跃度:active(2026-06-24)
  - 核心特性:实时音频转录、Whisper + Parakeet 双引擎、全局快捷键/按住录音、拖拽文件批量转录、多语言自动检测与亚洲语言自动校正
  - ⚠️ 注意:仅支持 macOS Apple Silicon/ARM64; Intel Mac 兼容性仍在 TODO 中; 本地构建依赖 Xcode 与多个工具链，对非 macOS 开发者不友好。
- **[Pindrop](https://github.com/watzon/pindrop)** ⭐546 · MIT · Swift/SwiftUI, Xcode, SwiftPM, WhisperKit, SwiftData, Sparkle · macOS · 中文 否
  A native macOS menu-bar dictation app that converts speech to text locally using OpenAI Whisper via WhisperKit (Core ML optimized for Apple Silicon). It runs fully offline for transcription, supports…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️ | 活跃度:active(2026-04-21)
  - 核心特性:100% local, offline speech-to-text via WhisperKit、Multiple transcription engines (WhisperKit, Parakeet) and streaming support、Global hotkeys (toggle / push-to-talk)、Transcription history with search and export (JSON/CSV/text)、Notes system with pinning, tagging, and AI-generated titles
  - ⚠️ 注意:macOS 14.0+ only and Apple Silicon (M1/M2/M3/M4) recommended; requires Xcode + Apple toolchain to build from source. Model downloads range from ~75 MB (Tiny) to ~3 GB (Large). Optional AI enhancement requires an external API key. UI language currently English only.
- **[whisper-dictation](https://github.com/foges/whisper-dictation)** ⭐219 · MIT · Python · macOS/Linux (partial) · 中文 部分
  离线运行的多语言语音听写工具：基于 OpenAI Whisper ASR 模型，通过全局快捷键触发录音，并将识别结果自动键入当前输入框。支持自选模型尺寸/语言、自定义快捷键组合，并在 macOS 菜单栏显示状态。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:maintenance(2024-07-20)
  - 核心特性:offline speech-to-text with OpenAI Whisper、global hotkey trigger (configurable)、menu bar status icon (macOS)、multiple Whisper model sizes、multilingual transcription
  - ⚠️ 注意:macOS-centric: uses `rumps` for the menu bar, so out-of-the-box Linux/Windows support is limited and may require porting. Requires PortAudio and LLVM system libraries. Larger Whisper models (small/medium/large) need a strong CPU or CUDA GPU for comfortable real-time transcription. Last commit/push was 2024-07-20, so active development appears paused.
- **[FnKey](https://github.com/evoleinik/fnkey)** ⭐45 · GPL-3.0 · Rust · macOS · 中文 否
  Hold the Fn key, speak, and have the transcribed text pasted into the active input. A tiny Rust macOS menu-bar app that streams audio to Deepgram Nova-3 (or falls back to Groq Whisper) while the Fn…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2026-03-23)
  - 核心特性:Hold Fn to record、Deepgram streaming transcription、Groq Whisper fallback、macOS menu-bar UI、Custom keyword vocabulary
  - ⚠️ 注意:macOS only; core transcription relies on external cloud APIs (Deepgram, Groq); no local/offline ASR; limited extensibility beyond keyword hints and backend key selection.
- **[hush](https://github.com/djmunro/hush)** ⭐6 · MIT · Rust；核心依赖 cpal（音频）、parakeet-rs（Whisper ONNX 推理）、deno_core（自定义 JS 解析器）、objc2 系列（AppKit/CoreFoundation/CoreGraphics 绑定）；构建脚本为 Bash/Swift · macOS · 中文 否
  macOS 本地按键即发即说（push-to-talk）听写工具。按住快捷键（默认 fn）说话，松开后使用本地 Whisper/Parakeet ONNX 模型实时转写，并自动粘贴到光标处。无云端、无始终监听麦克风，适合注重隐私与低延迟的 macOS 用户。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(单一 Rust 二进制，Cargo 依赖数量有限（cpal、parakeet-rs、deno_core、serde、toml、objc2 家族），无需 GPU，…) | 活跃度:active(2026-06-10)
  - 核心特性:按住 fn（可自定义）即说即写、本地 Whisper/Parakeet ONNX 转写，不上云、无持续监听，仅在按键期间采集音频、转写结果通过 CGEventPost 粘贴到光标处、浮动 pill 展示实时音量与转写动画
  - ⚠️ 注意:仅支持 macOS; 预构建二进制为 ad-hoc 签名，首次启动可能触发 Gatekeeper; 需要授予麦克风和辅助功能权限; 模型缓存约 100MB–2GB; 自定义脚本跑在 Deno 沙箱中，出错会回退到原始文本; 无 Windows/Linux/移动端版本。
- **[WhisperDictation](https://github.com/sam-pop/WhisperDictation)** ⭐1 · MIT · Swift, C/C++ (whisper.cpp submodule) · macOS · 中文 否
  A free, open-source, 100% offline macOS dictation app powered by OpenAI Whisper via whisper.cpp. It captures microphone audio, transcribes speech locally using Metal GPU acceleration (Apple Silicon)…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2026-04-13)
  - 核心特性:100% offline, local speech-to-text、Push-to-talk or toggle-mode global hotkey、Text injection at cursor in any app、Whisper.cpp with Metal GPU acceleration、Multiple Whisper models (Base/Small/Medium, full and quantized)
  - ⚠️ 注意:Only macOS 14+ is supported (no Windows, Linux, or mobile). Not notarized by Apple, so first launch requires manual security override. Whisper models can be up to 1.5 GB and are downloaded on demand. English-only at this time; Chinese is not yet supported.
- **[whisper-dictation](https://github.com/ashwin-pc/whisper-dictation)** ⭐25 · MIT · Python · Mac · 中文 否
  macOS 菜单栏应用：按下 Globe/Fn 键录音，松开后用本地 faster-whisper 转写并粘贴到光标处。新增可选 AWS Bedrock(Claude) 语音指令改写选中文本。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(纯 Python 项目，依赖仅 requirements.txt 中 9 个包；无需 GPU，录音/热键/菜单栏均用轻量库实现。但 faster-whisper…) | 活跃度:active(2026-03-15)
  - ⚠️ 注意:仅支持 macOS; 核心功能完全离线，但 AI 文本增强需要 AWS Bedrock（Claude）联网并配置 AWS 凭证; 中文界面未提及，转写能力取决于 faster-whisper 模型本身支持中文。

### AI 语音清理 / LLM 后处理型听写
在语音识别后接入本地或云端 LLM 进行润色、格式化、摘要、风格调整的听写工具，适合需要“说大白话，出规范文本”的工作流。
- **[typewhisper-mac](https://github.com/TypeWhisper/typewhisper-mac)** ⭐1541 · GPL-3.0 · Swift · Mac · 中文 否
  TypeWhisper for Mac is a macOS dictation and speech-to-text app that transcribes audio using on-device AI models or optional cloud APIs (Groq, OpenAI, xAI/Grok), then transforms results with reusable…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-30)
  - 核心特性:On-device STT with WhisperKit/MLX-based engines、Cloud STT via Groq/OpenAI/xAI/Grok、System-wide dictation with global hotkeys、Reusable AI transformation workflows、Plugin SDK and registry
  - ⚠️ 注意:macOS 14.0+ only; local larger models need 16 GB+ RAM; optional cloud APIs require provider API keys; commercial licensing is offered as a dual-licensing option.
- **[Amical](https://github.com/amicalhq/amical)** ⭐1388 · MIT · TypeScript / Electron / Next.js / React · Windows/macOS/Linux/Web/Android/iOS · 中文 否
  本地优先的 AI 语音转写/听写应用（Electron 桌面端 + Next.js 文档站）。基于 OpenAI Whisper 做本地语音转文字，结合 Ollama 等开源 LLM 做上下文感知格式化和智能笔记处理，支持离线运行。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Electron 桌面应用，Turborepo 管理；desktop 包依赖 80+ 个运行时库（React 19、Next.js、Lexical、Radix、…) | 活跃度:active(2026-06-30)
  - ⚠️ 注意:Electron 桌面应用较重，本地模型推理需要一定硬件资源; README 中 MCP 集成、实时会议转写等功能标记为 In Progress/Planned; 源码中仍包含 PostHog 等遥测依赖。
- **[VoiceTypr](https://github.com/moinulmoin/voicetypr)** ⭐389 · AGPL-3.0 · Rust + Tauri (backend), TypeScript/React + Vite (frontend), Whisper (local STT) · macOS/Windows · 中文 部分
  AI-powered offline voice-to-text dictation tool for macOS and Windows; system-wide hotkey records speech, inserts transcription at cursor, with optional cloud AI enhancement (Groq/Gemini).
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-30)
  - 核心特性:Offline local Whisper transcription、System-wide recording hotkey with auto text insertion、99+ language support、Hardware acceleration (Metal/OpenMP, GPU fallback CPU)、AI enhancement presets via Groq/Gemini
  - ⚠️ 注意:macOS 14+ required; Windows GPU acceleration needs up-to-date drivers; no Linux or mobile builds; 3-4 GB disk space required for models; license/trial check phones home (functionality not blocked but noted); UI/documentation only in English.
- **[HoldSpeak](https://github.com/karolswdev/HoldSpeak)** ⭐277 · Apache-2.0 · Python 3.10+（核心/插件/连接器）; FastAPI + Uvicorn（本地 Web 运行时）; Astro（Web UI）; Swift（Apple 伴侣应用）; SQLite（本地数据）; 可选 mlx-whisper/faster-whisper/openwakeword/llama-cpp-python · macOS/Linux/Web · 中文 部分
  HoldSpeak 是面向 macOS 与 Linux 的本地优先语音助手，支持“按住说话”式全局语音输入（可在任意应用内打字）以及会议录音/导入转写，并通过插件化流水线从会议记录中自动抽取决策、行动项、风险登记等结构化产物。Whisper 在本地运行，LLM 可选本地模型（GGUF/MLX）或任意 OpenAI 兼容端点，数据不离开本机。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(核心是纯 Python 应用，可通过 pip/uv 安装；核心依赖为常见库（FastAPI、sounddevice、numpy、PyYAML 等），无 GPU …) | 活跃度:active(2026-06-30)
  - 核心特性:任意应用全局语音输入与跨应用打字、本地 Whisper 语音识别（99 种语言）、会议录音/导入与说话人分离、插件化会议智能流水线（14+ 内置插件）、决策/行动项/风险登记/ADR 等结构化产物
  - ⚠️ 注意:项目尚处 0.x（v0.3.1），API、配置与默认值仍可能变化; 无 Windows 正式支持; Linux Wayland 下全局热键与跨应用输入为 best-effort; 部分 AI 能力需单独安装可选 extras（mlx/faster-whisper/llama-cpp 等）; 桌面吉祥物 Qlippy 与 iPad/AIPI-Lite 伴侣功能均为可选组件。
- **[QuickDictate](https://github.com/kristian-dott-42/QuickDictate)** ⭐1 · MIT · Swift · macOS · 中文 否
  macOS 上的 push-to-talk 轻量听写应用：按住 fn 说话，松开后通过 Whisper 将语音转写为文本，再经 LLM 清理格式/标点，最后模拟 ⌘V 粘贴到当前光标处。可作为 Wispr Flow 的免费本地替代方案。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-25)
  - ⚠️ 注意:仅支持 macOS 13+，非跨平台; README 与界面为英文，无中文本地化; 未提供正式插件/API 框架，扩展需通过修改源码或环境变量实现; 依赖网络 API 进行转写与清理，离线使用需自行部署 Whisper 与 LLM。
- **[Voicisst](https://github.com/lucyfromnaarm/voicisst)** ⭐0 · MIT · 未知 · Linux/macOS/Windows/Web · 中文 部分
  本地 AI 语音听写/转写工具。支持按住说话/切换模式，先用本地 Whisper 做语音识别，再通过本地/私有 LLM（默认 Ollama qwen3.5:4b）润色：去除填充词、修正自我重复、把口语列表转成 Markdown、自动标点、个人词典纠正。可在任意应用内输入，也支持文件转写；提供 all-in-one 与 client/server 分离两种架构。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Python 3.10+ 纯依赖安装（pipx/uv），但默认使用 Whisper large-v3-turbo + qwen3.5:4b，官方建议约 8GB …) | 活跃度:active(2026-06-25)
  - 核心特性:Whisper 本地语音识别（faster-whisper）、LLM 润色/后处理（Ollama/OpenAI-compatible）、按键说话/切换、自动静音停止、个人词典与选中文本词汇增强、实时打字流式输出与浏览器仪表盘
  - ⚠️ 注意:仓库较新（stars 0，2026-06-25 最后更新），默认模型对 GPU 和显存要求较高; 中文仅依赖 Whisper 多语言能力和 LLM 保持语言，文档与界面主要为英文。
- **[VoiceFlow](https://github.com/infiniV/VoiceFlow)** ⭐393 · MIT · Python (PySide6/Pyloid backend), React + Vite + Tailwind v4 frontend, faster-whisper/CTranslate2 inference, SQLite storage · Windows/Linux · 中文 部分
  本地语音听写与会议录制工具。按住全局热键说话，释放后将 faster-whisper 转录文本自动输入到光标处；会议模式可同时录制麦克风和系统音频，并调用用户自选的 OpenAI/Groq/OpenRouter/Ollama 等 LLM 生成总结。音频与转写本地处理，无需账号、无 telemetry、离线可用。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2026-06-21)
  - 核心特性:全局热键听写、faster-whisper 本地转录、16+ 可选 Whisper 模型、CPU/GPU 自动切换、会议模式：麦克风+系统音频双轨录制
  - ⚠️ 注意:macOS 仅可构建但官方未支持; 前端依赖 PySide6/Qt WebEngine 导致安装包较大; Whisper 大模型需要数 GB 磁盘/内存; 目前无正式插件 API，扩展需修改源码。
- **[VoiceInk](https://github.com/Beingpax/VoiceInk)** ⭐5387 · GPL-3.0 · Swift, whisper.cpp · macOS · 中文 部分
  Native macOS voice-to-text application that transcribes speech to text almost instantly using local AI models (whisper.cpp). Positioned as an open-source alternative to Superwhisper & Wispr Flow,…
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2026-06-28)
  - 核心特性:Local AI transcription via whisper.cpp、100% offline privacy-first processing、Context-aware modes per app/URL、Global keyboard shortcuts / push-to-talk、Personal dictionary and text replacements
  - ⚠️ 注意:Although the source is GPL v3 and free to build, the author sells a commercial binary that includes automatic updates and priority support. Platform is strictly macOS 14.4+; no Windows/Linux/Web/mobile versions. Chinese UI is partially present in Localizable.xcstrings (zh-Hans), but documentation is English-only.
- **[FluidVoice](https://github.com/altic-dev/FluidVoice)** ⭐5013 · GPL-3.0 · Swift · macOS · 中文 部分
  Open-source macOS voice-to-text dictation app with on-device speech recognition and optional local/cloud AI enhancement for formatting, capitalization, and post-processing.
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(Requires macOS 15 (Sequoia), Xcode to build, ~1 GB voice model, ~3.5 GB optional…) | 活跃度:active(2026-06-30)
  - 核心特性:On-device STT with multiple models (Nemotron, Parakeet, Cohere, Apple Speech, Whisper)、Optional local Fluid Intelligence AI enhancement、Command Mode and Write Mode for system control and text insertion、Global hotkey, menu bar integration, live transcription overlay、Per-app configuration and adaptive themes
  - ⚠️ 注意:Fluid Intelligence, the optional on-device AI enhancement runtime, is closed-source. Most non-Whisper models require Apple Silicon and macOS 15. Windows/iOS/Linux versions are listed as coming soon.
- **[OpenWhispr](https://github.com/OpenWhispr/openwhispr)** ⭐4143 · MIT · TypeScript, React 19, Electron 41, Vite, Tailwind CSS v4, shadcn/ui, better-sqlite3, whisper.cpp, sherpa-onnx, llama.cpp · macOS/Windows/Linux · 中文 部分
  跨平台桌面语音输入与转录应用，支持全局热键语音转文字、AI 语音助手、会议实时转写与说话人分离、本地语义搜索笔记。可离线运行（Whisper / NVIDIA Parakeet），也支持云端模型 BYOK。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(基于 Electron 41 的桌面应用；构建时下载 whisper.cpp、llama-server、sherpa-onnx、Qdrant、嵌入模型、说话人分…) | 活跃度:active(2026-06-30)
  - 核心特性:全局热键语音转文字、多模型 AI 语音助手、会议实时转写与说话人分离、本地语义搜索笔记、公开 API 与 MCP server
  - ⚠️ 注意:Electron + 本地 ML 运行时使其资源占用较高; 本地模型下载与推理需要较大磁盘空间和内存; 中文 UI/文档未明确，仅通过 ASR 模型可能支持中文识别。
- **[Ghost Pepper](https://github.com/matthartman/ghost-pepper)** ⭐2800 · MIT · 未知 · macOS · 中文 部分
  macOS 菜单栏应用，利用 Apple Silicon 本地运行的 Whisper/Qwen 模型实现按住 Control 说话转文字、会议录音转录、AI 文本清理与摘要，无需联网。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(无需独立 GPU，依赖 Apple Neural Engine；但作为原生 Swift/macOS 应用，仅支持 macOS 14+ 与 Apple Silic…) | 活跃度:active(2026-05-20)
  - 核心特性:按住 Control 说话，松开后自动转录并粘贴、会议录音转录并生成 AI 摘要 Markdown、100% 本地处理，核心功能无云 API、可编辑清理提示词，支持自定义常用词纠错、菜单栏应用、全局热键、开机自启
- **[Voquill](https://github.com/voquill/voquill)** ⭐977 · AGPL-3.0 (with enterprise-directory exception) · TypeScript, Rust (Tauri), React, Vite, Zustand, Astro, Firebase Functions, SQLite, Whisper/Groq · macOS/Windows/Linux/Web (marketing site)/iOS/Android · 中文 否
  Open-source, cross-platform AI voice typing app. It lets users dictate into any desktop application, clean transcripts with AI, maintain a personal glossary, and chat with a voice-powered assistant.…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(It is a pnpm monorepo containing a Tauri/Rust desktop app, marketing site, Fireb…) | 活跃度:active(2026-06-05)
  - 核心特性:Voice input overlay and system-wide hotkeys、Local Whisper transcription with optional GPU acceleration、Cloud transcription/cleanup providers (e.g., Groq)、AI transcript cleanup and writing-style switching、Personal dictionary and replacement rules
  - ⚠️ 注意:AGPLv3 covers most of the repository, but code in the `enterprise/` directory is governed by a separate Voquill enterprise license, so it is open-core rather than fully open. Building requires Node.js, Rust, Tauri CLI, and platform-native dependencies; GPU builds need the Vulkan SDK. Some features rely on Firebase/Groq cloud services.
- **[Tambourine Voice](https://github.com/kstonekuan/tambourine-voice)** ⭐366 · AGPL-3.0 · Rust (Tauri backend), TypeScript/React (Tauri frontend), Python/FastAPI (server), Pipecat (voice pipeline), WebRTC · Windows/macOS/Linux · 中文 否
  跨平台 AI 语音输入/口述助手。按下热键后，在任意应用的光标处直接输入语音转写文本，并通过 LLM 自动格式化（去填充词、加标点、按邮件/聊天/代码等上下文调整风格）。可完全本地运行（Whisper + Ollama），也可接入 Deepgram、OpenAI、Anthropic 等云端 STT/LLM。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(本地部署支持 CPU，可仅使用 Whisper/Ollama 不依赖云端；提供 Docker 与 docker-compose。但技术栈跨 Rust + Nod…) | 活跃度:active(2026-06-29)
  - 核心特性:双模式录音（按住/切换）、实时语音转文字（多 STT provider）、LLM 格式化与上下文感知输出、可自定义 prompt、个人词典、规则、应用内 provider 切换，无需重启
  - ⚠️ 注意:Linux 支持标记为 ⚠️; Android/iOS 不支持; README 声明项目仍在活跃开发，可能有破坏性变更; 未来 Hosted Service 是可选云端方案，不影响本地开源版本的完整性。
- **[OpenTypeless](https://github.com/tover0314-w/opentypeless)** ⭐308 · MIT · TypeScript, Rust, React, Tauri · Win/Mac/Linux · 中文 是
  跨平台 AI 语音输入桌面应用，支持在任意应用内通过热键语音打字、AI 改写/润色、选中文字重写，以及一键语音问答。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2026-06-30)
  - 核心特性:全局热键语音打字、AI 润色/改写/翻译、选中文字语音指令重写、Ask Anything 一键语音问答、多 STT/LLM provider 选择（BYOK 或本地）
  - ⚠️ 注意:提供可选的付费 managed cloud words（Pro/Lifetime）云服务; 如需完全本地、无云端增值，请在设置中选择非 Cloud 的 STT/LLM provider 并关闭 Cloud 相关功能。
- **[Aria](https://github.com/Xingxun7777/Aria)** ⭐71 · Apache-2.0 · Python 3.12 + PyTorch (CUDA 12.8) + PySide6 · Windows · 中文 是
  Windows 本地 AI 语音输入法，基于 Qwen3-ASR / FunASR 离线语音识别，支持屏幕 OCR 感知上下文、热词纠错、三档润色风格、语音唤醒词、语音指令操作选区（翻译/润色/总结/扩写等），并提供便携免安装版本。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(安装包 ~2 GB（精简版）至 ~6 GB（完整版），ASR 模型体积大；依赖 PyTorch cu128、transformers、PySide6、FunAS…) | 活跃度:active(2026-06-10)
  - 核心特性:离线语音识别 (Qwen3-ASR/FunASR/Whisper)、屏幕感知 OCR 上下文、热词纠错与 AI 润色、语音指令操作选区、三档收音/润色风格
  - ⚠️ 注意:Windows 10/11 独占（依赖 pywin32 / uiautomation / winocr），不跨平台; 模型体积与 AI 推理资源需求高; 仓库仅 1 位贡献者; 屏幕感知增强与 AI 润色需联网调用第三方 LLM API，非纯离线。
- **[OpenFlow](https://github.com/SadmanMahi67/OpenFlow)** ⭐15 · MIT · Electron + React + TypeScript，使用 whisper.cpp/llama.cpp 原生运行时 · Windows · 中文 否
  OpenFlow 是 Windows 桌面语音听写应用：按住 Ctrl+Win 录音，使用本地 whisper.cpp 离线转写，可选 Groq 云端或本地 llama.cpp 做 AI refinement（Casual/Formal/Summarised/Bullet Points/Email Ready 等风格），并将文本自动粘贴到当前活动窗口。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(Electron + React + TypeScript 桌面应用；运行时需额外下载多 GB 的 Whisper 模型并附带 whisper.cpp/llis…) | 活跃度:active(2026-05-28)
  - 核心特性:全局 Ctrl+Win 按住说话、whisper.cpp 离线转写，支持 CPU/Vulkan 加速、AI refinement（Groq 云端 / llama.cpp 本地）、多种精炼风格：Casual/Formal/Summarised/Bullet Points/Email Ready、自定义 Prompt 过滤器与用户词汇表
  - ⚠️ 注意:仅支持 Windows 10/11 x64; Whisper 模型需自行下载、体积不小; AI 云端精炼依赖 Groq API key; 本地 AI 精炼需要自备 llama.cpp 模型。
- **[localflow](https://github.com/sidharth-n/localflow)** ⭐0 · Apache-2.0 · Python · Linux · 中文 部分
  Fully-local, cross-platform AI voice dictation. Hold a hotkey, speak, and polished text is injected at the cursor via STT (Moonshine) and a local polish LLM (Qwen3-4B). Runs entirely on-device with…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-04-22)
  - 核心特性:On-device STT using Moonshine、Local polish LLM using Qwen3-4B-Instruct-2507 GGUF、Heuristic skip-gate to bypass LLM for already-clean text、Push-to-talk hotkey with waveform overlay、One-command setup via setup.sh
  - ⚠️ 注意:Early-alpha stage with breaking changes possible. Linux X11 only right now; Wayland and macOS ports are planned but not yet complete. GPU polish recommended for good latency; CPU fallback raises polish latency to 2–5 s. No formal plugin API yet.
- **[yammer](https://github.com/andynu/yammer)** ⭐0 · MIT · Rust, Tauri (JS/TS frontend), Node.js · Linux · 中文 否
  Local speech-to-text with LLM correction for Linux. Captures microphone audio with voice-activity detection, transcribes via local Whisper, cleans up the text with a local LLM, and types the result…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Rust + Tauri native binary; CPU inference works, CUDA is optional; first compile…) | 活跃度:active(2026-02-24)
  - 核心特性:Voice Activity Detection、Local Whisper speech-to-text、Local LLM text cleanup、Tauri floating overlay UI、Universal input injection via xdotool
  - ⚠️ 注意:X11 only; Wayland is not supported. First build is slow because it compiles whisper.cpp and llama.cpp. Needs ~2 GB of model downloads. Only Linux is supported. Repository has 0 stars, indicating a very early/niche project.

### 本地/离线 STT 引擎与工具包
可供上层应用集成的离线 ASR 引擎与全链路语音工具包，包括 Whisper 推理库、next-gen Kaldi/ONNX 工具包、Vosk，以及面向中文的 FunASR / PaddleSpeech / SenseVoice 等。
- **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)** ⭐51163 · MIT · C/C++（核心），CMake 构建，提供 Python/Java/Objective-C/C# 等绑定 · Mac/iOS/Android/Linux/Windows/Web（通过 WASM 构建） · 中文 部分
  OpenAI Whisper 自动语音识别（ASR）模型的高性能 C/C++ 移植实现，支持纯 CPU、量化及多种 GPU（Metal/CUDA/Vulkan/ROCm/OpenVINO/Ascend 等）加速推理，可作为实时语音转文字引擎嵌入其他应用。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-30)
  - 核心特性:纯 C/C++ 实现，无 Python 运行时依赖、CPU 即可运行，支持 INT8/量化、支持 Metal/CUDA/Vulkan/ROCm/OpenVINO/Ascend 等多后端 GPU 加速、零运行时内存分配、C 风格 API 与多语言绑定
  - ⚠️ 注意:模型权重需额外下载（OpenAI 提供的 Whisper 模型 / ggml 格式），本体代码无网络依赖; 中文 ASR 依赖模型固有能力，项目文档主要为英文。
- **[FunASR](https://github.com/modelscope/FunASR)** ⭐18745 · MIT · Python (PyTorch) · Linux/Mac/Windows/Web/Android/iOS · 中文 是
  阿里达摩院/魔搭社区开源的工业级端到端语音识别工具包，提供 Paraformer、SenseVoice、Fun-ASR-Nano 等模型，支持自动语音识别（ASR）、语音活动检测（VAD）、说话人分离、情绪识别、实时流式识别、字幕生成，并可通过 OpenAI 兼容 API 或 WebSocket/gRPC/HTTP 服务化部署。
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(支持纯 CPU 运行（SenseVoice 号称 17x 实时），GPU 仅用于旗舰模型；安装为标准 pip install funasr，依赖为常见 PyTo…) | 活跃度:active(2026-06-30)
  - 核心特性:工业级 ASR（Paraformer/SenseVoice/Fun-ASR-Nano）、原生中文优化及多语言支持（50+ 语言）、VAD + 说话人分离 + 情绪识别一体化、实时流式识别（WebSocket/HTTP）、OpenAI 兼容 API 服务端
  - ⚠️ 注意:旗舰 Fun-ASR-Nano 等 LLM-ASR 模型推荐 GPU 以获得标称 340x 实时性能; CPU 可跑但速度随模型尺寸下降。整体依赖较重（PyTorch/transformers/librosa 等），在低配或仅 CPU 设备上首次下载模型和安装体积较大。官方文档和示例中文丰富，但部分高级部署/调优文档以中文为主。
- **[vosk-api](https://github.com/alphacep/vosk-api)** ⭐14889 · Apache-2.0 · C++ core with bindings for Python, Java, C#, Node.js, Rust, Go, etc. · Windows/Mac/Linux/Web/Android/iOS · 中文 是
  Offline speech recognition toolkit providing small, CPU-only ASR models for 20+ languages with bindings for Python, Java, C#, Node.js, C++, Rust, Go and others.
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-04)
  - 核心特性:Offline ASR、20+ languages and dialects、Small models (~50 MB to hundreds MB)、CPU real-time recognition、Streaming API
  - ⚠️ 注意:Core engine and open models are fully open source; Alphacep also offers optional commercial support/hosted services, but the repository itself is not open-core and does not gate features behind a cloud tier.
- **[sherpa-onnx](https://github.com/k2-fsa/sherpa-onnx)** ⭐13280 · Apache-2.0 · C++, C, Python, Go, C#, Java, Kotlin, JavaScript, Swift, Rust, Dart, Pascal; CMake · Android/iOS/Windows/macOS/Linux/HarmonyOS/WebAssembly/WearOS/Raspberry Pi/RISC-V/NPU (RK/QNN/Ascend/Axera) · 中文 是
  基于 next-gen Kaldi 与 ONNX Runtime 的全离线语音处理工具包，支持 STT、TTS、说话人分割/识别/验证、语种识别、音频标签、VAD、语音增强、关键词唤醒、声源分离等，无需联网即可在本地运行。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(纯 CPU 可运行，GPU 仅为可选；ONNX Runtime 作为核心推理引擎，提供预编译 wheel、Android APK、WebAssembly 等产物…) | 活跃度:active(2026-06-30)
  - 核心特性:离线语音识别（流式/非流式 ASR）、离线文本转语音（TTS）、说话人分割、识别与验证、 spoken language identification、音频标签（Audio tagging）
  - ⚠️ 注意:预训练模型文件通常较大; 从源码完整构建需要 CMake 与 C++ 工具链，耗时较长; NPU/GPU 支持为可选组件，需要对应 SDK。
- **[PaddleSpeech](https://github.com/PaddlePaddle/PaddleSpeech)** ⭐12636 · Apache-2.0 · Python, C++ · Linux/Windows/Mac/Web/Android/ARM Linux · 中文 是
  百度飞桨官方语音工具套件，提供 ASR、TTS、声纹识别、说话人分割、标点恢复、语音翻译、关键词检测、音频分类等全链路语音能力，支持 CLI、Server 与流式服务。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(依赖 PaddlePaddle 深度学习框架、librosa、onnxruntime、scipy、h5py 等众多库；需要 GCC>=4.8.5 和 Pytho…) | 活跃度:active(2026-06-21)
  - ⚠️ 注意:适合需要中文语音能力的工程与研究场景，但安装体量大、依赖重，不建议在极简环境或嵌入式边缘设备上直接部署完整版。
- **[SenseVoice](https://github.com/FunAudioLLM/SenseVoice)** ⭐8731 · MIT（通过引用 FunASR 的 MIT 许可证；GitHub API 自身显示 NOASSERTION） · Python（核心推理/服务），C/C++（runtime/llama.cpp），依赖 PyTorch、funasr、modelscope、gradio、fastapi、torchaudio 等 · Linux/Windows/Mac/Web/Android/iOS · 中文 是
  阿里通义实验室开源的多语言语音理解基础模型，支持自动语音识别（ASR）、 spoken language identification、语音情感识别（SER）和音频事件检测（AED）。SenseVoice-Small 采用非自回归端到端架构，对中文/粤语 ASR 表现优异，推理延迟远低于 Whisper；同时提供微调脚本、服务化部署（FastAPI/WebUI）以及…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-29)
  - 核心特性:多语言 ASR（50+ 语言，中文/粤语领先）、语音情感识别（SER）与音频事件检测（AED）、非自回归端到端，SenseVoice-Small 推理比 Whisper-Large 快约 15 倍、官方提供 FastAPI 服务、WebUI、Docker 镜像、支持微调（finetune）与长音频 VAD 切分
  - ⚠️ 注意:模型权重需要从 ModelScope/HuggingFace 下载; 原始 PyTorch 版本对 GPU 更友好，但 q8 GGUF CPU 二进制已可用。

### 系统级语音输入 / IME
以输入法、IBus/Fcitx 扩展、Android IME/RecognitionService、iOS 键盘等形式深入系统输入层的语音输入方案。
- **[Whisper IME](https://github.com/woheller69/whisperIME)** ⭐603 · MIT · Java, Android, TensorFlow Lite · Android · 中文 部分
  Android Input Method Editor (IME) and system-wide voice input (RecognitionService) based on OpenAI Whisper. Provides offline speech recognition, translation to English, and can be activated as a…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-02-07)
  - 核心特性:Offline Whisper-based speech recognition on Android、Input Method Editor (IME) integration、System-wide voice input (RecognitionService)、RecognizerIntent support、English-to-English translation mode
  - ⚠️ 注意:First launch requires internet to download ~435 MB TFLite models from HuggingFace. Future availability on certified Android devices is uncertain due to Google's 2026/2027 identity disclosure policy for app developers.
- **[Vocalinux](https://github.com/jatinkrmalik/vocalinux)** ⭐404 · GPL-3.0 · Python 3.9+, GTK (PyGObject), whisper.cpp, OpenAI Whisper, VOSK, ONNX Runtime (optional), shell installer · Linux · 中文 否
  A free, GPLv3 Linux desktop voice dictation app that inserts spoken text into any X11 or Wayland application using fully offline speech recognition (whisper.cpp / OpenAI Whisper / VOSK) with optional…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-07-01)
  - 核心特性:Offline voice-to-text dictation across all Linux apps、Three swappable SR engines: whisper.cpp (default), OpenAI Whisper, VOSK、Optional Vulkan GPU acceleration and Silero VAD (ONNX Runtime)、X11 and Wayland support via text injection + IBus、Toggle / push-to-talk activation with customizable keyboard shortcuts
  - ⚠️ 注意:Optional OpenAI Whisper path pulls PyTorch + CUDA and is heavier/beta; Linux-only (X11/Wayland); remote API feature is optional and user-supplied.
- **[blurt](https://github.com/QuantiusBenignus/blurt)** ⭐107 · GPL-3.0 · JavaScript, Shell (zsh/bash), CSS · Linux · 中文 部分
  GNOME Shell 扩展，按住自定义热键即可在任意文本框进行离线语音输入。通过调用 whisper.cpp（本地 CLI、whisper.cpp server 或 whisperfile）将语音转写成文本，并写入 PRIMARY 选择区/剪贴板，支持 X11 与 Wayland。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(主体为少量 JavaScript 扩展文件与一个 zsh 脚本（wsi）；不捆绑 heavy 运行时；依赖仅为 GNOME Shell、sox、curl、xse…) | 活跃度:active(2026-05-07)
  - 核心特性:系统级热键触发离线语音输入、支持本地 whisper.cpp、whisper.cpp server 与 whisperfile 三种推理后端、GNOME 顶栏状态指示灯（颜色显示录音/识别状态）、可配置快捷键与偏好设置、识别结果写入 PRIMARY 选择区或剪贴板，兼容 X11/Wayland
  - ⚠️ 注意:仅适用于 GNOME Shell 的 Linux 桌面; 首次使用需要手动安装 whisper.cpp 或下载 whisperfile、配置模型路径及系统依赖; 界面与文档为英文，中文支持依赖底层 whisper 模型; 扩展性主要依赖修改脚本而非插件体系。
- **[Vosk Android Service](https://github.com/alphacep/vosk-android-service)** ⭐64 · Apache-2.0 · Java, Android SDK (compileSdk 33/minSdk 24), Gradle 7.2.2, Vosk Android AAR 0.3.46, JNA, RxJava2, Retrofit, Gson · Android · 中文 部分
  一个 Android 后台语音识别服务，封装了开源的 Vosk ASR 引擎，让其他 Android 应用可以通过标准的 android.speech.RecognitionService 接口调用离线语音转文字。包含模型下载、模型选择 UI 和识别服务本身，可直接作为系统级语音输入法/语音助手的后端。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:maintenance(2023-03-25)
  - 核心特性:基于 Vosk 的离线 ASR，无需联网即可识别、暴露标准 Android RecognitionService，可被任意输入法或 App 调用、内置模型下载与选择 UI、CPU 推理，无需 GPU、支持 armeabi-v7a/arm64-v8a/x86/x86_64 ABI
  - ⚠️ 注意:仓库活跃度低：最后 commit 为 2023-03-25，release 停留在 2022-06，多个 open issue 未处理; UI 只有英文，无中文界面; 需要用户自行构建/侧载; 模型下载源依赖外部服务器; 仅限 Android 平台。
- **[Dictus](https://github.com/getdictus/dictus-ios)** ⭐12 · MIT · Swift 5.9+, SwiftUI, WhisperKit (Swift Package Manager), Apple CoreML, Xcode 16+ · iOS · 中文 否
  Free, open-source iOS keyboard for on-device voice dictation. Uses WhisperKit (Apple CoreML) to transcribe speech locally, works system-wide in any app, supports AZERTY/QWERTY/QWWERTZ layouts and…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-19)
  - 核心特性:On-device voice transcription via WhisperKit/CoreML、System-wide custom iOS keyboard、AZERTY/QWERTY/QWERTZ layouts、Multiple Whisper model sizes (tiny/base/small)、100% offline, no account or subscription for core features
  - ⚠️ 注意:Future roadmap includes 'Smart Mode Pro' (on-device LLM reformulation), which could introduce a premium tier; core STT features remain free and open source. Build ecosystem is locked to macOS + Xcode 16+ and iPhone 12+/iOS 17+.
- **[voice-typing-linux](https://github.com/GitJuhb/voice-typing-linux)** ⭐11 · MIT · Python · Linux · 中文 否
  Linux speech-to-text input method engine using IBus, with streaming STT (NVIDIA Riva ASR NIM / Parakeet CTC / Moonshine / zipformer) and optional Whisper/Parakeet post-commit correction. Works on…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(Pure Python and pip-installable, but depends on heavy ML libraries (torch, trans…) | 活跃度:active(2026-05-01)
  - 核心特性:IBus input method engine、streaming STT with multiple backends、optional Whisper/Parakeet refinement、optional CUDA GPU acceleration、voice commands

### 中文语音输入 / 输入法
针对中文识别、中文输入法框架或中文用户场景优化的项目，包含基于 FunASR/Paraformer/SenseVoice 的中文 IME 与键盘。
- **[VocoType-linux](https://github.com/LeonardNJU/VocoType-linux)** ⭐163 · GPL-3.0 · Python（核心引擎、IBus 引擎），C++（Fcitx5 addon），Shell（安装脚本） · Linux · 中文 是
  Linux 离线中文语音输入法，基于 FunASR Paraformer，支持 IBus/Fcitx5 框架，实现 ~0.1s 语音上屏、长句润色、语音编辑，无需联网与 GPU。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-04-06)
  - 核心特性:100% 离线 ASR（FunASR Paraformer，CPU Only）、同时支持 IBus / Fcitx5 输入法框架、PTT 按键说话（F9）与长句润色（Shift+F9）、本地 SLM 与 OpenAI 兼容远程 SLM 双模式后处理、IBus 语音编辑（Ctrl+F9：改写/插入/删除/导航/撤销）
  - ⚠️ 注意:仅支持 Linux; 需要 Python 3.11-3.12; 运行时识别阶段约占用 700MB 内存; 模型文件需额外下载且体积较大; Fcitx5 版本目前未提供与 IBus 同等的语音编辑能力; 启用本地 SLM 需额外安装 torch/transformers。
- **[voice-input-method](https://github.com/pofice/voice-input-method)** ⭐38 · GPL-3.0-or-later · Python 3.10+ · Linux/Windows/macOS · 中文 是
  基于 FunASR + PySide6 的低延迟中文离线语音输入法，支持长按/Toggle 录音、文本后处理（热词、纠错、繁简转换）与跨平台自动粘贴。提供 GUI 与 headless CLI 两种使用方式，可被 AI agent 脚本化调用。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-04-22)
  - 核心特性:离线语音识别（默认 FunASR ONNX，~370MB 自动下载）、5 种可切换 ASR 后端：funasr / sherpa-sensevoice / sensevoice-lm / sherpa-nano / qwen3-asr、GUI 与 CLI 双入口，CLI 完全 headless、跨平台输入后端：Linux X11/Wayland、Windows、macOS、热词与纠错规则热重载
  - ⚠️ 注意:默认模型约 370MB，部分可选后端（sherpa-nano ~800MB、qwen3-asr ~500MB）需要手动下载模型; 当前 Star 数仅 38，社区规模尚小; README 显示最后一次更新在 2026-04-22，近两个半月未推新 commit，活跃度属于“可维护”而非高频迭代。
- **[BiBi-Keyboard](https://github.com/BryceWG/BiBi-Keyboard)** ⭐695 · Apache-2.0 · Kotlin 2.2.20 / Android SDK 36 / Compose / Gradle · Android · 中文 是
  基于 Kotlin 的 Android 智能语音输入法键盘应用，集成 ASR（语音识别）与 LLM 文本后处理，支持 11 种 ASR 引擎（7 云端 + 4 本地）、悬浮球跨输入法语音输入、AI 编辑面板、Material3 界面与多语言。
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(Kotlin Android 项目，依赖 AndroidX、Compose、OkHttp、sherpa-onnx 本地 ASR AAR、DashScope SD…) | 活跃度:active(2026-06-18)
  - 核心特性:长按录音与智能判停、11 种 ASR 引擎（云端+本地）、LLM 识别后处理、悬浮球跨输入法语音输入、AI 编辑面板
  - ⚠️ 注意:采用 open-core 模式：主体 Apache-2.0 开源，但 Pro 高级功能以付费应用形式在 Google Play 上架; README 中的文档部分依赖 Notion/外部站点; 构建需要 Android 工具链与 JDK 21。

### 浏览器与 Web 语音输入
Chrome/Firefox 扩展、WebAssembly 封装、Web UI 等面向浏览器环境的语音输入方案，多数需要配合本地或云端 STT 后端。
- **[Whisper-WebUI](https://github.com/jhj0517/Whisper-WebUI)** ⭐2821 · Apache-2.0 · Python; PyTorch / torchaudio; faster-whisper; Gradio; pyannote.audio; FFmpeg · Windows/Mac/Linux/Web · 中文 部分
  基于 Gradio 的 Whisper Web 界面，支持从本地文件/YouTube/麦克风生成字幕，内置语音翻译、字幕翻译（NLLB/DeepL）、Silero VAD、BGM 分离与 pyannote 说话人分离，并提供 /backend REST API。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Python 项目但依赖 PyTorch、torchaudio、faster-whisper、pyannote.audio 等大型库；Docker 镜像约 7G…) | 活跃度:active(2025-12-29)
  - 核心特性:本地文件/YouTube/麦克风语音转字幕、支持 SRT / WebVTT / txt 输出、切换多种 Whisper 后端与自定义模型、语音到英文翻译与字幕文本翻译(NLLB/DeepL)、Silero VAD 语音检测预处理
  - ⚠️ 注意:GPU 性能直接影响体验; 说话人分离需 Hugging Face token 并接受模型条款; 默认 CUDA 12.8，Intel/AMD 用户需自行修改 requirements.txt 的 extra-index-url; 中文界面需社区 PR 完善。
- **[Vosk-STT-Chrome-Extension](https://github.com/crrrowz/Vosk-STT-Chrome-Extension)** ⭐0 · MIT · JavaScript (Chrome extension Manifest V3), Python (Vosk WebSocket server) · Web/Linux/Mac/Windows · 中文 否
  Browser extension that performs real-time speech-to-text with offline Vosk, dictating into any input field. Supports Arabic (Iraqi dialect) & English with voice commands, Arabic spoken-number…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-03-11)
  - 核心特性:Real-time speech-to-text into any input field、Offline STT via local Vosk WebSocket server、Draggable floating mic button with quick language switch、Voice and editing commands (new line, period, delete, undo, clear)、Arabic (Iraqi dialect) and English support
  - ⚠️ 注意:Default online mode relies on Chrome's proprietary Web Speech API; fully offline operation requires manually running the Python Vosk server and downloading Vosk models.
- **[vosk-browser](https://github.com/ccoreilly/vosk-browser)** ⭐520 · Apache-2.0 · TypeScript / JavaScript (browser WebAssembly) · Web · 中文 部分
  A browser speech recognition library that packages Vosk as a WebAssembly build running in a WebWorker. It enables fully offline speech-to-text inside the browser without a backend.
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2025-12-07)
  - 核心特性:Browser-only offline STT via WebAssembly、Runs in WebWorker、No backend required、Event-based API (result, partialresult)、Supports custom Vosk models and word timestamps
  - ⚠️ 注意:The library itself is a thin wrapper; actual recognition depends on externally downloaded Vosk model tar.gz files, which can be large. README notes that tests and automated publishing are still TODOs. The WASM binary is checked into the repo (~4.3 MB), which some users may dislike.
- **[Speechfire](https://github.com/Jejkobb/Speechfire)** ⭐27 · None · JavaScript, Python · Win/Linux/Web · 中文 部分
  Browser extension + local Whisper server for offline speech-to-text in Firefox/Chrome. Press Alt+A to record audio, send it to a local Flask server, and paste the transcription into the focused text…
  - 开源 ⚠️ | 可扩展 ✅ | 轻量 ⚠️(Browser extension is small, but the local server depends on PyTorch, openai-whis…) | 活跃度:maintenance(2026-01-29)
  - 核心特性:Firefox and Chrome extension、Local Whisper offline STT、Alt+A hotkey recording、Configurable Whisper model、Docker deployment
  - ⚠️ 注意:No open-source license; macOS explicitly unsupported; Chrome extension version (0.0.1) lags behind Firefox (1.5); heavy PyTorch/Whisper dependency means low-end machines run slowly.
- **[Whisper-Paste](https://github.com/redocrepus/Whisper-Paste)** ⭐13 · MIT · JavaScript (React) · Web/Windows/Mac/Linux · 中文 否
  一款 Chrome 浏览器扩展，通过快捷键录制语音并调用 OpenAI Whisper API 转写成文本，自动粘贴到当前光标位置，支持自定义提示词、多提示词、翻译及下载录音。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:abandoned(2023-09-29)
  - 核心特性:快捷键（Ctrl+Alt+R）启停语音录制、调用 OpenAI Whisper API 进行语音转文本、可自定义提示词以优化识别效果、支持多组提示词切换、自动将转写结果粘贴到当前输入框
  - ⚠️ 注意:项目自 2023-09-29 后无更新，状态接近废弃; README 作者自称不熟悉 Web 开发且仅投入数小时，可能存在 bug 或性能问题。运行必须自备有效的 OpenAI API key，且需将音频数据发送到 OpenAI 服务端，存在隐私与网络访问要求。
- **[voico](https://github.com/Kirera-Wainaina/voico)** ⭐1 · MIT（仅 package.json 声明，无根目录 LICENSE 文件） · TypeScript / JavaScript，Chrome Extension Manifest V3，Node.js 后端 · Windows/Mac/Linux/Web · 中文 否
  浏览器扩展，可将语音转写并输入到当前网页的激活输入框中；配套 Node.js 后端负责接收流式音频并调用 Google Cloud Speech / OpenAI 进行语音识别。
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ⚠️(扩展端运行时依赖为空，仅 devDependency @types/chrome；后端引入 @google-cloud/firestore、@google-cl…) | 活跃度:maintenance(2024-06-19)
  - 核心特性:语音转文本并自动填入网页输入框、Chrome 扩展（Manifest V3）、流式音频传输与转写、Google OAuth 身份识别、选项/设置页面
  - ⚠️ 注意:无 README; 后端需要 Google Cloud Firestore/Speech、OpenAI 密钥及 TLS 证书，部署门槛高于扩展端本身; 最近一次推送为 2024-06-19，项目活跃度低。

### 移动端语音输入（非 IME）
Android / iOS 上独立的语音转写应用，而非输入法键盘。
- **[Transcribro](https://github.com/soupslurpr/Transcribro)** ⭐723 · ISC · Kotlin, Android, C++ (whisper.cpp), Jetpack Compose · Android · 中文 否
  Private on-device speech recognition keyboard and service for Android, using OpenAI Whisper models via whisper.cpp and Silero VAD for voice activity detection.
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2025-08-29)
  - ⚠️ 注意:English-only at this time (locale filter set to 'en'); translations are not accepted. Android-only. Extensibility is limited to model swapping and Android STT service integration, with no formal plugin API.
- **[WhisperBoard](https://github.com/Saik0s/Whisperboard)** ⭐1040 · GPL-3.0 · Swift, SwiftUI / The Composable Architecture, whisper.cpp, Tuist · iOS · 中文 否
  Open-source iOS app for recording and transcribing voice using OpenAI's Whisper model locally on mobile devices.
  - 开源 ✅ | 可扩展 ⚠️ | 轻量 ✅ | 活跃度:active(2025-12-18)
  - 核心特性:One-tap recording and playback、OpenAI Whisper-based local transcription via whisper.cpp、Import and export audio files、Microphone selection、In-app download and selection of Whisper models
  - ⚠️ 注意:iOS-only; no plugin system or documented extension API; requires macOS and Xcode to build and run.
- **[seamless](https://github.com/woheller69/seamless)** ⭐84 · MIT · Java / Kotlin / Android Gradle · Android · 中文 否
  Android 端离线语音转文字并翻译为目标语言（S2TT）的应用。首次启动从 Hugging Face 下载 Meta Seamless M4T 的 torchscript lite 模型（~504 MB），之后所有 STT 与翻译推理均在设备端完成，无需联网。支持英/西/葡/印/俄五种目标语言，并可通过 Android TTS 朗读译文。
  - 开源 ⚠️ | 可扩展 ⚠️ | 轻量 ⚠️(App 本身为 Gradle/Android 工程，Java/Kotlin 实现，运行时依赖 Android Jetpack（AppCompat/Materia…) | 活跃度:active(2025-09-19)
  - 核心特性:离线 STT+翻译、设备端 PyTorch Lite 推理、首次启动下载 504 MB 模型后完全离线、支持英/西/葡/印/俄 5 种目标语言、Android TTS 朗读结果
  - ⚠️ 注意:模型文件采用 CC-BY-NC 4.0 授权，商用受限; 当前只支持 5 个目标语言按钮且硬编码在 UI 中，扩展语言需改源码; 中文不在支持列表内; 首次启动必须联网从 Hugging Face 下载 ~504 MB 模型，对低端设备存储和首次流量有一定要求; Android 12+ 动态权限需用户授予录音权限。

### 轻量脚本 / CLI 与语音控制
以单文件脚本、命令行、系统托盘触发器或小工具形式存在的轻量方案，适合开发者集成或作为现有工具链的补充。
- **[nerd-dictation](https://github.com/ideasman42/nerd-dictation)** ⭐1882 · GPL-3.0 · Python · Linux · 中文 部分
  基于 VOSK-API 的 Linux 离线语音转文字工具。通过手动 begin/end 命令激活，可将识别结果模拟成键盘输入注入到任意应用，也可输出到 stdout。核心定位是"为任何应用输入文字"，脚本化程度高，支持自定义文本后处理。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2025-10-10)
  - 核心特性:离线语音识别、手动 begin/end 激活、模拟键盘输入到任意应用、用户可编程的 Python 后处理、suspend/resume 降低大模型加载开销
  - ⚠️ 注意:目前仅官方支持 Linux（X11/Wayland）; Windows 和 macOS 在 Further Work 中列为未来可能支持。中文需自行下载 VOSK 中文模型并编写自定义后处理，项目未内置中文模型或中文文档。
- **[voice_typing](https://github.com/themanyone/voice_typing)** ⭐155 · GPL-2.0 · Shell · Linux/Windows · 中文 否
  基于 OpenAI Whisper/Whisper.cpp 的轻量 Shell 脚本，实现 Linux TTY、X/Wayland 或 Windows WSL 环境下的离线语音打字。通过 sox 录音、ydotool 模拟键盘输入，把语音实时转换为文本并键入任意活动文本域；同时提供 voice_client/voice_client_local 客户端/服务端模式，以及可选的…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-05-19)
  - 核心特性:离线语音转文本打字、支持 TTY/X/Wayland/WSL、纯 Bash 脚本、可选 Whisper/Whisper.cpp 后端、客户端/服务端模式
  - ⚠️ 注意:Windows 仅支持 WSL，无原生 Windows/macOS/Android/iOS 客户端; ydotool 权限/套接字配置对新手是主要门槛; 首次运行需要下载 Whisper 模型。
- **[hns](https://github.com/primaprashant/hns)** ⭐107 · MIT · Python 3.10+ · Linux/macOS/Windows · 中文 部分
  hns 是一个面向开发者的本地语音转文本命令行工具：录制麦克风音频，使用 faster-whisper 在本地完成转录，将结果输出到 stdout 并自动复制到剪贴板，可与 Claude Code、Ollama、LLM 等 CLI 工具组合使用。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-17)
  - 核心特性:本地麦克风录音并转文本、自动复制转录结果到剪贴板、基于 faster-whisper 的完全离线推理、stdout 输出便于管道组合、通过环境变量配置模型/语言/缓存目录
  - ⚠️ 注意:默认使用 CPU 推理(int8); 首次运行需下载 Whisper 模型; 代码为单文件结构，扩展性受限于缺少插件/Hook 机制; 无 Web/移动端。
- **[Elograf](https://github.com/papoteur-mga/elograf)** ⭐82 · GPL-3.0 · Python 3.7+, PyQt6, vosk, ujson · Linux · 中文 否
  Elograf 是 nerd-dictation 的图形化管理器/启动器，常驻系统托盘，提供语音识别的开始/暂停/恢复/停止控制、模型下载管理、音频设备选择、预/后处理命令、KDE 全局快捷键等功能。
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-03-01)
  - 核心特性:系统托盘图标状态显示、点击/菜单控制听写状态、Vosk 模型下载与管理、PulseAudio 输入设备选择、X11/Wayland 输入模拟(XDOTOOL/DOTOOL)
- **[Osprey](https://github.com/osprey-voice/osprey)** ⭐26 · MIT · Python · Linux/macOS · 中文 部分
  Osprey is a cross-platform, command-based voice control / voice typing program. Users define voice commands in Python scripts; Osprey compiles a strict grammar, performs local speech recognition via…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ⚠️(Pure Python project (pyproject.toml). No GPU requirement; recognition uses CPU-b…) | 活跃度:abandoned(2021-01-03)
  - ⚠️ 注意:Last code push was 2021-01-03, so the project appears unmaintained. Windows installation is marked TODO in the README. Chinese is not mentioned; language support depends on the availability of a compatible Kaldi model, not on built-in localization.

### 其他值得了解
fit_score 较低或未归入上述类别的项目,仍可作为特定场景参考。
- **[VoxType](https://github.com/peteonrails/voxtype)** ⭐909 · MIT · Rust · Linux/macOS · 中文 是
  Local push-to-talk voice-to-text for Linux/Wayland (and macOS), running multiple ASR engines (Whisper, Parakeet, Moonshine, SenseVoice, Paraformer, Dolphin, Omnilingual) locally on CPU or optional…
  - 开源 ✅ | 可扩展 ✅ | 轻量 ✅ | 活跃度:active(2026-06-30)
  - 核心特性:Push-to-talk/toggle voice-to-text、7 local ASR engines including Whisper and ONNX-based engines、CPU-first with optional GPU (Vulkan/CUDA/Metal/ROCm)、Post-processing via external LLM or shell script、Meeting mode with speaker attribution and export (Markdown/JSON/SRT/VTT)
  - ⚠️ 注意:Primary platform is Linux/Wayland; macOS and X11 are supported but secondary. Some advanced engines require building from source with specific Cargo features.

## 开源方案 vs 对标产品

| 维度 | 开源方案整体 | Typeless | Lazytype | 闪电说（Shandianshuo） |
|------|--------------|----------|----------|----------------------|
| 开源性与可控性 | 源码完全公开，可本地离线运行，无订阅、无数据上传，适合隐私敏感场景 | 闭源商业软件，隐私承诺为“零云端数据留存”，但代码不可审计 | 闭源商业软件，提供本地 whisper.cpp 路径，但核心闭源 | 闭源商业产品，本地优先但核心代码不开放 |
| 系统级集成 | 部分项目（如 nerd-dictation、Vocalinux、VocoType-linux）支持全局热键/IBus 输入，但整体集成深度、稳定性、辅助功能 API 调用与 Typeless 相比仍显分散 | 深度 OS 级集成，可读取/写入任意应用文本框，上下文感知强 | 跨 Windows/macOS 的按住即写、悬浮预览、应用上下文适配 | 深度适配微信/钉钉/飞书等中文 IM，支持屏幕上下文与沟通 Agent |
| 中文识别与本地化 | SenseVoice/FunASR/Paraformer 等中文 ASR 已很强；VocoType-linux、voice-input-method 等专门优化中文输入法，但 UI/文档汉化、热词纠错距离商业产品仍有差距 | 支持 100+ 语言自动检测，中文可用但非专门优化 | 对英语/荷兰语效果最好，中文可用但非强项 | 以中文为核心，低延迟 SenseVoice、中文纠错、个人记忆/知识库、技能系统针对中文场景 |
| AI 后处理与 Agent 能力 | HoldSpeak、VoiceFlow、voicisst、amical 等可接入 LLM 润色/总结；但多为配置化接入，缺乏 Typeless/闪电说那样统一的上下文 Agent 工作流 | 上下文感知转写、语音指令、Ask AI、自动格式化，Agent 能力最成熟 | 支持 AI 清理、翻译、语气调整、语音宏，工作流较成熟 | 长按唤起“帮我说”Agent，结合屏幕上下文与个人记忆生成回复，中文场景领先 |
| 跨平台与移动端 | 多为桌面端（Linux/macOS/Windows），移动端和键盘输入法项目较少且成熟度参差 | macOS/Windows/iOS/Android 全平台 | Windows/macOS | 主要面向中文桌面用户，移动端能力未公开 |
| 安装与易用性 | 往往需要自行下载模型、配置环境、解决依赖，对非技术用户门槛较高 | 一键安装、自动更新、商业化支持 | 安装相对简单，提供 Personal/Pro 订阅 | 提供云端会员开箱即用，也可 BYOK 免费使用 |
| 成本 | 免费/社区驱动，硬件与模型下载成本由用户承担 | 付费订阅/买断 | 订阅或 BYOK | 免费 BYOK + 会员订阅 |
| 生态与扩展 | 插件生态薄弱，多数靠源码修改或配置扩展；TypeWhisper 等少数项目已有插件 SDK，但社区规模小 | 商业团队持续迭代，生态成熟 | 商业团队维护 | 商业团队维护，技能系统可扩展 |

## 如何选型(按场景)

基于项目数据,给出以下 5 条具体建议:

1. **最接近 Typeless 体验(跨平台+实时+可扩展):** 首选 **[Handy](https://github.com/cjpais/Handy)**。Rust+Tauri 跨三端、内置 Whisper/Parakeet、支持 Raycast 扩展与 CLI,fit_score 4,功能完整度最接近商业级。
2. **最轻量纯 CPU / 脚本化:** 首选 **[voice_typing](https://github.com/themanyone/voice_typing)**。纯 Bash 脚本,依赖 sox/ydotool/Whisper,无 GUI 包袱,适合 Linux/WSL 下追求极简的用户。
3. **中文最优 / 本土输入法替代:** 首选 **[Aria](https://github.com/Xingxun7777/Aria)**。针对中文场景优化,支持 Qwen3-ASR/FunASR、屏幕 OCR 感知、热词纠错与语音指令,中文支持“是”。
4. **二次开发底座 / ASR 引擎:** 首选 **[whisper.cpp](https://github.com/ggml-org/whisper.cpp)**。C/C++ 高性能移植,多平台/多后端 GPU 可选,CPU 即可跑,适合嵌入自有产品或做上层包装。
5. **离线隐私 / 会议+听写一体化:** 首选 **[HoldSpeak](https://github.com/karolswdev/HoldSpeak)**。插件化会议智能流水线、14+ 内置插件、本地 LLM 可选,适合需要语音输入+会议纪要的场景。

## 结构化数据

完整机器可读数据见 [`data/awesome.json`](data/awesome.json)(含每个项目的全部字段、对抗验证修正意见、对标产品详情)。

## 贡献

欢迎补充遗漏或更新过时信息。请提 PR,新增项目需:① GitHub(或公开 forge)可访问 ② OSI 许可证 ③ 明确标注语音输入/听写用途 ④ 标注三标准评估依据。

## License

清单内容采用 [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/)。各项目自身 License 以其仓库为准。

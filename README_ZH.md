# Audio Plugins — 历史、类型、技术与开发框架

这是一份关于 **audio plugins**（音频插件）的全面单页介绍 —— 涵盖塑造几乎所有录制声音的各类软件模块（EQ、compressor、reverb、synthesiser 等）。内容梳理了从外置硬件到现代 DAW 的演变历史，全景介绍了主流 plugin 格式（VST3、AU/AUv3、AAX、CLAP、LV2），归纳了常见的插件类型，剖析了 plugin 的内部架构（anatomy）以及 real-time audio 约束规范，对比了用于构建它们的开发框架（JUCE、iPlug2、DPF、nih-plug、Faust、RNBO…），并提供了深入的 JUCE 教程以及七个可实际运行与试听的示例 plugin。

**▶ 在线演示站点：** https://brendanjameslynskey.github.io/Audio_Plugins/

本项目属于 [DSP & Music](https://github.com/BrendanJamesLynskey/DSP_and_Music) 系列合辑。

## 目录
- **什么是 audio plugin？** — host 与 plugin 的关系、`f(x)` 模型、浏览器内实时演示
- **历史** — Sound Tools 与 TDM → VST (1996) → AU → RTAS/AAX → VST3 → AUv3 → CLAP (2022)
- **格式** — 对比 VST2/3、AU、AUv3、AAX、CLAP、LV2、LADSPA/DSSI、RTAS 以及 Standalone
- **常见的插件类型** — EQ、dynamics、reverb、delay、distortion、modulation、pitch/time、spectral、utility、instruments、samplers、MIDI effects
- **Plugin 的内部架构** — processor、parameters、state、editor；real-time 规范约束
- **开发框架** — JUCE、iPlug2、DPF、nih-plug、Faust、Cmajor、RNBO 以及原生 SDK
- **DSP 基础构建模块** — sample loop、biquads、delay lines、envelopes、oscillators、nonlinearities、transforms
- **构建与发布** — 验证（`auval`、`pluginval`）、签名与公证（signing/notarisation）、安装包（installers）、latency（延迟）
- **项目合辑** — JUCE 教程与全部七个示例 plugin 的链接

## 项目合集列表
| 仓库 | 涉及内容 |
|------|----------------|
| [JUCE_Tutorial](https://github.com/BrendanJamesLynskey/JUCE_Tutorial) | 深入讲解的 JUCE plugin 教程 |
| [Plugin_Example_EQ](https://github.com/BrendanJamesLynskey/Plugin_Example_EQ) | Parametric equaliser（参数均衡器） |
| [Plugin_Example_Compressor](https://github.com/BrendanJamesLynskey/Plugin_Example_Compressor) | Dynamics compressor（动态压缩器） |
| [Plugin_Example_Reverb](https://github.com/BrendanJamesLynskey/Plugin_Example_Reverb) | Algorithmic reverb（算法混响） |
| [Plugin_Example_Delay](https://github.com/BrendanJamesLynskey/Plugin_Example_Delay) | Delay / echo（延迟 / 回声） |
| [Plugin_Example_Distortion](https://github.com/BrendanJamesLynskey/Plugin_Example_Distortion) | Distortion / saturation（失真 / 饱和度） |
| [Plugin_Example_Modulation](https://github.com/BrendanJamesLynskey/Plugin_Example_Modulation) | Chorus / flanger / phaser（合唱 / 镶边 / 移相） |
| [Plugin_Example_Synth](https://github.com/BrendanJamesLynskey/Plugin_Example_Synth) | Subtractive synthesiser（减法合成器） |

## 制作信息
由 Brendan Lynskey 构建。数学公式使用 KaTeX 渲染。所有音频均通过 Web Audio API 实时合成与处理。
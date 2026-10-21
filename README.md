<!-- portfolio-strip:start (brief 40) -->
<sub>**Brendan Lynskey** · [Portfolio home](https://brendanjameslynskey.github.io/) · [Interactive sites](https://brendanjameslynskey.github.io/#sites)</sub>
<!-- portfolio-strip:end -->

# Audio Plugins — History, Types, Technologies & Frameworks

A comprehensive, single-page presentation on **audio plugins** — the software modules
(EQs, compressors, reverbs, synthesisers) that shape almost every recorded sound. It
traces their history from outboard hardware to the modern DAW, surveys the plugin
formats (VST3, AU/AUv3, AAX, CLAP, LV2), catalogues the types commonly built, dissects
the anatomy of a plugin and the real-time audio contract, compares the frameworks used
to build them (JUCE, iPlug2, DPF, nih-plug, Faust, RNBO…), and links to an in-depth JUCE
tutorial and seven working, playable example plugins.

**▶ Live site:** https://brendanjameslynskey.github.io/Audio_Plugins/

Part of the [DSP & Music](https://github.com/BrendanJamesLynskey/DSP_and_Music) collection.

## Contents
- **What is an audio plugin?** — the host/plugin relationship, `f(x)` model, a live in-browser demo
- **History** — Sound Tools & TDM → VST (1996) → AU → RTAS/AAX → VST3 → AUv3 → CLAP (2022)
- **Formats** — comparison of VST2/3, AU, AUv3, AAX, CLAP, LV2, LADSPA/DSSI, RTAS, Standalone
- **The types commonly built** — EQ, dynamics, reverb, delay, distortion, modulation, pitch/time, spectral, utility, instruments, samplers, MIDI effects
- **Anatomy of a plugin** — processor, parameters, state, editor; the real-time contract
- **Frameworks** — JUCE, iPlug2, DPF, nih-plug, Faust, Cmajor, RNBO and the raw SDKs
- **DSP building blocks** — the sample loop, biquads, delay lines, envelopes, oscillators, nonlinearities, transforms
- **Building & shipping** — validation (`auval`, `pluginval`), signing/notarisation, installers, latency
- **The collection** — links to the JUCE tutorial and all seven example plugins

## The family
| Repo | What it covers |
|------|----------------|
| [JUCE_Tutorial](https://github.com/BrendanJamesLynskey/JUCE_Tutorial) | In-depth JUCE plugin tutorial |
| [Plugin_Example_EQ](https://github.com/BrendanJamesLynskey/Plugin_Example_EQ) | Parametric equaliser |
| [Plugin_Example_Compressor](https://github.com/BrendanJamesLynskey/Plugin_Example_Compressor) | Dynamics compressor |
| [Plugin_Example_Reverb](https://github.com/BrendanJamesLynskey/Plugin_Example_Reverb) | Algorithmic reverb |
| [Plugin_Example_Delay](https://github.com/BrendanJamesLynskey/Plugin_Example_Delay) | Delay / echo |
| [Plugin_Example_Distortion](https://github.com/BrendanJamesLynskey/Plugin_Example_Distortion) | Distortion / saturation |
| [Plugin_Example_Modulation](https://github.com/BrendanJamesLynskey/Plugin_Example_Modulation) | Chorus / flanger / phaser |
| [Plugin_Example_Synth](https://github.com/BrendanJamesLynskey/Plugin_Example_Synth) | Subtractive synthesiser |

## Credits
Built by Brendan Lynskey. Maths rendered with KaTeX. All audio synthesised and processed
live with the Web Audio API.

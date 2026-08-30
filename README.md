# Waveform — Making Sound Visible

**Live site:** [https://sound-core-vert.vercel.app/](https://sound-core-vert.vercel.app/)

An interactive visualization that makes an invisible phenomenon — sound — visible in real time. Sound is just air pressure changing thousands of times a second; this page listens through your microphone and draws that pressure wave live as a glowing, reactive ring.

Built for the **"Make the Invisible Visible"** challenge, Website track.

## What it does

- Renders a full-screen radial waveform on an HTML5 canvas, driven by the Web Audio API
- On load, animates a procedurally generated demo signal so the visual is never static
- Click **"Enable microphone"** to switch to live audio — the ring's shape, color, and particle bursts react to your actual voice in real time
- Color maps to dominant frequency: warm red for bass, amber for mid, teal for treble
- A live readout shows dominant frequency (Hz) and amplitude (%) as it updates
- An explainer section breaks down the three properties of sound (frequency, amplitude, timbre) driving the visual

## Tech stack

- Vanilla HTML, CSS, and JavaScript — no framework, no build step
- Canvas 2D API for rendering
- Web Audio API (`AnalyserNode`) for live audio analysis
- Google Fonts: Space Grotesk, Inter, JetBrains Mono

## Privacy

No audio is recorded, stored, or transmitted anywhere. All analysis happens client-side, live, in the browser's `AnalyserNode` — nothing leaves the page.

## Project structure

```
SoundCore/
├── index.html    # entire site — markup, styles, and script in one file
└── README.md
```

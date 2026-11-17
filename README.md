# AI Podcast Generator 🎙️✨

A modern, responsive, 3D interactive web application for generating AI podcasts from any topic prompt. Built with Three.js, GSAP, Web Audio API, and integrated with an automated n8n workflow pipeline.

![Theme](https://img.shields.io/badge/Theme-Deep%20Black%20Teal-0a7075?style=flat-square)
![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=flat-square)
![GSAP](https://img.shields.io/badge/GSAP-3.12.5-green?style=flat-square)

---

## ✨ Features

- **3D Procedural Centerpiece:** Interactive layered 3D shield with custom GLSL vertex and fragment shaders reacting to cursor physics and real-time audio frequencies.
- **Micro-Interaction Sound Synthesizer:** Fully procedural Web Audio API sound generator providing tactile clicks, hover chimes, and generation sweeps with autoplay safeguards and cooldown management.
- **Glassmorphic UI Design:** Deep Black Teal theme with fluid responsive typography, kinetic text reveals (SplitType), and interactive card tilts.
- **Real-Time Visualizer:** Live FFT audio analyzer analyzing bass and treble frequencies to drive dynamic shader animations during playback.
- **n8n Automation Ready:** Configurable Webhook endpoint that sends the topic as JSON and receives raw binary `.mp3` audio, loading it directly into the audio player.

---

## 🚀 Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/Milan-6/Podcast-Generator.git
   cd Podcast-Generator
   ```

2. Open `index.html` in your browser.

3. Configure your webhook:
   Open `index.html` and update line 381 with your live n8n webhook URL:
   ```javascript
   const WEBHOOK_URL = "https://your-n8n-instance.com/webhook/generate-podcast";
   ```

---

## 🛠️ Stack

- **Frontend:** Vanilla HTML5, Modern CSS (Grid/Flexbox, 3D Transforms), Vanilla JavaScript (ES6+)
- **Graphics & Motion:** Three.js (WebGL Shaders), GSAP, SplitType
- **Audio:** Web Audio API (AnalyserNode, BiquadFilter, Oscillators)
- **Backend / Integration:** n8n Webhook Workflow (LLM script generation & TTS synthesis)

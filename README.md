<div align="center">

<!-- Animated gradient wave banner - music themed colors -->
<img src="https://capsule-render.vercel.app/api?type=soft&color=gradient&customColorList=12,18,24&height=200&section=header&text=MelodyForge&fontSize=55&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=AI%20Music%20%26%20Ambient%20Soundscape%20Generator&descAlignY=55&descSize=17" width="100%"/>

<!-- Animated typing subtitle -->
<img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=26&duration=2800&pause=900&color=C77DFF&center=true&vCenter=true&multiline=true&repeat=true&width=750&height=90&lines=%F0%9F%8E%B5+Composing+Music+with+LSTM+Neural+Networks;%F0%9F%8C%8A+Live+Ambient+Soundscapes+in+Your+Browser;%F0%9F%8E%A7+Focus+%7C+Relax+%7C+Energetic" alt="Typing SVG" />

<br/>

<p align="center">
  <img src="https://img.shields.io/badge/Python-TensorFlow%2FKeras-9D4EDD?style=for-the-badge&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/LSTM-Deep%20Learning-5A189A?style=for-the-badge&logo=brain&logoColor=white"/>
  <img src="https://img.shields.io/badge/Web%20Audio%20API-JavaScript-F72585?style=for-the-badge&logo=javascript&logoColor=white"/>
  <img src="https://img.shields.io/badge/music21-MIDI%20Parsing-7209B7&style=for-the-badge"/>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/ayeshajavid91-star/MelodyForge?style=for-the-badge&color=C77DFF&labelColor=240046"/>
  <img src="https://img.shields.io/github/forks/ayeshajavid91-star/MelodyForge?style=for-the-badge&color=E0AAFF&labelColor=240046"/>
  <img src="https://img.shields.io/github/last-commit/ayeshajavid91-star/MelodyForge?style=for-the-badge&color=success&labelColor=240046"/>
  <img src="https://img.shields.io/badge/License-All%20Rights%20Reserved-critical?style=for-the-badge&labelColor=240046"/>
</p>

<p align="center">
  <a href="https://ayeshajavid91-star.github.io/MelodyForge/">
    <img src="https://img.shields.io/badge/🎧_LAUNCH_LIVE_DEMO-Click_to_Listen-F72585?style=for-the-badge&labelColor=10002B"/>
  </a>
</p>

</div>

<div align="center">
<img src="https://raw.githubusercontent.com/mayhemantt/mayhemantt/Update/svg/Bottom.svg" width="100%"/>
</div>

<br/>

<!-- Animated audio wave gif -->
<div align="center">
<img src="https://raw.githubusercontent.com/aritranath/aritranath/main/wave.gif" width="100%" height="4"/>
</div>

<br/>

## 📚 Table of Contents

<div align="center">

| 🎼 [Overview](#-project-overview) | ✨ [Features](#-features) | 🛠️ [Tech Stack](#️-tech-stack) | ⚙️ [How It Works](#️-how-it-works) |
|:---:|:---:|:---:|:---:|
| ▶️ [Run It](#️-how-to-run) | 📂 [Structure](#-project-structure) | 🎚️ [Mood Engine](#️-mood-engine) | 🗺️ [Roadmap](#️-roadmap) |
| 🤝 [Contributing](#-contributing) | 👤 [Author](#-author) | 📄 [License](#-license) | |

</div>

---

## 📌 Project Overview

<img align="right" width="240" src="https://raw.githubusercontent.com/ashutosh1919/ashutosh1919/master/gifs/knowledge.gif"/>

**MelodyForge** is a two-part sonic experiment:

🎼 **1. AI Music Generator** — an **LSTM deep learning model** trained on preprocessed MIDI sequences, learning musical patterns note by note to compose brand-new original piano pieces.

🌊 **2. Ambient Soundscape Generator** — a **browser-based synthesizer** that generates mood-driven ambient audio (**Focus / Relax / Energetic**) live using the **Web Audio API** — every sound is generated in real time, nothing is pre-recorded.

> 💡 One half learns from centuries of composed music. The other half never plays the same soundscape twice.

<br clear="right"/>

---

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🧠 AI Music Generation
- Parses MIDI files into note/chord sequences via `music21`
- Numeric encoding of notes for model input
- **LSTM architecture** — Embedding → LSTM → Dense
- Generates entirely new, original note sequences
- Exports directly to a playable **`.mid`** file

</td>
<td width="50%" valign="top">

### 🌊 Ambient Soundscape Engine
- Three moods: **Focus 🎯 · Relax 🌙 · Energetic ⚡**
- Unique frequency, waveform & tempo per mood
- **Real-time synthesis** — evolves with subtle randomness
- Live **radial visualizer** reacting to generated audio
- 100% client-side — zero audio files, zero server

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Badge |
|:---|:---|:---:|
| **Model Training** | Python, TensorFlow/Keras | ![TF](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) |
| **MIDI Parsing** | music21 | ![music21](https://img.shields.io/badge/music21-7209B7?style=flat-square) |
| **Sequence Model** | LSTM Neural Network | ![LSTM](https://img.shields.io/badge/LSTM-5A189A?style=flat-square) |
| **Web Synthesis** | Web Audio API | ![WebAudio](https://img.shields.io/badge/Web%20Audio%20API-F72585?style=flat-square) |
| **Frontend** | HTML, CSS, JavaScript | ![JS](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) |
| **Training Environment** | Google Colab | ![Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white) |

</div>

---

## ⚙️ How It Works

<div align="center">

```mermaid
flowchart TB
    subgraph AI["🎼 AI Music Generation"]
    A1[🎹 MIDI Dataset] --> A2[🔤 Note/Chord Parsing - music21]
    A2 --> A3[🔢 Numeric Encoding]
    A3 --> A4[🧠 LSTM Training]
    A4 --> A5[🎶 New Sequence Generated]
    A5 --> A6[💾 Export as .mid]
    end

    subgraph AMB["🌊 Ambient Soundscape"]
    B1[🎯 Mood Selected] --> B2[🎛️ Frequency + Waveform Profile]
    B2 --> B3[🔊 Web Audio Oscillators]
    B3 --> B4[✨ Continuous Evolving Layers]
    B4 --> B5[📊 Live Radial Visualizer]
    end

    style A4 fill:#5A189A,stroke:#000,color:#fff
    style A6 fill:#C77DFF,stroke:#000,color:#000
    style B3 fill:#F72585,stroke:#000,color:#fff
    style B5 fill:#E0AAFF,stroke:#000,color:#000
```

</div>

<table>
<tr><th colspan="2">🎼 Music Generation Pipeline</th></tr>
<tr><td>1️⃣</td><td>MIDI files are parsed into note/chord sequences</td></tr>
<tr><td>2️⃣</td><td>Sequences are encoded numerically for model input</td></tr>
<tr><td>3️⃣</td><td>An LSTM network learns to predict the next note from prior context</td></tr>
<tr><td>4️⃣</td><td>The trained model generates a new sequence → exported as <code>.mid</code></td></tr>
</table>

<table>
<tr><th colspan="2">🌊 Soundscape Synthesis Pipeline</th></tr>
<tr><td>1️⃣</td><td>A mood is selected — Focus, Relax, or Energetic</td></tr>
<tr><td>2️⃣</td><td>Web Audio API generates oscillator tones matching that mood's profile</td></tr>
<tr><td>3️⃣</td><td>New notes layer in continuously with slight variation — never repeats</td></tr>
</table>

---

## 🎚️ Mood Engine

<div align="center">

| Mood | Icon | Vibe | Waveform | Tempo |
|:---|:---:|:---|:---:|:---:|
| **Focus** | 🎯 | Steady, minimal, clear-headed | Sine | Slow |
| **Relax** | 🌙 | Warm, drifting, low-frequency | Triangle | Very Slow |
| **Energetic** | ⚡ | Bright, layered, driving | Sawtooth | Fast |

</div>

---

## ▶️ How to Run

### 🎧 Ambient Soundscape App — Instant, No Install

<div align="center">

[![Launch App](https://img.shields.io/badge/▶️_Launch-MelodyForge-F72585?style=for-the-badge&labelColor=10002B)](https://ayeshajavid91-star.github.io/MelodyForge/)

</div>

Or run it locally:

```bash
# 1️⃣ Clone the repository
git clone https://github.com/ayeshajavid91-star/MelodyForge.git

# 2️⃣ Move into the project folder
cd MelodyForge

# 3️⃣ Open in your browser
open index.html      # macOS
start index.html      # Windows
```

### 🧠 Train the AI Music Model

<table>
<tr><td>1️⃣</td><td>Open <a href="https://colab.research.google.com">Google Colab</a></td></tr>
<tr><td>2️⃣</td><td>Upload <code>AI_Music_Generator_Training.ipynb</code></td></tr>
<tr><td>3️⃣</td><td>Add <code>.mid</code> files to a <code>midi_dataset</code> folder (e.g. Classical Piano MIDI dataset on Kaggle)</td></tr>
<tr><td>4️⃣</td><td>Run all cells (<i>Runtime → Run all</i>)</td></tr>
<tr><td>5️⃣</td><td>Download the generated <code>.mid</code> output</td></tr>
</table>

<div align="center">
<img src="https://img.shields.io/badge/Training_Time-~15--30_min_(GPU)-blueviolet?style=flat-square"/>
<img src="https://img.shields.io/badge/Difficulty-Intermediate-orange?style=flat-square"/>
</div>

---

## 📂 Project Structure

```
MelodyForge/
├── 🧠 AI_Music_Generator_Training.ipynb   # LSTM model training notebook
├── 🌐 index.html                          # Ambient soundscape web app
├── 🎵 generated_music.mid                 # Sample AI-generated output
├── 💾 music_lstm_model.h5                 # Trained LSTM model
└── 📖 README.md                           # You are here
```

---

## 🗺️ Roadmap

- [x] LSTM-based MIDI music generation
- [x] Real-time Web Audio ambient synth
- [x] Mood-based soundscape presets
- [ ] Export soundscape sessions as audio files
- [ ] Add Transformer-based music generation option
- [ ] Custom mood builder (user-defined frequencies)
- [ ] Mobile-optimized visualizer

---

## 🤝 Contributing

Contributions, issues, and feature ideas are welcome for discussion — please reach out to the author first, as this repository is **All Rights Reserved** (see [License](#-license)).

<div align="center">
<img src="https://img.shields.io/badge/PRs-By_Permission_Only-orange?style=for-the-badge"/>
</div>

---

## 🏷️ Suggested GitHub Topics

<div align="center">

`python` • `deep-learning` • `lstm` • `music-generation` • `web-audio-api` • `javascript` • `midi` • `generative-art`

</div>

---

## 👤 Author

<div align="center">

<img src="https://api.dicebear.com/7.x/initials/svg?seed=Ayesha%20Javid&backgroundColor=7209B7" width="90" style="border-radius:50%"/>

### **Ayesha Javid**

<a href="https://github.com/ayeshajavid91-star"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="mailto:ayeshajavid91@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>

</div>

---

## 📄 License

**All Rights Reserved.**

This project and its source code are the intellectual property of the author. No part of this repository — including the code, design, or documentation — may be copied, modified, distributed, used, or reproduced in any form without the explicit written permission of the author.

© 2026 Ayesha Javid. Unauthorized use is strictly prohibited.

📧 For permissions or licensing inquiries, contact: **ayeshajavid91@gmail.com**

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=soft&color=gradient&customColorList=12,18,24&height=120&section=footer"/>

<sub>🎵 If this project struck a chord with you, consider giving it a star! ⭐</sub>
</div>

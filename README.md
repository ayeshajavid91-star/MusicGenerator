# 🎵 MelodyForge

An **AI Music & Ambient Soundscape Generator** combining a deep learning model that composes original music from MIDI sequences with a live, mood-based soundscape app that synthesizes ambient audio directly in the browser.

**🔗 Live Demo:** [https://ayeshajavid91-star.github.io/MelodyForge/](https://ayeshajavid91-star.github.io/MelodyForge/)

---

## 📌 Project Overview

MelodyForge consists of two complementary parts:

1. **AI Music Generator** — an LSTM deep learning model trained on preprocessed MIDI sequences, learning musical patterns to generate brand-new original compositions.
2. **Ambient Soundscape Generator** — a browser-based app that synthesizes mood-driven ambient audio (Focus / Relax / Energetic) live using the Web Audio API — no pre-recorded audio files involved.

---

## ✨ Features

### 🧠 AI Music Generation (LSTM Model)
- Preprocesses MIDI files into note/chord sequences using `music21`
- Encodes notes into numeric sequences for training
- **LSTM architecture** (Embedding → LSTM → Dense layers) learns musical patterns
- Generates entirely new note sequences from the trained model
- Converts generated sequences back into a playable `.mid` file

### 🌊 Ambient Soundscape App (Web Audio API)
- Three distinct moods: **Focus**, **Relax**, and **Energetic**
- Each mood maps to a unique set of frequencies, waveform shape, filter tone, and tempo
- **Real-time synthesis** — sound is generated continuously and evolves with subtle randomness, never looping a fixed track
- Live **radial visualizer** that reacts to the generated audio
- Runs entirely client-side — no audio files, no server required

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Model Training | Python, TensorFlow/Keras (LSTM), music21 |
| Web App | HTML, CSS, JavaScript, Web Audio API |
| Environment | Google Colab (for training) |

---

## ⚙️ How It Works

**Music Generation Pipeline:**
1. MIDI files are parsed into note/chord sequences
2. Sequences are encoded numerically for model input
3. An LSTM network is trained to predict the next note given a sequence of previous notes
4. The trained model generates a new sequence, which is converted back into a `.mid` file

**Soundscape Synthesis:**
1. A mood is selected (Focus / Relax / Energetic)
2. The Web Audio API generates oscillator-based tones matching that mood's frequency/waveform profile
3. New notes are layered in continuously with slight variation, creating an evolving, non-repeating soundscape

---

## ▶️ How to Run

### 🎧 Ambient Soundscape App (Instant)
No installation needed — try it live:
👉 **[Open MelodyForge](https://ayeshajavid91-star.github.io/MelodyForge/)**

Or run locally:
```bash
git clone https://github.com/ayeshajavid91-star/MelodyForge.git
cd MelodyForge
```
Then open `index.html` in your browser.

### 🧠 Train the AI Music Model
1. Open [Google Colab](https://colab.research.google.com)
2. Upload `AI_Music_Generator_Training.ipynb`
3. Add `.mid` files to a `midi_dataset` folder (e.g. the Classical Piano MIDI dataset on Kaggle)
4. Run all cells (Runtime → Run all)
5. Download the generated `.mid` output

---

## 📂 Project Structure

```
MelodyForge/
├── AI_Music_Generator_Training.ipynb   # LSTM model training notebook
├── index.html                            # Ambient soundscape web app
├── generated_music.mid                    # Sample AI-generated output
├── music_lstm_model.h5                     # Trained LSTM model
└── README.md
```

---

## 🏷️ Suggested GitHub Topics

```
python
deep-learning
lstm
music-generation
web-audio-api
javascript
```

---

## 👤 Author

Developed by **Ayesha Javid**.

---

## 📄 License

**All Rights Reserved.**

This project and its source code are the intellectual property of the author. No part of this repository — including the code, design, or documentation — may be copied, modified, distributed, used, or reproduced in any form without the explicit written permission of the author.

© 2026 Ayesha Javid. Unauthorized use is strictly prohibited.

For permissions or licensing inquiries, contact: **ayeshajavid91@gmail.com**

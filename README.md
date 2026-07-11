# 🎵 AI Music & Soundscape Generator

InternGrow Artificial Intelligence Track — Task 3

## What's in this repo

| File | Purpose |
|---|---|
| `AI_Music_Generator_Training.ipynb` | Trains an **LSTM deep learning model** on preprocessed MIDI sequences and generates new music (the core task) |
| `index.html` | **Upgrade feature** — a mood-based app (Focus / Relax / Energetic) that generates ambient soundscapes live in the browser |
| `generated_music.mid` | Sample output from the trained model *(add after running the notebook)* |

---

## Part 1: Model Training (`AI_Music_Generator_Training.ipynb`)

### How to run
1. Go to [Google Colab](https://colab.research.google.com)
2. Upload `AI_Music_Generator_Training.ipynb` (File → Upload notebook)
3. Add a few `.mid` files to the `midi_dataset` folder in Colab's file browser (left sidebar) — a free dataset like **Classical Piano MIDI** on Kaggle works well
4. Run all cells (Runtime → Run all)

### What it does
1. **Preprocesses** MIDI files into note/chord sequences using `music21`
2. **Encodes** notes into numeric sequences the network can learn from
3. Builds an **LSTM** architecture (Embedding → LSTM → Dense layers)
4. **Trains** the model to predict the next note given a sequence of previous notes
5. **Generates** a brand-new sequence of notes from the trained model
6. Converts the generated sequence back into a playable `generated_music.mid` file

This satisfies the core task requirement: *"Train a deep learning architecture (RNN, LSTM, or GAN) on preprocessed MIDI musical sequences to learn underlying patterns."*

---

## Part 2: Mood-Based Soundscape App (`index.html`) — Upgrade Feature

A single-file web app with **no external audio files** — every sound is synthesized live using the **Web Audio API**.

### How it works
- Each mood (**Focus, Relax, Energetic**) maps to a different set of frequencies, waveform shape, filter tone, and tempo
- On selection, the app continuously generates new notes on the fly with slight randomness — so the soundscape evolves rather than looping a fixed track
- A radial visualizer reacts to the live audio output

### Run it
Just open `index.html` in a browser — no server or install needed.

### Deploy on GitHub Pages
1. Push this repo to GitHub (repo name: `InternGrow_MusicGenerator`)
2. Settings → Pages → Source: `main` branch, `/ (root)` → Save
3. Live link: `https://YOUR-USERNAME.github.io/InternGrow_MusicGenerator/`

---

## Submission checklist
- [ ] Run the notebook fully in Colab, keep outputs visible, export/download it
- [ ] Download the generated `.mid` file from Colab and add it to this repo
- [ ] Push all files to GitHub under `InternGrow_MusicGenerator`
- [ ] Record a demo video showing both the training notebook output and the live mood app
- [ ] Post on LinkedIn tagging @InternGrow with the GitHub link

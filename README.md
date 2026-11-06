# Persian & English Neural Speech Synthesis & G2P Research Showcase (GitHub Pages)

A minimalist, responsive, and lightweight academic showcase website for **Text-to-Speech (TTS)** and **Grapheme-to-Phoneme (G2P)** research projects developed by **Soroush Soleimani** and **Melika Parhiz**.

---

## 🌟 Featured Projects Included

1. **Large-Scale Persian G2P via ByT5 Domain Adaptation** (*Soroush Soleimani*)
   - **GitHub**: [SoroushSoleimani/g2p-byt5-minifinetune](https://github.com/SoroushSoleimani/g2p-byt5-minifinetune)
   - **Kaggle**: [g2p-implementation-and-mini-finetune-byt5](https://www.kaggle.com/code/soroushsoleimani/g2p-implementation-and-mini-finetune-byt5)
   - **Audio Samples**: Side-by-side Before vs. After fine-tuning `.wav` comparisons (recovering short vowels, Ezafe `-e-`, and gemination).

2. **End-to-End Persian G2P with VITS TTS** (*Melika Parhiz*)
   - **GitHub**: [melolikepz/persian-g2p-vits](https://github.com/melolikepz/persian-g2p-vits)
   - **Kaggle**: [persian-g2p-vits-kaggle](https://www.kaggle.com/code/melikaparhiz/persian-g2p-vits-kaggle)
   - **Audio Sample**: `kaggle_sample.wav` generated via Coqui VITS on ManaTTS dataset with `Homo-GE2PE` phonemization.

3. **F5-TTS Architecture Analysis & Flow-Matching Fine-Tuning** (*Soroush Soleimani*)
   - **Kaggle Architecture Breakdown**: [f5-tts-architecture-complete-explanation](https://www.kaggle.com/code/soroushsoleimani/f5-tts-architecture-complete-explanation)
   - **Kaggle Fine-Tuning**: [fine-tuning-f5-tts](https://www.kaggle.com/code/soroushsoleimani/fine-tuning-f5-tts)
   - **Audio Sample**: High-fidelity zero-shot studio synthesis demonstration.

4. **English TTS Engine with VITS Architecture** (*Melika Parhiz*)
   - **GitHub**: [melolikepz/English-TTS](https://github.com/melolikepz/English-TTS)
   - **Notebook**: `VITS_Local.ipynb` trained on LJSpeech-1.1 with MAS (Monotonic Alignment Search).

---

## 🚀 How to Publish to GitHub Pages

### Method A: Publish under your personal user domain (`<username>.github.io`)
1. Create a repository on GitHub named:
   - `SoroushSoleimani.github.io` (for Soroush) OR `melolikepz.github.io` (for Melika).
2. Inside this folder (`C:\Users\sorou\.gemini\antigravity\scratch\persian-tts-g2p-showcase`), open PowerShell or Terminal and initialize git:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Persian & English TTS/G2P showcase page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. Your site will automatically go live within 1–2 minutes at:
   `https://<your-username>.github.io`

---

### Method B: Publish as a Project Page (e.g. `https://<username>.github.io/tts-showcase/`)
1. Create a repository on GitHub with any name, e.g. `tts-showcase` or `persian-speech-lab`.
2. Push this directory:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Persian & English TTS/G2P showcase page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/tts-showcase.git
   git push -u origin main
   ```
3. In your GitHub repository:
   - Go to **Settings** &rarr; **Pages** (under Code and automation).
   - Under **Build and deployment**:
     - **Source**: `Deploy from a branch`
     - **Branch**: `main` / `/ (root)`
     - Click **Save**.
4. Your site will be published at:
   `https://<your-username>.github.io/tts-showcase/`

---

## 📁 Repository Structure

```text
.
├── index.html          # Clean, modern white-themed single-page website with embedded audio players
├── .nojekyll           # Bypasses Jekyll processing on GitHub Pages
├── README.md           # Documentation and deployment instructions
├── assets/             # Architecture diagrams and figures
│   └── persian_tts_g2p_architecture.png
└── audio/              # Playable .wav audio output samples
    ├── sentence1_before_finetune.wav
    ├── sentence1_after_finetune.wav
    ├── sentence2_before_finetune.wav
    ├── sentence2_after_finetune.wav
    ├── modele_amari_before_finetune.wav
    ├── modele_amari_after_finetune.wav
    ├── kaggle_sample.wav
    ├── sentence1_vits_high_mos.wav
    └── persian_g2p_output.wav
```

---

## 📄 License
This project is released under the **MIT License**.

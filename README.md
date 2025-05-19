
# 🗣️ Arabic Text-to-Speech (TTS) Model Benchmark

This project presents a comparative study and implementation of three modern Text-to-Speech (TTS) systems for Arabic: **Meta’s MMS**, **Coqui’s XTTS-v2**, and **Microsoft’s SpeechT5**. The goal is to evaluate their performance across Arabic dialects including MSA, Najdi, Hijazi, and Gulf.

---

## 📁 Repository Contents

| File Name                          | Description |
|-----------------------------------|-------------|
| `mms_tts_ara_model.ipynb`         | MMS TTS model for Arabic using Meta’s multilingual model |
| `xtts_v2.ipynb`                   | XTTS-v2 implementation using Coqui TTS for multilingual voice synthesis |
| `speecht5_tts_clartts_ar.ipynb`   | SpeechT5 implementation using HuggingFace Transformers for Arabic |
| `DEMO of the finalized model   `  | SpeechT5 implementation DEMO |
| `Xtts_outputs folder           `  | Evaluation and sample outputs from xtts model |
| `mms-tts-ara_outputs foler     `  | Evaluation and sample outputs from mms model |
| `speech t5 outputs  foler     `   | Evaluation and sample outputs from speech t5 model |

| `README_TTS_Models.md`            | Instructions and model overview (you’re reading it!) |

---

## 🧩 TTS Models Overview

### 1. Meta MMS
- **Notebook**: `mms_tts_ara_model.ipynb`
- **Model**: `facebook/mms-tts-ara`
- **Strength**: Low latency
- **Limitation**: Robotic output, lower naturalness

### 2. Coqui XTTS-v2
- **Notebook**: `xtts_v2.ipynb`
- **Model**: `tts_models/multilingual/multi-dataset/xtts_v2`
- **Strength**: Best naturalness and clarity across dialects
- **Limitation**: High latency due to model complexity

### 3. Microsoft SpeechT5
- **Notebook**: `speecht5_tts_clartts_ar.ipynb`
- **Model**: `microsoft/speecht5_tts`
- **Strength**: Balanced quality, good naturalness and clarity
- **Limitation**: Moderate latency

---

## 🔧 Setup Instructions

### ✅ Environment Requirements
- Python 3.8+
- Recommended: virtual environment (venv or conda)

### 📦 Install Dependencies

```bash
pip install torch torchaudio transformers soundfile scipy librosa gradio matplotlib
pip install git+https://github.com/huggingface/transformers.git
pip install TTS  # Required for XTTS-v2

# 🎤 Speech Emotion Recognition (SER)

This project is a **Speech Emotion Recognition system** built in **Google Colab**.  
It trains a deep learning model (CNN + LSTM) on the **RAVDESS dataset** and allows you to record your own speech and predict emotions directly in Colab.

---

## 🚀 Features
- Uses **MFCC audio features** extracted with Librosa.
- Trains on the **RAVDESS dataset** (8 emotions: neutral, calm, happy, sad, angry, fearful, disgust, surprised).
- Model: **Conv1D + LSTM + Dense layers** with dropout.
- Supports:
  - **Training** from scratch on RAVDESS.
  - **Evaluation** on test set.
  - **Prediction** on new audio files.
  - **Recording live speech** in Colab (short clips, then classification).

---

## 📂 Dataset
We use the **RAVDESS Emotional Speech Audio** dataset:

- Download link: [Zenodo – RAVDESS](https://zenodo.org/record/1188976)  
- The dataset contains 24 actors vocalizing different emotions.

---

## ⚙️ Installation
Run in Google Colab (recommended).  
Install dependencies:

```bash
!pip install librosa soundfile tensorflow keras scikit-learn matplotlib tqdm gradio

!wget https://zenodo.org/record/1188976/files/Audio_Speech_Actors_01-24.zip
!unzip -q Audio_Speech_Actors_01-24.zip -d ravdess


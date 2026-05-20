# Emotional_Mapping

📊 Emotion Detection from Video using NLP
📌 Overview

Project ini bertujuan untuk mendeteksi emosi dari video dengan pendekatan Natural Language Processing (NLP).

Alih-alih langsung menganalisis visual video, sistem ini:

Mengekstrak teks (speech/caption) dari video
Mengolah teks tersebut menggunakan teknik NLP
Mengklasifikasikan emosi berdasarkan isi teks
🗂️ Dataset

Dataset berbentuk CSV dengan format:

id,video,emotion
1,https://www.instagram.com/reel/xxx,Surprise
2,https://www.instagram.com/reel/yyy,Surprise

📌 Penjelasan Kolom

id → ID unik data
video → Link video (Instagram Reels)
emotion → Label emosi (ground truth)
⚙️ Pipeline Sistem
🔹 1. Video Input
Mengambil video dari URL (Instagram Reels)
🔹 2. Text Extraction
Ekstraksi teks dari video menggunakan:
Speech-to-Text (audio → teks)
atau caption/overlay text (jika ada)
🔹 3. Text Preprocessing
Lowercasing
Stopword removal
Tokenization
Cleaning noise (URL, simbol, dll)
🔹 4. NLP Processing
Feature extraction:
TF-IDF / Embedding
Model:
Machine Learning / Deep Learning
🔹 5. Emotion Classification
Output berupa label emosi:
Surprise
Happy
Sad
Angry
dll

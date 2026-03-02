Audio Grammar Scoring
📌 Project Description

This project predicts the grammar quality of spoken English from audio recordings.

The system takes an audio file as input and gives a score from:

👉 1 (Poor grammar) to 5 (Good grammar)

Built for the SHL Audio Grammar Scoring Challenge.

🧠 How It Works
Audio → Extract Features → Machine Learning Model → Score

The model learns from speech patterns like fluency, pauses, and clarity.

🎤 Features Used

The following audio features are extracted:

MFCC (speech features)

Pitch and energy

Speech duration

Model Used

LightGBM Regressor

Used to predict the grammar score from audio features.

Dataset
dataset/
 ├── audios/
 │     ├── train/
 │     └── test/
 │
 └── csvs/
       ├── train.csv
       └── test.csv

train.csv → audio filenames + scores

test.csv → audio filenames

Output

The program generates:

submission.csv

Format:

filename,label
audio_1,3.2
audio_2,4.1

Zero Crossing Rate

These help measure speaking quality.

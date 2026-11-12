# 📰 Emotion-Aware Fake News Detection on Social Media using AI

An AI-powered fake news detection framework that combines textual representations, speaker credibility, and emotion-based features to identify misleading and deceptive information on social media.

## Overview

Fake news on social media spreads rapidly and can influence public opinion, create misinformation, and affect decision-making. Traditional detection approaches primarily focus on textual patterns, often overlooking the emotional characteristics and credibility of the information source.

This project explores an **Emotion-Aware Feature Fusion Framework** that integrates textual meaning, speaker credibility, and emotional signals to improve fake news classification.

The framework uses Natural Language Processing (NLP) and Deep Learning techniques to analyze news statements and classify them based on their credibility.

## Key Features

- **Textual Feature Extraction:** Extract contextual and semantic information from news statements.
- **Emotion Analysis:** Identify emotional signals using the NRC Emotion Lexicon.
- **Speaker Credibility:** Incorporate speaker-related information to provide additional context.
- **Feature Fusion:** Combine textual, emotional, and credibility representations.
- **Deep Learning Models:** Experiment with CNN, RNN, LSTM, and BERT-based architectures.
- **Performance Evaluation:** Evaluate models using standard classification metrics.

## Dataset

**LIAR Dataset**

The project uses the LIAR benchmark dataset, which contains manually labeled short statements collected from PolitiFact.

The dataset includes information such as:

- News statement
- Speaker information
- Speaker's political and demographic context
- Subject and context
- Truthfulness labels

The original LIAR dataset contains six classification labels:

| Label | Description |
|---|---|
| Pants-fire | Completely false |
| False | False statement |
| Barely-true | Mostly false |
| Half-true | Partially true |
| Mostly-true | Mostly true |
| True | True statement |

## Methodology

The proposed framework follows an emotion-aware feature fusion approach.

### 1. Text Preprocessing

- Remove missing and invalid records.
- Clean and normalize textual data.
- Tokenize news statements.
- Apply padding and sequence preparation.
- Generate contextual text representations.

### 2. Textual Feature Extraction

Textual representations are generated using NLP techniques and embedding-based approaches to capture semantic and contextual information.

### 3. Emotion Feature Extraction

The NRC Emotion Lexicon is used to identify emotional associations in news statements.

The emotion categories include:

- Anger
- Anticipation
- Disgust
- Fear
- Joy
- Sadness
- Surprise
- Trust

### 4. Speaker Credibility Analysis

Speaker-related information is incorporated to provide contextual credibility signals for the news statements.

### 5. Emotion-Aware Feature Fusion

Textual, emotional, and speaker credibility representations are integrated into a unified framework for classification.

### 6. Classification

The fused representations are used by different deep learning architectures to classify news statements.

## Models Implemented

| Model | Description |
|---|---|
| CNN | Captures local textual patterns |
| RNN | Processes sequential textual information |
| LSTM | Learns long-term dependencies in text |
| BERT | Captures contextual and bidirectional language representations |

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Environment | Jupyter Notebook / Google Colab |
| NLP | NLTK, Tokenization |
| Deep Learning | TensorFlow / Keras |
| Transformer Models | BERT, Hugging Face |
| Feature Extraction | NRC Emotion Lexicon |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Evaluation | Scikit-learn |

## Project Workflow

```text
       LIAR Dataset
             |
             v
      Text Preprocessing
             |
             v
    Feature Extraction
             |
       +-----+------+
       |      |     |
       v      v     v
     Text  Emotion Speaker
   Features Features Credibility
       |      |     |
       +------+-----+
             |
             v
      Feature Fusion
             |
             v
     Deep Learning Models
       CNN / RNN / LSTM
             |
        BERT Model
             |
             v
    Fake News Classification
             |
             v
     Performance Evaluation
```

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics help assess classification performance and compare the effectiveness of different model architectures.

## Project Structure

```text
Fake-News-Detection/
│
├── dataset/
│   └── liar_dataset/
│
├── notebooks/
│   ├── data_preprocessing.ipynb
│   ├── emotion_extraction.ipynb
│   ├── cnn_model.ipynb
│   ├── rnn_model.ipynb
│   ├── lstm_model.ipynb
│   └── bert_model.ipynb
│
├── results/
│   └── evaluation_results/
│
├── README.md
└── requirements.txt
```

*Note: The directory structure is illustrative. Adjust it according to the actual repository.*

## Research Contribution

This project investigates the integration of emotional information and speaker credibility with contextual textual representations for fake news detection.

Rather than relying exclusively on textual features, the proposed framework explores how emotion-aware feature fusion can provide additional information for identifying potentially misleading news statements.

## Future Scope

- Explore advanced transformer architectures.
- Improve contextual emotion representation.
- Investigate explainable AI techniques for classification decisions.
- Evaluate the framework on additional misinformation datasets.
- Explore real-time fake news detection on social media platforms.

## Research Publication

This work is based on the research paper:

**An Affective Feature Fusion Framework for Fake News Detection on the LIAR Benchmark**

Presented at the **3rd IEEE International Conference on Women in Computing (InCoWoCo 2026)**.

---

## License

This project is intended for academic and research purposes. Please refer to the dataset's original licensing and usage terms before redistribution.
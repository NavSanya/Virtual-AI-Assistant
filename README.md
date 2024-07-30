# Virtual-AI-Assistant

### General Idea
* Initialize and Setup
* Listen for Voice Input
* Process Voice Input using AI
* Generate AI-based Response
* Convert Text to Speech
* Output Audio Response

## Flow Chart
```
+----------------------+       +-------------------------+
|                      |       |                         |
|  Initialize & Setup  +------>+  Listen for Voice Input |
|                      |       |                         |
+----------+-----------+       +-----------+-------------+
           |                           |
           |                           v
           |                +----------+-----------+
           |                |                      |
           |                |  Convert Audio to    |
           |                |         Text         |
           |                |                      |
           |                +----------+-----------+
           |                           |
           |                           v
           |                +----------+-----------+
           |                |                      |
           |                |  Process Voice Input |
           |                |        using AI      |
           |                |                      |
           |                +----------+-----------+
           |                           |
           |                           v
           |                +----------+-----------+
           |                |                      |
           v                |  Generate AI-based   |
+----------+-----------+    |        Response      |
|                      |    |                      |
| Convert Text to      |    +----------+-----------+
| Speech               +--------------->|
|                      |                v
+----------------------+    +-----------+----------+
                            |                      |
                            |  Output Audio        |
                            |      Response        |
                            |                      |
                            +----------------------+


```

### Contexual Emotion Reader
Step 1: Collect Datasets
* Emotion Detection from Text: https://www.kaggle.com/datasets/pashupatigupta/emotion-detection-from-text/data 
* Emotion Detection Dataset (Audio): https://www.kaggle.com/datasets/ritika0111/emotion-detection-dataset

Step 2: Preprocess the Datasets
* Text Preprocessing
    * Tokenization: Break down the text into tokens (words or subwords).
    * Normalization: Convert text to lowercase, remove punctuation, and handle contractions.
    * Annotation: Extract sentences and annotate them with corresponding emotions.
* Audio Preprocessing
    * Feature Extraction: Extract audio features such as Mel-frequency cepstral coefficients (MFCCs), spectrograms, and chroma features.
    * Segmentation: Divide audio files into segments corresponding to individual sentences or phrases.
    * Annotation: Annotate audio segments with corresponding emotions.

Step 3: Train Emotion Detection Models
* Text Emotion Detection Model
    * Model Selection: Choose a pre-trained language model such as BERT or RoBERTa.
    * Fine-Tuning: Fine-tune the model on the datasets for emotion classification.

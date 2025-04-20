# English to Arabic Translation System

A neural machine translation system that translates English text to Arabic using both custom neural networks and pre-trained transformer models.

## Project Overview

This project implements two different approaches for English to Arabic translation:

1. **Custom Neural Network Model**:
   - Bidirectional GRU layers with embedding
   - Training on parallel English-Arabic corpus

2. **Pre-trained Transformer Model**:
   - Utilizing Hugging Face's transformer models
   - Fine-tuned model for English to Arabic translation

## Installation
  - Clone the Repository
```bash
git clone https://github.com/Abdelrahman-Elshahed/English-Arabic-NLP-Translator.git
cd English-Arabic-NLP-Translator
```
  - Install Python dependencies:
  ```bash
  pip install -r requirements.txt
  ```
## Dataset
The project uses a parallel English-Arabic corpus `(ara_eng.txt)`, with tab-separated values containing English sentences and their Arabic translations.

## Model Architecture
- Custom Neural Network
  - Embedding layer
  - Bidirectional GRU with 256 units
  - Dropout (0.5) for regularization
  - Dense output layer with softmax activation
- Transformer Model
  - Pre-trained Seq2Seq model from Hugging Face
  - Model: "Shularp/model-translate-en-to-ar-from-120k-dataset-ar-en-th230111447"
## Results
The notebook includes visualizations of training and validation accuracy over 7 epochs, allowing for performance comparison between the custom model and the pre-trained transformer.

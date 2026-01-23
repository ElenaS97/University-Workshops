# English-to-Russian Neural Machine Translation (Seq2Seq)
*Deep Learning Project using LSTM & GRU Architectures*

## Project Overview
This project implements a **Sequence-to-Sequence (Seq2Seq)** model to translate English phrases into Russian. It demonstrates advanced Natural Language Processing (NLP) techniques by building a character-level Encoder-Decoder architecture from scratch.

## Dataset
The model was trained on the Russian-English sentence pairs provided by [Tatoeba](https://www.manythings.org/anki/), hosted by ManyThings.org.

## Model Architectures
I implemented and compared two Recurrent Neural Network (RNN) approaches:
1.  **LSTM (Long Short-Term Memory):** Handles long-range dependencies in text.
2.  **GRU (Gated Recurrent Unit):** A more efficient variant of LSTM.

## Performance Results
| Model | Training Accuracy | Validation Accuracy | Training Time (approx) |
| :--- | :--- | :--- | :--- |
| **LSTM** | **96.3%** | **88.2%** | ~42s / epoch |
| GRU | 95.8% | 88.9% | ~41s / epoch |

## Tech Stack
* **Framework:** TensorFlow / Keras
* **Techniques:** Encoder-Decoder, Character-level Embedding, Softmax Activation.
* **Data Processing:** Vectorization of 10,000+ sentence pairs.

## Example Translations
The model generates translations character-by-character:
* **Input:** "Hi." -> **Output:** "Здрасте." (Correct informal greeting)
* **Input:** "Run!" -> **Output:** "Беги!" (Correct imperative form)

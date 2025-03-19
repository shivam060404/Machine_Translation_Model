# Neural Machine Translation Model

## Project Overview
This project implements a sequence-to-sequence neural machine translation (NMT) model that translates English sentences to French. The model uses an encoder-decoder architecture with LSTM networks and attention mechanisms to learn the mapping between languages.

## Features
- English to French translation capability
- Encoder-decoder architecture with LSTM cells
- Word embedding using pre-trained vectors
- Sequence padding for variable-length inputs
- Interactive translation testing mode

## Dataset
The model uses the English-French dataset from the Tatoeba Project, accessible through the Anki format. The dataset consists of pairs of English sentences and their French translations.

## Model Architecture
- **Encoder**: LSTM network that processes the input English sentence
- **Decoder**: LSTM network that generates the French translation
- **Embedding Layer**: Pre-trained word vectors to represent words semantically
- **Dense Layer**: Output layer with softmax activation for word prediction

## Requirements
- TensorFlow 2.0+
- NumPy
- Matplotlib
- Python 3.6+

## Setup Instructions
1. Clone this repository
2. Install the required packages:
   ```
   pip install tensorflow numpy matplotlib
   ```
3. Run the script:
   ```
   python machine_translation_model.py
   ```

## Usage
The model provides an interactive mode for testing translations. After training, you can input English sentences and receive French translations.

## Performance
The model is trained for 5 epochs with a batch size of 64, achieving reasonable translation quality for simple sentences. The training process monitors loss and accuracy metrics.

## Limitations
- Limited vocabulary (20,000 words)
- Maximum sequence length of 100 tokens
- Training sample size of 10,000 sentences
- Basic handling of unknown words

## Future Improvements
- Implement attention mechanisms
- Increase vocabulary size
- Use bidirectional encoder LSTMs
- Implement beam search for better translations
- Add more language pairs

## License
MIT License 

## Acknowledgments
- Tatoeba Project for the language dataset
- TensorFlow team for the deep learning framework

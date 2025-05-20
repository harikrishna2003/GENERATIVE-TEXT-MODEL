COMPANY: CODETECH IT SOLUTIONS
NAME: HARIKRISHNA PILLAI
INTERN ID: C0DF49
DOMAIN: ARTIFICIAL INTELLIGENCE
DURATION: 4 WEEKS
MENTOR: NEELA SANTOSH



# 📖 Text Generation with GPT-2 and LSTM

A Python-based project demonstrating two approaches to text generation:  
1. **GPT-2** (Transformer-based) for high-quality, context-aware text.  
2. **LSTM** (RNN-based) for simpler, sequential text prediction.  

## Features
- **GPT-2 Implementation**:
  - Loads pre-trained `gpt2` from Hugging Face Transformers.
  - Generates text with configurable sampling (`top_k`, `temperature`).
- **LSTM Implementation**:
  - Trains a custom LSTM model on a small corpus.
  - Predicts next words using token sequences.
- **User-Friendly**:
  - Example prompts included (e.g., `"The importance of biodiversity"`).
  - Handles GPU/CPU compatibility (disables GPU if unavailable).

## Technologies Used
- **Python** (Core language)
- **PyTorch** (GPT-2 model loading/inference)
- **TensorFlow/Keras** (LSTM model)
- **Hugging Face Transformers** (GPT-2 tokenizer and model)
- **NLTK/Tokenizer** (Text preprocessing for LSTM)

## How It Works
### GPT-2
1. **Model Load**: Uses `GPT2LMHeadModel` and `GPT2Tokenizer`.
2. **Text Generation**:  
   - Encodes input prompt.  
   - Generates text with `model.generate()` (supports sampling for diversity).  

### LSTM
1. **Data Prep**:  
   - Tokenizes a custom corpus.  
   - Creates n-gram sequences for training.  
2. **Model**:  
   - Embedding → LSTM → Dense layers.  
   - Predicts next word probabilities.  
3. **Inference**:  
   - Seed text → Preprocess → Predict next words iteratively.  

## Installation
```bash
git clone https://github.com/yourusername/text-generation.git
cd text-generation
pip install -r requirements.txt

# Chinese-to-English Neural Machine Translation System

## Project Description
This repository implements two neural network architectures for Chinese-to-English translation:
1. Sequence-to-sequence model with attention mechanism
2. GPT-style transformer decoder model

Trained on ~30,000 parallel sentences from tatoeba.org (CC-BY 2.0 France license).

## Quick Start
```bash
# Install dependencies
pip install -r requirements.txt

# Run the Jupyter notebook
jupyter notebook 122090791_partA_s2s.ipynb # Sequence-to-sequence model with attention mechanism
jupyter notebook 122090791_partA_gpt.ipynb # GPT-style transformer decoder model
```

## Data Format
Input file (cmn-eng.txt) should be tab-separated with format:

English sentence<TAB>Chinese sentence<TAB>Attribution
Example: 
Hello<TAB>你好<TAB>CC-BY 2.0 (user123)

## Model Details
### Seq2Seq with Attention
​Architecture: Bidirectional GRU encoder + Attention decoder
​Parameters:
Hidden size: 256
Embedding dim: 256
Dropout: 0.1
​Training:
Epochs: 128
Batch size: 32
Learning rate: 0.001
### GPT-style Model
​Architecture: 4-layer transformer decoder
​Parameters:
Hidden size: 256
Attention heads: 8
Max length: 1024
​Training:
Epochs: 128
Batch size: 16
Learning rate: 1e-4

Contact
For questions or contributions:

Email: zhengyizhao@link.cuhk.edu.cn
# 📖 Introduction

[**spaCy**](https://spacy.io) is a free, open-source library for advanced Natural Language Processing (NLP) in Python. The library have a lot of pre-trained models for many languages.

<p align="center">
    <img src="https://spacy.io/images/architecture.svg" width=400>
</p>

## Processing Pipeline

<p align="center">
    <img src="https://spacy.io/images/pipeline.svg" width=600>
</p>

## Vocab, Hashes and Lexemes

<p align="center">
    <img src="https://spacy.io/images/vocab_stringstore.svg" width=600>
</p>

# Installation

```bash
pip3 install spacy
```

## Downloading Models

```bash
python3 -m spacy download "en_core_web_lg"
```

- `"sm"` - small model
- `"md"` - medium model
- `"lg"` - large model
- `"trf"` - transformer model

# Usage

```python
spacy.load("en_core_web_lg")
```

# References

- [**🌐 spaCy**](https://spacy.io)
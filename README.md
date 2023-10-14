# 📖 Introduction

This repository contains my studies about **Natural Language Processing (NLP)**. I will study the theory and practice of NLP.

My name is **Matheus Diniz**, and I am a student at Universidade Federal do Rio Grande do Norte (UFRN). If you want to know more about me, check out:

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/dinizmaths)
[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DinizMaths)

## 📝 What is NLP?

Natural Language Processing (NLP) is an implementation of functionalities of **Machine Learning (ML)** that enables computers to "understand" and process human language. Translation, sentiment analysis, speech recognition, and topic segmentation are examples of NLP.

This area of study is on a constant rise and extremely hard. This is why currently the most part of advancements in NLP are made by **Artificial Intelligence (AI)**.

## 📝 Why NLP is hard?

The language is **ambiguous**. The same word can have different meanings depending on the context. For example, the word _"bank"_ can mean a financial institution or a river bank.

Other problem is **irony**. The same sentence can have different meanings depending on the context. For example, the sentence _"He studied by 10 minutes, certainly will pass in the exam"_ can be ironic or not depending on the context.

And, at last, the language is **dynamic**. New words are created and old words are forgotten all the time.

## 📝 Applications of NLP

The applications of NLP are countless. Here are some examples:

- Translation
- Sentiment Analysis
- Speech Recognition
- Topic Segmentation
- Question Answering
- Text Summarization
- Text Generation and Prediction
- Text Classification
- Chatbots

## 📝 NLP Concepts

In this section, we will see some concepts of NLP.

### 💭 Corpus

Corpus is a collection of texts (non-structured) in natural language. It can be a collection of books, articles, tweets, etc.

### 💭 Annotations

Annotations are a technique to locate and classify elements in a text. Usually, they are specific in a domain. For example, in the domain of medicine, annotations can be used to locate and classify diseases, symptoms, and treatments in a text.

We have specialized tools to do annotations, like:

[**🌐 Brat**](http://brat.nlplab.org/)

[**🌐 Doccano**](https://doccano.herokuapp.com)

### 💭 Tokenization

Tokenization is the process of breaking a text into tokens. A token is a sequence of characters that represents a unit of information. For example, the sentence _"I love pizza"_ can be tokenized into the tokens _"I"_, _"love"_, and _"pizza"_.

### 💭 Part-of-Speech Tagging (POS Tagging)

Part-of-Speech Tagging is the process of marking up a word in a text as corresponding to a particular part of speech. For example, the sentence _"I love pizza"_ can be tagged as:

| PRON | VERB   | NOUN    |
| ---- | ------ | ------- |
| _I_  | _love_ | _pizza_ |

### 💭 Lemmatizing (Lemma)

Lemmatizing is the process of grouping together the different inflected forms of a word so they can be analyzed as a single item. For example, the words _"go"_, _"goes"_, and _"went"_ can be lemmatized as _"go"_.

### 💭 Stemming (Stem)

Stemming is the process of reducing inflected (or sometimes derived) words to their word stem, base or root form. For example, the words _"program"_, _"programs"_, _"programmer"_ and _"programming"_ can be stemmed as _"program"_.

### 💭 Dependency Parsing

Dependency Parsing is the process of analyzing the grammatical structure of a sentence based on the dependencies between the words in a sentence. For example, the sentence _"Our lives are controlled by algorithms"_ can be parsed as:

<center>
    <img src="./images/parsing.png" alt="Dependency Parsing" width="200"/>
</center>

### 💭 NGRAM

NGRAM is a contiguous sequence of n items from a given sample of text or speech. For example, the sentence _"I love pizza"_ can be tokenized into the BIGRAMS _"I love"_ and _"love pizza"_.

Generally, we use **BIGRAMS** and **TRIGRAMS**, four or more grams are rare because they are too sparse.

# 🎯 Projects

[**💻 Project 01 - Text Classification**](./Project_01)

# 📦 Instalation

To clone this repository, use:

```bash
git clone https://github.com/DinizMaths/natural-language-processing.git
```

Each project has its own dependencies. To install them, cahnge to the project directory and use:

```bash
pip install -r requirements.txt
```

Example:

```bash
cd Project_01
pip install -r requirements.txt
```


# 📚 References

[**🌐 Formação Processamento de Linguagem Natural: NLP [2023]**](https://www.udemy.com/course/formacao-processamento-de-linguagem-natural-nlp/)


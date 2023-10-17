# 📖 Introduction

This repository contains my studies about **Natural Language Processing (NLP)**. I will study the theory and practice of NLP.

My name is **Matheus Diniz**, and I am a student at Universidade Federal do Rio Grande do Norte (UFRN). If you want to know more about me, check out:

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dinizmaths)
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

&nbsp;
&nbsp;
<p align="center">
  <img src="./images/parsing.png" alt="Dependency Parsing" width="200"/>
</p>
&nbsp;

### 💭 NGRAM

NGRAM is a contiguous sequence of n items from a given sample of text or speech. For example, the sentence _"I love pizza"_ can be tokenized into the BIGRAMS _"I love"_ and _"love pizza"_.

Generally, we use **BIGRAMS** and **TRIGRAMS**, four or more grams are rare because they are too sparse.

## 📝 NLP Word Embedding

Computers are capable of processing only numbers, they don't handle very well with non-strucutred data like text. So, we need to convert text into numbers, non-structured data into structured data. This process is called **Word Embedding**.

Word Embedding is the collective name for a set of language modeling and feature learning techniques in NLP where words or phrases from the vocabulary are mapped to vectors of real numbers.

### 💭 One-Hot Encoding

One-Hot Encoding is a process of converting a sentence into a matrix of 0s and 1s. Each row of the matrix represents a word in the sentence, and each column represents a word in the vocabulary. For example, the sentence _"Our lives are controlled by algorithms"_ can be encoded as:

|            | algorithms | are | by | Our | controlled | lives |
| ---------- | ---------- | --- | -- | --- | ---------- | ----- |
| Our        | 0          | 0   | 0  | 1   | 0          | 0     |
| lives      | 0          | 0   | 0  | 0   | 0          | 1     |
| are        | 0          | 1   | 0  | 0   | 0          | 0     |
| controlled | 0          | 0   | 0  | 0   | 1          | 0     |
| by         | 0          | 0   | 1  | 0   | 0          | 0     |
| algorithms | 1          | 0   | 0  | 0   | 0          | 0     |

One of the highest problems of One-Hot Encoding is the **sparsity**. The matrix is very sparse, because the number of words in the vocabulary is much higher than the number of words in a sentence.

### 💭 TF-IDF (Term Frequency - Inverse Document Frequency)

TF-IDF is a process of representing a sentence by the frequency of the words. In a juridical process, for example, the words _"process"_ and _"law"_ are more frequent than the words _"banana"_ and _"pineapple"_. So, the words _"process"_ and _"law"_ will have a higher **weight** than the words _"banana"_ and _"pineapple"_.

In a scenario that we have to choose what process is of a ambiental área:
- Document 01: The word _"ambiental"_ appears 0 times.
- Document 02: The word _"ambiental"_ appears 3 times.
- Document 03: The word _"ambiental"_ appears 9 times.

We have two ways to calculate the weight of the word _"ambiental"_:
- TF(_"ambiental"_) = (Number of times that _"ambiental"_ appears in the document) / (Number of words in the document)
- TF(_"ambiental"_) = (Number of times that _"ambiental"_ appears in the document) / (Number of times that the most frequent word appears in the document)

Supose we choose the second way and in all documents the most frequent word appears 10 times. Now, the IDF(_"ambiental"_) is calculated as:

- [Smooth IDF = True] IDF(_"ambiental"_) = $ln\left(\frac{1 + \text{Number of documents}}{1 + \text{Number of documents that ambiental appears}}\right ) + 1$
- [Smooth IDF = False] IDF(_"ambiental"_) = $ln\left(\frac{\text{Number of documents}}{\text{Number of documents that ambiental appears}}\right ) + 1$

Supose we choose the second way. Now, the TF-IDF(_"ambiental"_) is calculated as:

|             | TF         | IDF             | TF-IDF          |
| ----------- | ---------- | --------------- | --------------- |
| Document 01 | 0/10 = 0.0 | ln(3/2) = 1.405 | TF * IDF = 0.00 |
| Document 02 | 3/10 = 0.3 | ln(3/2) = 1.405 | TF * IDF = 0.42 |
| Document 03 | 9/10 = 0.9 | ln(3/2) = 1.405 | TF * IDF = 1.26 |

So, the term _"ambiental"_ has more associated to the document 03.

### 💭 Word2Vec

By a process of training, produces a vector that represents the relation between the words. There are two main ways:

- CBOW (Continuous Bag of Words)

    Predict a central word based on the context.

- Skip-Gram

    Predict the context based on a central word.

So, the result is a representation of the word in a vector space.

### 💭 Other Ways

- FastText
- GloVe (Global Vectors for Word Representation)
- BERT (Bidirectional Encoder Representations from Transformers)

## 📝 NLP Pipelines

A pipeline is a sequence of steps that are executed to solve a problem. There are many ways to build a NLP pipeline, but one of the most common is:

1. **Data Collection**

    Collect the data from the source. Can be a **Digital Document**, **Database**, **Cloud**, **OCR** (Optical Character Recognition), **Web Scraping**, etc.

2. **Data Preprocessing**

    Prepare the data to be used in the model. Using techniques like we saw on the section **📝 NLP Concepts**.

3. **Text Representation**

    Represent the text in a numerical way. Using techniques like we saw on the section **📝 NLP Word Embedding**.

4. **Model Training**

    - Train the model
    - Evaluate the model
    - Tunne the model

5. **Deploy**

    Deploy the model. Can be a **Web Application**, **API**, **Mobile Application**, **Desktop Application**, etc.

# 🗂️ Folders

[**💻 NLP With spaCy**](./nlp_with_spacy)


# 📦 Instalation

To clone this repository, use:

```bash
git clone https://github.com/DinizMaths/natural-language-processing.git
```

Each project has its own dependencies. To install them (I recommend using a virtual environment), change to the project directory and use:

```bash
pip install -r requirements.txt
```

Example:

```bash
cd nlp_with_spacy
pip install -r requirements.txt
```

# 📚 References

[**🌐 Formação Processamento de Linguagem Natural: NLP [2023]**](https://www.udemy.com/course/formacao-processamento-de-linguagem-natural-nlp/)

[**🌐 TF-IDF — algoritmo de recomendação**](https://medium.com/data-hackers/tf-idf-algoritmo-de-recomendação-6c3cbd55e439)
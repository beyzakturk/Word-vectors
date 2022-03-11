# Word vectors

A Beginner’s Guide to Word Embedding with Gensim Word2Vec Model

![Image of NLP](https://www.erdempsikiyatri.com/upload/sayfa_resimleri/nlp-nedir_75.jpg)

Word embedding is one of the most important techniques in natural language processing(NLP), where words are mapped to vectors of real numbers. Word embedding is capable of capturing the meaning of a word in a document, semantic and syntactic similarity, relation with other words. It also has been widely used for recommender systems and text classification. This tutorial will show a brief introduction of genism word2vec model with an example of generating word embedding for the vehicle make model.

## Introduction of Word2vec

Word2vec is one of the most popular technique to learn word embeddings using a two-layer neural network. Its input is a text corpus and its output is a set of vectors. Word embedding via word2vec can make natural language computer-readable, then further implementation of mathematical operations on words can be used to detect their similarities. A well-trained set of word vectors will place similar words close to each other in that space. For instance, the words women, men, and human might cluster in one corner, while yellow, red and blue cluster together in another.

![Image of NLP](https://miro.medium.com/max/1400/1*HmmFCZpKk3i4EvMYZ855tg.png)

There are two main training algorithms for word2vec, one is the continuous bag of words(CBOW), another is called skip-gram. The major difference between these two methods is that CBOW is using context to predict a target word while skip-gram is using a word to predict a target context. Generally, the skip-gram method can have a better performance compared with CBOW method, for it can capture two semantics for a single word. For instance, it will have two vector representations for Apple, one for the company and another for the fruit. For more details about the word2vec algorithm

## Gensim Python Library Introduction

Gensim is an open source python library for natural language processing and it was developed and is maintained by the Czech natural language processing researcher Radim Řehůřek. Gensim library will enable us to develop word embeddings by training our own word2vec models on a custom corpus either with CBOW of skip-grams algorithms.

At first, we need to install the genism package. Gensim runs on Linux, Windows and Mac OS X, and should run on any other platform that supports Python 2.7+ and NumPy. Gensim depends on the following software:
- Python >= 2.7 (tested with versions 2.7, 3.5 and 3.6)
- NumPy >= 1.11.3
- SciPy >= 0.18.1
- Six >= 1.5.0
- smart_open >= 1.2.1

There are two ways for installation. We could run the following code in our terminal to install genism package.
```
pip install --upgrade gensim
```
Or, alternatively for Conda environments:
```
conda install -c conda-forge gensim
```

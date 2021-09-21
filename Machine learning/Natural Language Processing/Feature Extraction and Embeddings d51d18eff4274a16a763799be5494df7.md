# Feature Extraction and Embeddings

Statistics of text data → to compare different text to each other

Get feature of individual words → (to build a knowledge graph)?

# Bag of Words

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled.png)

## Creating a Vector representation of each document in the corpus

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%201.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%201.png)

## How to compare two sentences?

Dot poduct? → not great, it doesnt take the differences into account

Think of sentences as vectors! → then check how big the angle difference is between the vectors! Genious

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%202.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%202.png)

Cosine similarity is also great, because it is automatically normalized between -1 and 1.

## Document frequency

How to get word uniqueness of a sentence in a corpus? Words that only appear once will get a higher score, because we normalize it according to how many of those words exist in the corpus.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%203.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%203.png)

## TF-IDF (Term Frequency - Inverse Document Frequency)

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%204.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%204.png)

# Single Words

## One-Hot Encoding

Similarly to how we encoded bag of words, but instead for individual words.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%205.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%205.png)

## Word Embeddings - Word2Vec

Transforms words to vectors.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%206.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%206.png)

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%207.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%207.png)

We take the hidden layer and say that is the representation of the word.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%208.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%208.png)

## GloVe

## Co-occurrence Probabilities

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%209.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%209.png)

# Embeddings

## Distributional Hypothesis

Words that occur in the same context have similar meanings.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2010.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2010.png)

Just like with Computer Vision, we can use pretrained layers for embeddings.

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2011.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2011.png)

## t-SNE - visualizing word embeddings

A very useful tool to see what the network learns, it visualizes clusters. Great for debugging.

It is like Principle Component Analysis, with one difference: it keeps similar objects similarly together. It preserves the linear substructures that has been learned by the embedding model (like word2vec)

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2012.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2012.png)

It can also be used with images:

![Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2013.png](Feature%20Extraction%20and%20Embeddings%20d51d18eff4274a16a763799be5494df7/Untitled%2013.png)
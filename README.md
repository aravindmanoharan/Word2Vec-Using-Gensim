# Word2Vec-Using-Gensim

This is an implementation of Word2Vec model using Gensim on Game of Thrones corpora.

Word2vec is a very popular Natural Language Processing technique, that uses a neural network to learn the vector representations of words called "word embeddings" in a particular text.

After training the Word2Vec model, we will use t-Distributed Stochastic Neighbor Embedding (t-SNE) from sklearn to visualize the learned embeddings vectors.

## Dataset

Here, the Word2Vec model is trained on the Game of thrones corpora which consists of five books of Game of Thrones. Each corpus has been preprocessed to extract only the tokens and removed all the stopwords. 

## Requirements

This Word2Vec model is implemented using [Gensim](https://radimrehurek.com/gensim/install.html) Packages.

```
pip install --upgrade gensim
```

Please check the requirements.txt file for all the packages which you need to install. Most of the packages can be installed using the pip package manager.

## Training the model

The model is trained for 50 epochs for 5 times and the sentences in the corpora are shuffled for each time. After training the model, let's see some of the results.

```
model.wv.most_similar('stark')
```
<p align="left">
  <img width="325" alt="screen shot 2018-09-11 at 9 47 38 pm" src="https://user-images.githubusercontent.com/35612880/45402867-cc678800-b60c-11e8-87f4-ecc574bf049d.png">
</p>

```
model.wv.most_similar('aerys')
```
<p align="left">
  <img width="358" alt="screen shot 2018-09-11 at 9 48 05 pm" src="https://user-images.githubusercontent.com/35612880/45402910-f6b94580-b60c-11e8-8d51-9263fefa6b28.png">
</p>

## Model Visualization

We visualize the learned embeddings using t-SNE. It is a tool for data visualization that reduces the dimensionality of data to 2 or 3 dimensions so that it can be plotted easily.

Let's visualize the entire data

<p align="center">
  <img width="994" alt="screen shot 2018-09-11 at 9 56 09 pm" src="https://user-images.githubusercontent.com/35612880/45403120-b27a7500-b60d-11e8-80fc-e601554fa6bb.png">
</p>

Let's visualize a particular bag of words

<p align="center">
  <img width="661" alt="screen shot 2018-09-11 at 9 57 05 pm" src="https://user-images.githubusercontent.com/35612880/45403153-dd64c900-b60d-11e8-82a0-e8bacd9622ef.png">
</p>

## Discussion

Word2Vec model can be an important process in Deep Learning where each text can be represented in the form of word embeddings so that deep neural network can understand better.

## Have questions? Need help with the code?

If you're having issues with or have questions about the code, [file an issue](https://github.com/aravindmanoharan/Word2Vec-Using-Gensim/issues) in this repository so that I can get back to you soon.

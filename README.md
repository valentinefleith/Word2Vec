## Word2Vec

Development of a Word2Vec neural network using the CBOW technique from scratch with PyTorch to generate word embeddings for word prediction.

### CBOW Model Architecture

The CBOW model consists of three layers:

1. **Input Layer**: This layer takes the contexts.
2. **Hidden Layer**: Also called the *embedding layer*, it is used to learn word embeddings. The number of neurons is the same as the number of words in the vocabulary since each neuron represents a word.
3. **Output Layer**: This layer predicts the target word according to its context.

Here is a visual representation of the architecture:

![image](https://github.com/valentinefleith/Word2Vec/assets/125041345/c2dbae4e-3c87-4994-abd5-f5c2422a4d95)


Source: [Understanding the Continuous Bag of Words (CBOW) Model Architecture](https://medium.com/@codethulo/understanding-the-continuous-bag-of-words-cbow-model-architecture-working-mechanism-and-math-78c7284a8d5a)

### Expected results

Since the `Word2Vec` method is based on predicting a word by its surrounding ones, it can be expected that words that appear in similar context would have similar embeddings as well. The expected relations between those words are the following:


- king - man ≈ queen - woman
- king - queen ≈ man - woman

Here is a representation of what the expected output could look like after performing a PCA reduction :

![image](https://github.com/valentinefleith/Word2Vec/assets/125041345/3bf9747e-dec3-4926-b679-bdc455afab87)


Source : [https://www.researchgate.net/figure/The-classical-king-woman-man-queen-example-of-neural-word-embeddings-in-2D-It\_fig1\_332679657](https://www.researchgate.net/figure/The-classical-king-woman-man-queen-example-of-neural-word-embeddings-in-2D-It_fig1_332679657).

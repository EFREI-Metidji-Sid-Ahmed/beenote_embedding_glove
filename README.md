## GloVe: Global Vectors for Word Representation

File  | Usage
------------- | -------------
my_corpus_bees_efrei.txt  | Corpus
vectors.txt  | generated embedding
vocab.txt | number of apparaitions of each word

## Train word vectors on a new corpus

<img src="https://travis-ci.org/stanfordnlp/GloVe.svg?branch=master"></img>

If the web datasets above don't match the semantics of your end use case, you can train word vectors on your own corpus.

    $ git clone https://github.com/stanfordnlp/glove
    $ cd glove && make
    $ ./demo.sh

The demo.sh script downloads a small corpus, consisting of the first 100M characters of Wikipedia. It collects unigram counts, constructs and shuffles cooccurrence data, and trains a simple version of the GloVe model. It also runs a word analogy evaluation script in python to verify word vector quality. More details about training on your own corpus can be found by reading [demo.sh](https://github.com/stanfordnlp/GloVe/blob/master/demo.sh) or the [src/README.md](https://github.com/stanfordnlp/GloVe/tree/master/src)

### License
All work contained in this package is licensed under the Apache License, Version 2.0. See the include LICENSE file.

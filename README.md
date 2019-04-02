# pretrained-italian-word2vec-emb

# COMING SOON... # 

A pretrained word2vec embeddings for italian languages.

This repositoy has one big purpose: in the last years I've had the possibility to work on NLP projects. I've spend a significant portion of my time looking for a decent pre-trained word vectors model for the Italian language. The faster solution I found was to make it on my own.

In this repository you can easily download (a not so light version of) a pre-trained 300-dimensional word vectors model (trained using word2vec) for Italian.

Vectors are trained using almost 24 milion of unique sentences, collected during the last year, enconding M different words. 
It's possible to see also extra-italian language words inside the vocabulary. This is because original texts may contain some foreign sentences.
I hope you will find my job useful for your purpose as well.

# Cleaning rules

I've decided to start with an easy cleaning:

* Words longer than 26 chars have been removed
* Words that start with *"http"* have been removed
* Words that contain *"@"* have been removed
* Words that contain *"#"* have been removed
* Words that contain *"www"* have been removed
* Words that end with *".ly"* have been removed
* Words that contain digits have been removed
* All no-alphabetic chars have been removed
* Lower transformation has been applied

# Usage 

``` python
from gensim.models import KeyedVectors
model2vec = KeyedVectors.load_word2vec_format("./PATH_HERE/pretrained-italian-word2vec-emb-300.bin", binary = True)
```

# Tutorials
* [link](https)
* [link](https)
* [link](https)

# Suggestions

New versions are going to be uploaded as soon as I can. Please feel free to contact me with suggestions regard cleaning rules or anything else.

# Requirement

* Gensim 3.3.0

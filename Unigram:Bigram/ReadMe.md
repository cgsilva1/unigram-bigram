## Overview

In this project, we build unigram and bigram indexes from text files using MapReduce. The unigram index captures occurrences of single words, while the bigram index captures occurrences of two-word sequences.

- **Unigram format**: `(word, docID:count)`
- **Bigram format**: `(word1 word2, docID)`

The merged reducer logic processes both unigrams and bigrams, outputting them in the correct formats based on the key type.

## File Structure

- **Unigram Data**: Data for unigrams is processed from files in the `fulldata` folder.
- **Bigram Data**: Data for bigrams is processed from files in the `devdata` folder.

The input data used is from the shorted data files provided 

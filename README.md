# Unigram & Bigram Indexing using MapReduce

## Overview
This project builds **unigram and bigram indexes** from large text datasets using **MapReduce**. It processes textual data to generate word frequency counts and track occurrences across documents.

## Features
- **Unigram Indexing**: Maps single words to their document occurrences.
- **Bigram Indexing**: Captures consecutive word pairs across documents.
- **Scalability**: Optimized for large-scale distributed processing.

## Input & Output Format
- **Unigram Output**: `(word, docID:count)`
- **Bigram Output**: `(word1 word2, docID)`

## Technologies Used
- **Hadoop MapReduce**
- **Java**
- **Apache Hadoop (YARN)**
- **HDFS (Hadoop Distributed File System)**

## How to Run
1. Upload the dataset (`fulldata` for unigrams, `devdata` for bigrams) to HDFS.
2. Compile and execute the MapReduce job:
   ```bash
   hadoop jar UnigramBigramIndexer.jar UnigramJob input_path output_path

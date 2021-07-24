# stance-detection/fake-news detection

Natural Langauge Processing Project - This repository contains an implementation of the paper "Emergent: a novel data-set for stance classification" used for identifying whether news topics are true or false. In executing this project we learnt about extracting useful feature representations from textual descriptions by first processing them into tokens and learning word embeddings such as word2vec which allow for numeric representations of the text. We then used these processed features for training machine learning models to be able to generate predictions. 

## Setting up for Development

1. Make a virtual environment using virtualenv: `virtualenv -p python3 env`
2. Activate it when running python scripts: `source env/bin/activate` (to deactivate, run `deactivate`).
3. Install required dependencies: `pip install -r requirements.txt`
4. Download Emergent Data from [here](https://drive.google.com/folderview?id=0BwPdBcatuO0vYTAxSnA1d09qdGM&usp=sharing) into `data/raw`
5. Download the PPDB data (xl lexical) from [paraphrase.org](http://paraphrase.org/#/download) int `data/external`
6. Run [notebooks/create_ppdb_dict.ipynb](notebooks/create_ppdb_dict.ipynb) to parse PPDB and convert it to a dictionary form

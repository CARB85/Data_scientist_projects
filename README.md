# Film Junky Union: Movie Review Classification

## Project Description

Film Junky Union, a cutting-edge community for classic movie enthusiasts, is developing a system to filter and categorize movie reviews. Your goal is to train a model to automatically detect negative reviews. To achieve this, you will use a labeled IMDB movie review dataset to build a model that classifies reviews as positive or negative. The model should achieve an F1 score of at least 0.85.

### Important Notes

You don't have to use BERT for the project because it requires significant computational power and will be very slow on a CPU for the entire dataset. BERT generally needs to run on a GPU for reasonable performance. However, if you'd like to include BERT, we recommend doing it on a smaller portion of the dataset. You can process only a few hundred items per part of the dataset (training/test) to avoid long waiting times. Make sure to indicate that you're using BERT in the first cell (project header).

## Data Description

The data is stored in the file `imdb_reviews.tsv`. 

The data was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts (2011). *Learning Word Vectors for Sentiment Analysis*. Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

### Dataset Fields:

- **review**: The text of the review.
- **pos**: The target label, '0' for negative and '1' for positive.
- **ds_part**: 'train'/'test' for the training/test split of the dataset, respectively.

There are other fields in the dataset, which you may explore if desired.

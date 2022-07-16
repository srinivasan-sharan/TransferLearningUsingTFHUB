# Transfer Learning Using TFHUB
In this project, I have tried learning more about transfer learning which is a subset of machine learning.


<img width="600" alt="627d125248f5fa07e1faf0c6_61f54fb4bbd0e14dfe068c8f_transfer-learned-knowledge" src="https://user-images.githubusercontent.com/63301665/179365804-ba690eae-5f0e-4ed4-8e47-75d9839a80d7.png">


# Dataset

We are using the [Quora Insincere Questions Classification](https://www.kaggle.com/c/quora-insincere-questions-classification/data) dataset, which is a collection of dataset whihc consists of questions provided by users on the popular social question-and-answer website. It also contains a tag which specifies wether a question is sincere or insincere, meaning if the questions asked are intended to make a statement rather than look for helpfull answers.

Characteristics of insincere questions: 
1) Has a non-neutral tone
2) Is disparaging or inflammatory
3) Isn't grounded in reality
4) Uses sexual content


# Models

Now to classify this data into sincere/insincere, we will be making use of several text-classification models, namely:
1) gnews-swivel-20dim
2) nnlm-en-dim50
3) nnlm-den-dim128
4) universal-sentence-encoder
5) universal-sentence-encoder-large

All of these models can be found on [tfhub.dev](tfhub.dev)

--------------------------------------------------------------------------------------------------------------------

gnews-swivel:

Token based text embedding trained on English Google News 130GB corpus. Created using Swivel matrix factorization method. The module takes a batch of sentences in a 1-D tensor of strings as input. The prepocessing is done by splitting on the spaces. It also contains 20000 tokens and 1 out of vacabulary bucket for unknown tokens.


nnlm: 

Collection of feed-forward neural network language token embeddings. Based on NNLM with two or three hidden layers, see individual module documentation. The modules take a batch of sentences in a 1-D tensor of strings as input. The module preprocesses its input by splitting on spaces and/or removing punctuation, see individual module documentation. Small fraction of the least frequent tokens and embeddings (~2.5%) are replaced by hash buckets. Each hash bucket is initialized using the remaining embedding vectors that hash to the same bucket. It contains a large number of trained models. We have used 2 of them


universal-sentece-encoder:

Collection of universal sentence encoders trained on variety of data. The Universal Sentence Encoder encodes text into high-dimensional vectors that can be used for text classification, semantic similarity, clustering and other natural language tasks. It contains a large number of trained models. We have used 2 of them


 








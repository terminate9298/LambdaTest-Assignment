# Assignment 3
##### Prepare a classifier to classify real news from fake news and assess on below dataset. Use suitable methods for extra accuracy.
* Download Link : https://drive.google.com/file/d/1PHvaNfmqeZkXRoXkMaMnbfjHFqaXPzUz/view?usp=sharing

## Possible Solutions to the Problem

1.   RNN Based Models : Training Any DNN Model from Scratch and Training that over Complete Dataset.
2.   Machine Learning Approch : Tokenizing the Dataset and using Word2Vec followed by Any Machine Learning Model like Random Forest or KNN to classify sentences.
3.   Using Any pretrained Sentence Embedding Like BERT or GPT-2 followed by ANN to find Fake News in Dataset

I implemented Sentence Embedding followed by Neural Network gaining over accuracy of 99.76% on testing Dataset.

## Sentence Transformers
This framework provides an easy method to compute dense vector representations for sentences, paragraphs, and images. The models are based on transformer networks like BERT / RoBERTa / XLM-RoBERTa etc. and achieve state-of-the-art performance in various task. Text is embedding in vector space such that similar text is close and can efficiently be found using cosine similarity.

![Github Link](https://github.com/UKPLab/sentence-transformers)

### Advantages of using Pretrained Sentence Embedding
* Faster Compution due to Simpler Artitecture
* Can Take Advantage of Pretrained BERT Network
* Sentence sizes are Long and required 16+ Gb of RAM if not truncated while implementing RNN Based Network
* Vocab size is 1,00,000+ Making Embedding Matrix Very large and Computationaly Expensive
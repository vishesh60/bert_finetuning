# Bert Finetuning

Finetuning the BERT model on glance data to get more semantically informative embeddings


## Training

The following framework allows you to finetune the BERT model based on your own domain data.

#### Training data steps

The framework utilizes a siamese network structure on a given base BERT model and adds a pooling layer on top of it, followed by a softmax classifier.
The training data consists of 3 columns, with the first two consisting of sentence A and sentence B while the third column contains a label marking the 2 given sentences as semantically similar or dissimilar.

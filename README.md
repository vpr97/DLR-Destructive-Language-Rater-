# DestructiveLanguageRater

Nowadays, contributing content online has grown to be a
primary factor. It has become the main connecting factor for
people around the world. Every day, social networking sites
post millions of pieces of material. The contents are a mixture
of compliments, opinions, harmful material, etc. The quality
of human existence is greatly impacted by the toxic material,
which also has harmful direct and indirect effects. To protect
the wellness and comfort of their users, all social media firms
employ a variety of techniques to remove these harmful words
from their platforms. It is now difficult to distinguish between
harmful and normal material due to the vast volume of data.
Our project’s goal is to create a machine-learning model that
can distinguish between different message types. Some of the
types which we mainly consider classifying the language are
toxic, obscene, severe toxic, identity hate, threat, and insult.
Initially we planned on proceeding LSTM model as we
thought of training the whole model using our dataset for
accuracy and reliability. But based on the feedback we received
we are now using BERT model where we use pretrained model
for our project.


We are using BERT (Bidirectional Encoder Representations
from Transformers) model ”bert-base-uncased” for our project.
This model is pretrained on raw text without any labels
by Masked language modeling (MLM) and Next sentence
prediction (NSP). Our model takes sequence of token as input
and classifies the text. We first train the BERT model with our
train dataset and use validation dataset to validate the working
of the model.

Our baseline model is a simple Machine learning model that
converts the input words to vectors. This model will be having
a fully connected linear layer and the output from the layer will
be passed to an activation function. Based on the probabilities
obtained, the sentence will be classified into different toxicity
classes.

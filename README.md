# NLP_BERT
BERT Implementation on various datasets


## BERT Basics:

BERT stands for Bidirectional Encoder Representations from Transformers (BERT). It is a transformer-based machine learning technique for Natural Language Processing   (NLP) developed by Google.

It is basically a transformer language model with a variable number of encoder layers and self-attention heads.

BERT has two models: 
  * BERTBASE: 12 encoders with 12 bidirectional self-attention heads
  * BERTLARGE: 24 encoders with 16 bidirectional self-attention heads

Both models are pre-trained from unlabeled data extracted from the BooksCorpus with 800M words and English Wikipedia with 2,500M words.

Training is done by making a few words(~15%) in a sentence and tasking the model to predict the masked words.
As the model learns to predict the masked words, it simultaneously learns to produce a powerful internal representation of the words as word embeddings.

BERT was pretrained on two tasks:
  * Language Modelling (15% of tokens were masked and BERT was trained to predict them from context)
  * Sentence Prediction (BERT was trained to predict if a chosen next sentence was probable or not given the first sentence).

As a result of the training process, BERT learns contextual embeddings for words. After pretraining, which is computationally expensive, BERT can be finetuned with     fewer resources on smaller datasets to optimize its performance on specific tasks.


## LSTM Basics:


  LSTM networks are an improvement over RNN (Recurrent Neural Networks).


  They are specifically designed for processing, classifying, and making predictions based on time series of sequential data to compensate for unknown lags between       important events in a time series.


  Applications such as speech recognition, handwriting recognition, and anomaly detection in network traffic or Intrusion Detection Systems (IDS’s) finds the use of     LSTMs.


  Unlike standard feed-forward neural networks, LSTMs have feedback connections and, as a result, can process entire data sequences in addition to single data points     (such as images, speech or video).


  An LSTM unit is typically built with a cell, an input gate, an output gate, and a forget gate.


  The cell can remember values from arbitrary time intervals, and the three gates control the flow of information in and out of the cell.


  LSTMs were created to solve vanishing and bursting gradients, which are common while training regular RNNs.


## RNN Basics:

Recurrent Neural Network(RNN) is a popular architecture of Neural Network which is used extensively with use cases consist of sequential or contextual data.

In traditional neural networks, all the inputs and outputs are independent of each other, but in cases like when it is required to predict the next word of a           sentence, the previous words are required and hence there is a need to remember the previous words. Thus RNN came into existence, which solved this issue with the     help of a Hidden Layer. The main and most important feature of RNN is Hidden state, which remembers some information about a sequence.

RNN have a “memory” which remembers all information about what has been calculated. It uses the same parameters for each input as it performs the same task on all     the inputs or hidden layers to produce the output. This reduces the complexity of parameters, unlike other neural networks.

Advantages of RNN:
  * An RNN remembers each and every information through time. It is useful in time series prediction only because of the feature to remember previous inputs as             well. This is called Long Short Term Memory.
  * For Computer Vision and Image Processing Applications, Recurrent neural network are even used with convolutional layers to extend the effective pixel neighborhood.


Disadvantages of Recurrent Neural Network:
  * Gradient vanishing and exploding problems.
  * Training an RNN is a very difficult task.
  * It cannot process very long sequences if using tanh or relu as an activation function.


## Contributors
* Tonumoy Mukherjee tonumoymukherjee1@gmail.com

## License & Copyright
&#169; Tonumoy Mukherjee, TuTeck Technologies Pvt. Ltd
> Licensed under the [MIT License](LICENSE).

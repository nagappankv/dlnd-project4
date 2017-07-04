### dlnd-project4 - Language Translation

In this project, we are going to take a peek into the realm of neural network machine translation. We will be training a sequence to sequence model on a dataset of English and French sentences that can translate new sentences from English to French.

## Environment: Tensorflow 1.0

floyd run --cpu --env tensorflow-1.0 --mode jupyter

## Hyperparameters
- Number of Epochs
epochs = 5
- Batch Size
batch_size = 256
- RNN Size
rnn_size = 256
- Number of Layers
num_layers = 3
- Embedding Size
encoding_embedding_size = 256
decoding_embedding_size = 256
- Learning Rate
learning_rate = 0.001
- Dropout Keep Probability
keep_probability = 0.8

## Training
Epoch   4 Batch  536/538 - Train Accuracy:  0.975, Validation Accuracy:  0.963, Loss:  0.017

## Translation
Input
  Word Ids:      [170, 139, 151, 140, 197, 113, 59]
  English Words: ['he', 'saw', 'a', 'old', 'yellow', 'truck', '.']

Prediction
  Word Ids:      [131, 317, 343, 162, 139, 231, 114, 1]
  French Words: ['il', 'vu', 'une', 'nouveau', 'camion', 'jaune', '.', '<EOS>']
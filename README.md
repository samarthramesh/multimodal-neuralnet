# Multimodal Neural Network
Multimodal modal recipe retrieval system built using PyTorch for text (instructions and ingredients) and images


# Dataset
Utilized the MIT Recipe 1M+ dataset for recipe information

# Text Side
## Instruction Embeddings
The [Infersent](https://github.com/facebookresearch/InferSent) sentence embeddings were used to embed the recipe instructions

## Ingredient Embeddings
The individual ingredients were cleaned and embedded using TensorFlow

# Image Side
The ResNet-50 CNN model was used for the image embeddings

# Model
Ingredient encodings were fed into a bi-directional LSTM and instruction embeddings were fed into a unidirectional LSTM. These encodings were concatenated and passed through a fully connected layer. Cosine similarity loss function was then used to train the model. First, the text side was trained and then, resnet-50 model was fine tuned. 

# Contributors
Ananya Gupta, Raghav Sriram, Samarth Ramesh, Samyak Jain
# License
[MIT](License)

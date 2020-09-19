# Multimodal Neural Network
Multimodal modal recipe retrieval system for text and images


# Dataset
Utilized the MIT Recipe 1M+ dataset for recipe information

# Text Side
## Instruction Embeddings
The [Infersent](https://github.com/facebookresearch/InferSent) sentence embeddings were used to embed the recipe instructions

## Ingredient Embeddings
The individual ingredients were cleaned and embedded using TensorFlow

# Image Side
The ResNet-50 CNN model was used for the image embeddings

# License
https://github.com/facebookresearch/InferSent

# Multimodal Neural Network
Multimodal modal recipe retrieval system built using PyTorch for text (instructions and ingredients) and images


# Dataset
Utilized the MIT Recipe 1M+ dataset for recipe information

# Text Side
## [Instruction Embeddings](https://github.com/sriram-raghav/multimodal-neuralnet/blob/master/Text-side/Instructions_embeddings.ipynb)
The [Infersent](https://github.com/facebookresearch/InferSent) sentence embeddings were used to embed the recipe instructions

## [Ingredient Embeddings](https://github.com/sriram-raghav/multimodal-neuralnet/blob/master/Text-side/IngredientsEmbedding.ipynb)
The individual ingredients were cleaned and embedded using TensorFlow

# [Image Side](https://github.com/sriram-raghav/multimodal-neuralnet/blob/master/Image-side/Image_Embeddings.ipynb)
The ResNet-50 CNN model was used for the image embeddings

# [Model](https://github.com/sriram-raghav/multimodal-neuralnet/blob/master/model.ipynb)
Ingredient encodings were fed into a bi-directional LSTM and instruction embeddings were fed into a unidirectional LSTM. These encodings were concatenated and passed through a fully connected layer. Cosine similarity loss function was then used to train the model. First, the text side was trained and then, resnet-50 model was [fine tuned](https://github.com/sriram-raghav/multimodal-neuralnet/blob/master/Image-side/Finetuning.ipynb). 

# Contributors
Ananya Gupta, Raghav Sriram, Samarth Ramesh, Samyak Jain
# License
[MIT](License)

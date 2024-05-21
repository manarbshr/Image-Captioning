### Image Captioning with Deep Learning

This repository contains code for an image captioning model implemented using TensorFlow and Keras. Below is an overview of the key components and functionalities:

#### 1. Data Preprocessing:
- The dataset used is the Flickr8k dataset, which contains images along with corresponding captions.
- Text preprocessing techniques such as lowercasing, removing special characters, tokenization, and adding start and end sequence tokens are applied to the captions.

#### 2. Model Architecture:
- The image captioning model consists of a combination of convolutional and recurrent neural network layers.
- Image features are extracted using a pre-trained DenseNet201 model.
- Custom data generators are used for efficient memory usage and dynamic data loading during training.

#### 3. Training and Evaluation:
- The model is trained using a custom data generator on a training set and evaluated on a separate validation set.
- Model checkpoints, early stopping, and learning rate reduction callbacks are employed to monitor and improve training performance.

#### 4. Inference and Caption Generation:
- Trained models can be used to generate captions for new images.
- Text-to-speech functionality is included to convert generated captions into audio.

#### 5. Requirements:
- Python 3.x
- TensorFlow 2.x
- Keras
- NumPy
- gTTS (Google Text-to-Speech)

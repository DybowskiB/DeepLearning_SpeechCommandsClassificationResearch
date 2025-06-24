# Speech Command Classification

This project explores the effectiveness of different deep learning architectures for speech command classification. We compare a standard ResNet-18 model, its variant enhanced with silence detection, and the transformer-based Wav2Vec2.0 model.

## Dataset

We use the [Speech Commands v0.02](https://arxiv.org/abs/1804.03209) dataset, which contains short audio clips of spoken commands. The data is split into training, validation, and testing sets based on provided list files. Background noise and silence clips are also included to evaluate model robustness.

## Models

- **ResNet-18**: A convolutional baseline using MelSpectrograms and a pretrained ResNet-18 backbone.  
- **SilenceDetector**: An improved ResNet-18 that includes silence and noise samples to boost noise robustness.  
- **Wav2Vec2.0**: A pretrained transformer model (by Meta) used in a zero-shot setting or with a lightweight classification head.

# waste-image-classification
Explore the performance of waste image classification through modifying the architectures of InceptionResNetV2.

## Comparison of Optimizers
The Inception-ResNetV2 is trained with different optimizers with default hyperparameter setting and below shows the result obtained.
| Optimizers | Train Acc (%) | Test Acc (%) |
| :--------: | :-----------: | :----------: |
| RMSprop (baseline) | 99.7526 | 85.7708 |
| Adam | 99.9505 | 86.9565 |
| SGD | 95.5962 | 81.4229 |
| SGD + Nesterov | 93.7160 | 81.2253 |
| Adagrad | 99.7031 | 83.9921 |
| Adadelta | 97.9713 | 80.0395 |

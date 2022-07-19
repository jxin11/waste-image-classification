# waste-image-classification
Dataset: TrashNet (https://github.com/garythung/trashnet)
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

## Comparison of Network Depth
In the previous experiment, the Adam optimiser is selected as the most suitable optimiser. The Inception-ResNetV2 is trained with different depth by reducing the Inception-ResNet A, B and C blocks. 
| Model | Train Acc (%) | Test Acc (%) |
| :--------: | :-----------: | :----------: |
| Inception-ResNetV2-5,10,5 (baseline) | 99.9505 | 86.9565 |
| Inception-ResNetV2-4,9,4 | 99.9505 | 86.1660 |
| Inception-ResNetV2-3,8,3 | 99.9010 | 84.1897 |
| Inception-ResNetV2-2,7,2 | 99.8516 | 86.9565 |
| Inception-ResNetV2-1,6,1 | 99.9505 | 87.3518 |

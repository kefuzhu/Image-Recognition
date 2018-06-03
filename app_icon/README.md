# App Icon

This is a project from TalkingData. I tried to identify different packageNames from the same app by recognizing their app icon image.

The first try was a 4-convolutional layers CNN built from scratch using Pytorch. After 500 iterations training on 11,334 labeled images (10,826 distinct classes), the model can reach about 84% accuracy on the training data. Since I only have 11,334 images for 10,826 different classes, this is basically a one-shot learning.

In general, due to few human label errors and lack of training data, the model does not perform up to expectation.

** Furture work **:
1. Try retrain and finetune pre-trained model (Transfering learning)
2. Perform more transformations on images to make the model more robust and also potentially add more training data
3. Try different pooling techniques (currently using GlobalAveragePooling) and add more convolutional layers

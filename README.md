# EfficientNet_B0---Image-Classification \n

Using a pretrained EfficientNet-B0 model to build a image classifier on Cards Dataset.\n
Used timm module to import the pretrained model. \n
The dataset used is available at https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification and I've used the kaggle API to download and import the dataset directly to my working directory. \n
The loss calculation is done with Cross Entropy, Adam optimizer is used with a learning rate=0.001 and the training loop goes for 5 epochs. \n

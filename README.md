# EfficientNet_B0---Image-Classification

Using a pretrained EfficientNet-B0 model to build a image classifier on Cards Dataset.

Used timm module to import the pretrained model.

The dataset used is available at https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification and I've used the kaggle API to download and import the dataset directly to my working directory. I've used Google Colab with T4 GPU to run this model.

The loss calculation is done with Cross Entropy, Adam optimizer is used with a learning rate=0.001 and the training loop goes for 5 epochs.

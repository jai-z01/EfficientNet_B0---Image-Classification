# Playing Card Image Classification with EfficientNet-B0

## Overview

This repository contains code for training a playing card image classifier using a pretrained EfficientNet-B0 model. The model is trained on the Cards Dataset, and the implementation is done in Google Colab using a T4 GPU.

## Dataset

The Cards Dataset is used for training and evaluation. You can download the dataset from [Kaggle](https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification) and follow the instructions in the notebook to set up the dataset in your working directory.

## Environment Setup

To run the code, ensure you have the required dependencies installed. You can install them using the following:

```bash
pip install torch torchvision timm tqdm matplotlib
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. Set up the Kaggle API:

   - Place your Kaggle API key in the `kaggle.json` file and copy it to the `~/.kaggle/` directory.

3. Download and extract the dataset:

   ```bash
   kaggle datasets download -d gpiosenka/cards-image-datasetclassification
   unzip cards-image-datasetclassification.zip
   ```

4. Run the Jupyter Notebook:

   Open the Jupyter Notebook in Google Colab and execute the cells. Make sure to select the appropriate GPU runtime for accelerated training.

## Model Architecture

The image classifier uses a SimpleCardClassifier based on the EfficientNet-B0 model. The model is trained for 5 epochs with the Adam optimizer and Cross Entropy loss.

## Training

The training loop is implemented with a validation step, and the training progress is visualized with loss curves.

## Evaluating Results

The model's performance is evaluated on sample test images, and predictions are visualized alongside the original images.

## Contributing

If you'd like to contribute to this project, please follow the standard GitHub flow:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your fork and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

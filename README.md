# EfficientNet_B0 Image Classification

## Overview

This project leverages a pretrained EfficientNet-B0 model for image classification on the Cards Dataset. The EfficientNet-B0 model is imported using the `timm` module, and the entire process is implemented using Google Colab with a T4 GPU.

## Dataset

The dataset used for training and evaluation is available on Kaggle: [Cards Image Dataset](https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification). The Kaggle API is utilized to download and import the dataset directly into the working directory.

## Environment

The model is trained using Google Colab, taking advantage of the T4 GPU for accelerated computations.

## Dependencies

Ensure the following dependencies are installed to run the project:

- `timm`
- `torch`
- `torchvision`
- `kaggle`

Install the required packages using the following:

```bash
pip install timm torch torchvision kaggle
```

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### 2. Download and Extract the Dataset

Use the Kaggle API to download and extract the dataset:

```bash
kaggle datasets download -d gpiosenka/cards-image-datasetclassification
unzip cards-image-datasetclassification.zip
```

### 3. Run the Jupyter Notebook

Open the Jupyter Notebook in Google Colab and execute the cells. Make sure to select the appropriate GPU runtime for accelerated training.

### 4. Configuration

The configuration can be adjusted in the Jupyter Notebook. Key configurations include:

- Model: EfficientNet-B0
- Loss Function: Cross Entropy
- Optimizer: Adam with learning rate=0.001
- Training Epochs: 5

## Contributing

If you'd like to contribute to this project, please follow the standard GitHub flow:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push to your fork and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The EfficientNet-B0 model is from the `timm` module.
- The dataset is provided by [gpiosenka](https://www.kaggle.com/gpiosenka) on Kaggle.

Feel free to customize this README to suit your specific project details. A clear and concise README enhances the usability and collaboration potential of your project.

# Unit 0: Binary Image Classification

This unit demonstrates a transfer learning pipeline using **EfficientNet-B0** to classify fruit variants from the Fruits-360 dataset.

## Project Structure

* **`00_Check_Environment.ipynb`**: GPU/CUDA and dependency verification.
* **`01_Check_Data.ipynb`**: Dataset EDA and category distribution analysis.
* **`02_PrepData.ipynb`**: Dataset subsetting using **symlinks** to `PrepData/`.
* **`03_TrainModel.ipynb`**: Fine-tuning via `timm` (PyTorch Image Models).
* **`04_Inference.ipynb`**: Performance metrics (Confusion Matrix, F1-Score).



## Technical Requirements

Managed via `uv`. Key dependencies:
- `torch`, `torchvision` (Deep Learning)
- `timm` (EfficientNet-B0 architecture)
- `scikit-learn` (Evaluation metrics)
- `matplotlib`, `ipywidgets` (Visualization)

## Workflow

1. **Symlinking**: We avoid data duplication by linking raw images into `PrepData/Training`, `Validation`, and `Test`.
2. **Transfer Learning**: We utilize ImageNet-pretrained weights and replace the classifier head for binary output.
3. **Normalization**: Images are resized to $224 \times 224$ and normalized using model-specific mean/std.



## Usage

1. Ensure the dataset is in `data/fruits-360`.
2. Run `uv sync` to install dependencies.
3. Execute notebooks sequentially (00–04).

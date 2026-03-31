# Dog vs. Cat Classification using Transfer Learning (ResNet18)

This repository features a binary image classification system designed to distinguish between cats and dogs. By utilizing **Transfer Learning** with a pre-trained **ResNet18** model, the project achieves high accuracy and rapid convergence.

## 📊 Project Performance
* **Test Accuracy:** 97.90%
* **Training Efficiency:** Reached high precision in just 5 epochs using an NVIDIA T4 GPU.

## 📂 Dataset
The model is trained on the **Dog and Cat Classification Dataset** available on Kaggle.
* **Dataset Link:** [Kaggle: Dog and Cat Classification](https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset/data)
* **Structure:** The project expects a `PetImages.zip` file containing labeled subfolders for 'Cat' and 'Dog'.

## 🛠️ Key Features
- **Architecture:** Pre-trained ResNet18 with frozen early layers to preserve low-level feature detection.
- **Custom Head:** A modified fully connected layer specifically for 2-class (binary) output.
- **Dynamic Inference:** A built-in utility to perform predictions on images directly from web URLs.
- **Persistence:** Full support for saving and loading model `state_dicts` to bypass retraining.

## 🚀 Usage & Environment

### Recommended: Google Colab
**For optimal performance, it is highly recommended to run this notebook on Google Colab using a GPU or TPU.** 1. Open `main.ipynb` in Google Colab.
2. Set the Hardware Accelerator to **T4 GPU** (`Runtime` > `Change runtime type`).
3. Mount Google Drive to access your dataset and save model weights.

### Local Setup
If running locally, ensure you have a CUDA-compatible environment.
```bash
git clone [https://github.com/ehsaan08-ai/image-classification-using-cnn.git](https://github.com/ehsaan08-ai/image-classification-using-cnn.git)
cd image-classification-using-cnn
pip install -r requirements.txt

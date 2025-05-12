# Brain Tumor Classifier with Gradio UI

This project is a brain tumor image classification system built using TensorFlow/Keras and integrated with a simple Gradio user interface. It detects four classes of brain tumors:

* Glioma
* Meningioma
* No Tumor
* Pituitary

## 📁 Dataset

The model uses a dataset organized into subfolders per class under:

```
/content/drive/MyDrive/braintumor/Training/
```

Each subfolder should contain images corresponding to that class label.

## 🚀 Features

* Preprocessing with OpenCV
* Neural network built with Conv2D, MaxPooling, BatchNormalization, and Dropout
* Model evaluation and validation
* Image upload and live prediction using Gradio

## 📦 Requirements

Install the required libraries:

```bash
pip install gradio opencv-python tensorflow
```

Also mount Google Drive in Colab to access the dataset:

```python
from google.colab import drive
drive.mount('/content/drive')
```

## 🧠 Model Architecture

The CNN model includes:

* 3 convolutional blocks
* Global Average Pooling
* Dense layers with ReLU and softmax activations
* Dropout for regularization

## 🖼️ Usage

1. Run all cells in the notebook to train the model.
2. Upload a brain MRI image via the Gradio interface.
3. The model will predict one of the four tumor types.

## 📝 Notes

* Training may take several minutes depending on hardware.
* You can adjust `EPOCHS`, `IMG_SIZE`, and other hyperparameters to improve accuracy.

## 📄 License

For academic and educational use only.

---

Developed for brain tumor classification research and experimentation.

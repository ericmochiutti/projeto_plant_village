# Plant Disease Detection with TensorFlow and Keras

This project focuses on developing and training a deep learning model to classify plant diseases from leaf images. The model is optimized for deployment on embedded devices like the Raspberry Pi.

---

## 1. Project Overview

- **Dataset:** Uses the [PlantVillage dataset](https://www.kaggle.com/datasets/abdallahalide/plantvillage-dataset), which contains images of plant leaves with various diseases.  
- **Model:** A `DenseNet121` convolutional neural network (CNN) is trained using TensorFlow and Keras.  
- **Output:** The trained model is saved in three formats:  
  - `densenet_plantvillage.h5` (Legacy HDF5 format)  
  - `densenet_plantvillage.keras` (Native Keras format)  
  - `densenet_plantvillage.tflite` (TensorFlow Lite format for edge devices)  

---

## 2. Setup and Installation

This project uses [`uv`](https://pypi.org/project/uv/) from Astral for environment and dependency management.

### 2.1 Create a virtual environment

```bash
uv venv
```

### 2.2 Create a virtual environment

```bash
uv shell
```

### 2.3 Install dependencies


```bash
uv pip install -e .
```

### 3.3 Open and Run the Notebook

Open `notebook/plant_disease_detection.ipynb` in your browser and run the cells sequentially.

---

## 4. Project Structure

- `data/` – Contains the PlantVillage dataset.  
- `model/` – Stores trained models in `.h5`, `.keras`, and `.tflite` formats.  
- `notebook/` – Contains the main Jupyter notebook with the complete code for the project.  
- `pyproject.toml` – Defines project dependencies for `uv`.
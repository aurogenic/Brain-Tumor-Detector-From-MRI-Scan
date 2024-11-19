# **Tumor Detection from MRI Scans**

This repository contains a deep learning model and a simple graphical user interface (GUI) for detecting tumors in MRI scans. The project is built using TensorFlow/Keras and leverages transfer learning with the Xception architecture for accurate classification.

---

## **Features**
- **Pre-trained Model**: The model is fine-tuned on MRI images for multi-class tumor classification.
- **Image Augmentation**: Improves model generalization through augmented data during training.
- **Graphical User Interface**: A user-friendly GUI for testing or example usage.
- **Training Notebook**: Includes a Jupyter notebook detailing the training process step-by-step.
- **Robust Image Handling**: MRI Scan Images of all Dimensions and Mode are accepted as they are handled Dynamically.

---

## **How It Works**
1. **Training**:
   - Transfer learning with the Xception model, fine-tuned on MRI scan data.
   - Includes techniques to prevent overfitting, such as dropout and data augmentation.

2. **Inference**:
   - Accepts MRI images.
   - Processes the image (resizing, normalizing, and ensuring RGB format).
   - Predicts tumor presence and type with confidence levels.

---

## **Repository Contents**
- `model/`: Contains the saved trained model in Multiple Formats(.keras and .h5).
- `app.py`: Python script for the GUI, built using libraries like Tkinter.
- `utils.py`: Contains Model class with methods for image preprocessing and model predictions.
- `trainer.ipynb`: Jupyter notebook used to train the model, including all preprocessing steps.
- `requirements.txt`: Lists all dependencies for easy setup.
- `README.md`: Instructions on setting up and running the project.

---

## **Dataset**
The model was trained using an MRI scan dataset available on Kaggle. You can download the dataset [here](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset).

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/aurogenic/Brain-Tumor-Detector-From-MRI-Scan
   cd Brain-Tumor-Detector-From-MRI-Scan
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the GUI:
   ```bash
   python app.py
   ```

---

## **Usage**
- Open the GUI and upload an MRI image for classification.
- The application will display the predicted tumor type along with the confidence score.

---

## **Contributing**
Feel free to contribute by submitting issues or pull requests. Let's improve this project together!

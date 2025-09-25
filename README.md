# Computer Vision: CIFAR-10 Image Classification

This project demonstrates the construction and training of a Convolutional Neural Network (CNN) from scratch to classify images from the classic CIFAR-10 dataset. It showcases a professional workflow where the dataset is loaded directly via the Keras API, ensuring the code repository remains lightweight and perfectly reproducible.


*(After running the notebook, take a screenshot of your final training/validation curves, upload it to a site like Imgur, and paste the link here.)*

## The Goal
To build an accurate, end-to-end deep learning model for the benchmark CIFAR-10 image classification task, demonstrating a strong understanding of CNN architecture, training, and evaluation.

## The Process
1.  **Dynamic Data Loading:** The CIFAR-10 dataset (60,000 32x32 color images in 10 classes) is loaded directly using `tensorflow.keras.datasets.cifar10.load_data()`. This professional approach requires no manual data downloads or uploads.
2.  **Data Augmentation:** To combat overfitting, `RandomFlip` and `RandomRotation` layers are added to the model to generate modified training images in real-time.
3.  **CNN Architecture:** A sequential CNN was designed with three convolutional blocks and Dropout for regularization, optimized for the 32x32 input size of CIFAR-10 images.
4.  **Training & Evaluation:** The model was trained and evaluated, with the accuracy and loss curves plotted to provide a clear visual representation of the learning process.

## How to Run
```bash
# Clone the repository
git clone [https://github.com/YOUR_USERNAME/cv-image-classifier.git](https://github.com/YOUR_USERNAME/cv-image-classifier.git)
cd cv-image-classifier

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter Notebook
# The first time you run the notebook, Keras will automatically download the CIFAR-10 dataset.
jupyter notebook image_classification.ipynb
```

## Architect's Notes
- **Professional Data Handling:** Storing large datasets in Git is bad practice. Loading standard benchmark datasets directly from the deep learning framework's API (like Keras Datasets) is the clean, reproducible, and professional standard.
- **Tuning for Small Images:** CIFAR-10's 32x32 images are challenging. The CNN architecture was specifically designed to not downsample the image too quickly with `MaxPooling` layers, preserving spatial information for as long as possible.

### My Process & Learnings
***(This is your section. Follow the Authenticity Blueprint. Example: "Getting high accuracy on CIFAR-10 was tougher than I expected due to the low-resolution images. I found that adding a third convolutional layer and a Dropout rate of 0.3 provided the best balance between learning complex features and preventing overfitting. This taught me that model architecture is not one-size-fits-all and must be adapted to the data's specific characteristics.")***

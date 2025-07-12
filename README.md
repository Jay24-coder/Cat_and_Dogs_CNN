# Cat vs Dog Classifier 🐱🐶

This project implements a binary image classifier using a Convolutional Neural Network (CNN) in Keras to distinguish between images of cats and dogs.

---

## 🗂️ Dataset Structure

Make sure your dataset is organized like this:
```
cat_dog/
├── cats/
│ ├── cat1.jpg
│ ├── cat2.jpg
│ └── ...
└── dogs/
├── dog1.jpg
├── dog2.jpg
└── ...
```

Each subdirectory contains images for the corresponding class.

## 🛠️ Installation

1. Clone this repository or copy the code into your project folder.
2. Install the required Python packages:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow keras
```

---

## 📦 Libraries Used
- `TensorFlow/Keras`: For building and training the deep learning model
- `scikit-learn`: For splitting data
- `Pandas & NumPy`: For data manipulation
- `Matplotlib`: For visualization

---

## 📸 Image Preprocessing
Images are resized to `(150, 150)` pixels.

Images are loaded and converted to NumPy arrays for feeding into the model.

Labels: `0` for cats and `1` for dogs.

---

## 🧠 Model Architecture
Sequential Model:
- Conv2D: 50 filters, 3x3 kernel, ReLU activation
- MaxPooling2D: 2x2 pool size
- Conv2D: 50 filters, 3x3 kernel, ReLU activation
- Flatten
- Dense: 1 neuron, sigmoid activation

---

## 📊 Sample Visualization
The script visualizes 15 random images from the dataset along with their class labels before training.

---

## 🚀 Results
After training, the model outputs training and validation accuracy for each epoch. You can further improve performance by:
- Adding Dropout layers
- Using more Conv2D/MaxPool2D layers
- Switching to more advanced architectures (e.g., VGG16, ResNet)

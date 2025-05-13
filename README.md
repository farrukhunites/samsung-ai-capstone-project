# Facial Emotion Recognition using CNN 😃😢😡

This project implements a Convolutional Neural Network (CNN) to recognize human emotions from facial expressions using the **FER-2013 dataset**. It classifies images into one of seven emotions: **Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral**.

## 📌 Overview

Facial emotion recognition is a key application of computer vision and deep learning in fields like healthcare, human-computer interaction, and behavioral analysis. In this project:

- We preprocess grayscale face images from FER-2013 dataset.
- We train a custom CNN model for emotion classification.
- We evaluate and visualize model performance with metrics and plots.

---

## 🧠 Model Architecture

The CNN architecture includes:

- 3 convolutional blocks (Conv → ReLU → MaxPooling → Dropout)
- Fully connected dense layers
- Softmax activation for multiclass classification

```text
Input → [Conv2D → ReLU → MaxPool → Dropout] x3 → Flatten → Dense → Dropout → Output
```

---

## 📊 Dataset

- **Name**: [FER-2013](https://www.kaggle.com/datasets/msambare/fer2013)
- **Format**: 48x48 grayscale images
- **Classes**: Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral
- **Split**: Training (28,709), Validation (3,589), Test (3,589)

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib, Seaborn
- Scikit-learn

---

## 🚀 How to Run

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/facial-emotion-recognition-cnn.git
   cd facial-emotion-recognition-cnn
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run training**
   ```bash
   python train.py
   ```

4. **Evaluate model**
   ```bash
   python evaluate.py
   ```

5. **Make predictions**
   ```bash
   python predict.py --image path/to/image.jpg
   ```

---

## 📈 Results

- **Training Accuracy**: 92%
- **Validation Accuracy**: 65% (FER-2013 is a noisy dataset)
- **Confusion Matrix** and **Classification Report** included in results.

---

## 🖼️ Sample Outputs

| Input Image | Predicted Emotion |
|-------------|--------------------|
| ![sample1](assets/sample1.png) | Happy |
| ![sample2](assets/sample2.png) | Sad   |

---

## 📂 Project Structure

```
.
├── data/                     # Dataset folder (download separately)
├── models/                   # Saved model weights
├── src/
│   ├── model.py              # CNN architecture
│   ├── train.py              # Training script
│   ├── evaluate.py           # Evaluation script
│   └── predict.py            # For inference
├── assets/                   # Plots and sample images
├── requirements.txt
└── README.md
```

---

## 🔮 Future Improvements

- Use data augmentation to improve generalization
- Add facial landmarks detection for better feature learning
- Experiment with transfer learning (e.g., VGG16, ResNet)
- Deploy using Streamlit or Flask as a web app

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙋‍♂️ About Me

**Muhammad Farrukh Umair**  
Associate Software Engineer | AI & Data Enthusiast  
🔗 [LinkedIn](https://www.linkedin.com/in/YOUR_PROFILE) | 📫 [Email](mailto:haris.umair2002@gmail.com)

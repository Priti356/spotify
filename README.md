# 🎵 Music Genre Classification Using CNN

## 📌 Project Overview

Music Genre Classification is a deep learning project that uses a Convolutional Neural Network (CNN) to classify audio files into different music genres.

The project extracts meaningful audio features using **Mel Spectrograms** and uses a CNN model built with TensorFlow and Keras to predict the genre of a music track.

The model is designed to classify music into 10 different genres.

## 🎯 Project Objectives

- Load and process audio files using Librosa.
- Extract Mel Spectrogram features from audio signals.
- Prepare and encode music genre labels.
- Build and train a CNN-based classification model.
- Evaluate model performance using classification metrics.
- Predict the genre of a new audio file.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Deep Learning:** TensorFlow, Keras
- **Audio Processing:** Librosa, SoundFile
- **Data Processing:** NumPy
- **Data Visualization:** Matplotlib
- **Machine Learning:** Scikit-learn
- **Development Environment:** Google Colab

## 📂 Dataset

This project uses the **GTZAN Music Genre Dataset**, which contains audio tracks belonging to 10 different genres.

**Dataset:** [GTZAN Music Genre Classification – Kaggle](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification)

### Music Genres

1. Blues
2. Classical
3. Country
4. Disco
5. Hip-hop
6. Jazz
7. Metal
8. Pop
9. Reggae
10. Rock

The original dataset contains 1,000 audio files. Due to one unreadable audio file, 999 files were successfully processed for this project.

## ⚙️ Project Workflow

1. **Data Collection:** Obtain the GTZAN music genre dataset.
2. **Audio Loading:** Load audio files using Librosa at a sampling rate of 22,050 Hz.
3. **Feature Extraction:** Generate Mel Spectrograms with 128 Mel frequency bands.
4. **Data Preprocessing:** Convert genre labels into numerical values and reshape features for CNN input.
5. **Data Splitting:** Split the dataset into 80% training data and 20% testing data.
6. **Model Building:** Develop a CNN architecture using convolutional, pooling, batch normalization, and dense layers.
7. **Model Training:** Train the model using the Adam optimizer and sparse categorical cross-entropy loss.
8. **Model Evaluation:** Evaluate predictions using accuracy, precision, recall, F1-score, and a confusion matrix.
9. **Genre Prediction:** Test the trained model on an audio file to predict its music genre.

## 🧠 Model Architecture

The CNN model consists of:

- Three Convolutional layers
- Batch Normalization
- Max Pooling layers
- Flatten layer
- Dense layer with ReLU activation
- Dropout for regularization
- Softmax output layer for 10 genre classes

## 📊 Model Performance

The model was evaluated using a separate test dataset.

| Evaluation Metric | Result |
|---|---:|
| Test Accuracy | 27% |
| Test Loss | 3.70 |
| Training Samples | 799 |
| Testing Samples | 200 |
| Number of Genres | 10 |

**Note:** The current model provides baseline results and requires further improvement. Its classification performance is limited, and predictions should not be considered highly reliable.

## 🔍 Prediction Example

The trained model was tested using an audio file from the Blues genre.

- **Actual Genre:** Blues
- **Predicted Genre:** Disco
- **Prediction Confidence:** 26.59%

This example demonstrates the current model's prediction capability and also highlights the need for further optimization.

## 📈 Visualizations

The project includes:

- Mel Spectrogram visualization
- CNN model accuracy graph
- Training and validation loss graph
- Confusion matrix
- Classification report

## 🚀 Future Improvements

- Improve classification accuracy through hyperparameter tuning.
- Apply audio data augmentation techniques.
- Experiment with different CNN architectures.
- Improve feature extraction and data preprocessing.
- Address class-wise prediction performance.
- Explore transfer learning and more advanced audio classification techniques.

## ▶️ How to Run the Project

1. Open the project notebook in Google Colab.
2. Download the GTZAN dataset from Kaggle.
3. Set up the dataset path in the notebook.
4. Install the required Python libraries.
5. Run the notebook cells in sequence.
6. Train and evaluate the CNN model.
7. Test the model using an audio file.

## 📁 Project Files

- `music_genre_classification.ipynb` – Main Jupyter Notebook containing data preprocessing, feature extraction, CNN training, evaluation, and prediction.
- `README.md` – Project documentation.
- `requirements.txt` – Python dependencies.

*Note: The trained model file and original dataset are not included in this repository.*

## 👩‍💻 Author

**Priti Kumari**

GitHub: [Priti356](https://github.com/Priti356)

---

⭐ If you find this project useful, feel free to explore the repository!

# AI Emotion Recognition from Text

## Author
**Shanvi Tripathi**  
B.Tech – CSE (Artificial Intelligence & Machine Learning) 

Email - shanvitripathi023@gmail.com

---

## Project Overview

This project presents an **AI-based emotion recognition system** that analyzes textual input and predicts the emotional tone expressed in the text.

The system uses **Natural Language Processing (NLP)** and **Machine Learning techniques** to classify emotions such as:

- Joy
- Sadness
- Anger
- Fear

Emotion detection from text is widely used in applications such as:

- Sentiment analysis
- Customer feedback analysis
- Social media monitoring
- Mental health analysis

---

## Dataset

The model is trained using an **emotion-labeled dataset** containing text sentences with corresponding emotion labels.

Example dataset entry:
text ; emotion
I feel very happy today ; joy
I feel very sad today ; sadness
This situation makes me angry ; anger
I am scared of this situation ; fear

Dataset files used in the project:

- `train.txt` – Training dataset  
- `test.txt` – Testing dataset  
- `val.txt` – Validation dataset  

---

## Project Architecture

The system follows this pipeline:
Text Input → Text Preprocessing → TF-IDF Vectorization → Naive Bayes Model → Emotion Prediction

---

## Methodology

The project follows these steps:

### 1. Data Loading
The dataset is loaded using **Pandas**.

### 2. Text Preprocessing
Text data is cleaned and prepared for processing.

### 3. Feature Extraction
Text is converted into numerical features using **TF-IDF vectorization**.

### 4. Model Training
A **Multinomial Naive Bayes classifier** is trained on the dataset.

### 5. Prediction
The trained model predicts the emotion of new text input.

---

## Technologies Used

Programming Language:

- Python

Libraries:

- Pandas
- Scikit-learn
- NumPy

Machine Learning Algorithm:

- Multinomial Naive Bayes

Text Processing Method:

- TF-IDF Vectorization

---

## Example Output

Example 1

Input:
I feel very happy today

Output:
Predicted Emotion: joy

Example 2

Input:
I am feeling very sad

Output:
Predicted Emotion: sadness

---

## Model Performance

Approximate model accuracy:
Accuracy ≈ 71%

The performance may vary depending on:

- dataset size
- preprocessing methods
- training parameters

---

## Project Structure

```
AI-Emotion-Recognition-from-Text
│
├── train_model.py        # Script to train the emotion classification model
├── emotion_model.py      # Script to predict emotions from user input
├── train.txt             # Training dataset
├── test.txt              # Testing dataset
├── val.txt               # Validation dataset
├── requirements.txt      # Python dependencies
├── emotion_model.pkl     # Saved trained model
├── vectorizer.pkl        # Saved TF-IDF vectorizer
├── README.md             # Project documentation
└── presentation.pptx     # Project presentation slides
```

---

## Installation

Clone the repository:
git clone https://github.com/Shanvi587/AI-Emotion-Recognition-from-Text.git

Navigate to the project directory:
cd AI-Emotion-Recognition-from-Text

Install dependencies:
pip install -r requirements.txt

---

## Running the Project

Train the model:
python train_model.py

Run emotion prediction:
python emotion_model.py

Example:
Enter text: I feel amazing today
Predicted Emotion: joy

---

## Future Improvements

Possible improvements include:

- Using **Deep Learning models such as LSTM or BERT**
- Increasing dataset size
- Building a **web interface using Flask**
- Deploying the system as an API

---

## References

1. Scikit-learn Documentation  
https://scikit-learn.org

2. Natural Language Processing Resources  
https://www.nltk.org

3. Emotion Dataset for NLP  
https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp

4. TF-IDF Explanation  
https://en.wikipedia.org/wiki/Tf%E2%80%93idf

---

## License

This project is developed for **educational and academic purposes**.

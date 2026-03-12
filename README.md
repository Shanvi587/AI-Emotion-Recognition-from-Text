AI Emotion Recognition from Text using NLP

An AI-based system that detects human emotions from textual input using Natural Language Processing (NLP) and Machine Learning.
The model predicts emotions such as joy, sadness, anger, and fear from sentences.

The system is trained on an emotion-labeled dataset and achieves ~60–90% accuracy depending on training data and preprocessing.

Architecture

Text Processing Pipeline

Text Input
   ↓
Text Preprocessing
   ↓
TF-IDF Vectorization
   ↓
Multinomial Naive Bayes Classifier
   ↓
Emotion Prediction

Model Components

TF-IDF Vectorizer – converts text to numerical features

Multinomial Naive Bayes – classification algorithm

Train/Test Split – 80% training, 20% testing

Dataset

The model is trained on an Emotion Dataset containing thousands of labeled sentences.

Example dataset entries:

i feel very happy today ; joy
i feel lonely and sad ; sadness
this situation makes me angry ; anger
i am scared of this situation ; fear

Emotion classes used in the model:

Joy

Sadness

Anger

Fear

Training Configuration

Algorithm: Multinomial Naive Bayes

Feature Extraction: TF-IDF Vectorization

Train/Test Split: 80% / 20%

Dataset Size: ~20k sentences (if using Kaggle dataset)

Evaluation Metric: Accuracy Score

Results

Example model performance:

Training Step	Accuracy
Initial Training	~60%
After preprocessing improvements	~80–90%

Example predictions

Input

I feel very happy today

Prediction

joy

Input

I am very sad and lonely

Prediction

sadness
Requirements

Python 3.8+

Required libraries:

pandas

scikit-learn

numpy

Install dependencies

pip install -r requirements.txt
Usage

Run the training script

python train_model.py

The script will:

Load the emotion dataset

Convert text into TF-IDF features

Train the machine learning model

Evaluate accuracy

Save the trained model as emotion_model.pkl

Run the prediction script

python emotion_model.py

The program will allow users to enter text and receive predicted emotion.

Example:

Enter text: I feel amazing today
Predicted Emotion: joy
GPU Support

This project runs on CPU since the model is a lightweight machine learning classifier.
No GPU is required.

Project Structure
.
├── train_model.py        # Model training script
├── emotion_model.py      # Emotion prediction script
├── train.txt             # Training dataset
├── test.txt              # Testing dataset
├── val.txt               # Validation dataset
├── requirements.txt      # Python dependencies
├── presentation.pptx     # Project presentation slides
└── README.md             # Project documentation
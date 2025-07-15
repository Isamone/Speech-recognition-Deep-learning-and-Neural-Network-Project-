# Speech-recognition-Deep-learning-and-Neural-Network-Project-
This project uses a deep learning approach to classify IMDB movie reviews as positive or negative based on their textual content. The dataset contains 50,000 labeled reviews and the model is built using Keras with TF-IDF features.

📁 Dataset
Source: IMDB Dataset.csv

Structure:

review: The full text of the movie review

sentiment: Label indicating if the sentiment is positive or negative

🧹 Data Preprocessing
Lowercased all text

Removed HTML tags and URLs using regex

Removed stopwords using NLTK

Converted text into numerical features using TF-IDF Vectorizer (top 5000 features)

🧠 Model
A simple Fully Connected Neural Network with:

Input Layer: 5000 units (TF-IDF features)

Hidden Layers: 512 & 256 units with ReLU activation

Output Layer: 1 unit with Sigmoid (for binary classification)

Loss: BinaryCrossentropy

Optimizer: Adam

🚀 Training
Epochs: 10

Batch size: 64

Validation split: 20% of training data

Achieved validation accuracy of ~87.7%

📊 Evaluation
Test Accuracy: ~87.76%

Loss: Increased steadily in later epochs → suggests overfitting

📈 Visualizations
Two line plots showing:

Training vs Validation Loss

Training vs Validation Accuracy

🧠 Insights & Challenges
Dataset is well-balanced (25K positive, 25K negative)

Overfitting observed after a few epochs

HTML cleaning and stopword removal were critical

Cloud computing (e.g., AWS, GCP) helped speed up training



🛠️ Requirements
pandas, nltk, sklearn, keras, matplotlib

Run nltk.download() for:

stopwords, punkt


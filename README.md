# Spam Classifier

A Machine Learning based **SMS Spam Classifier** built using Python and Natural Language Processing (NLP).

This project classifies SMS messages into two categories:

* **Spam** — unwanted or fraudulent messages
* **Ham** — legitimate messages

The project uses the **SMS Spam Collection** dataset and demonstrates the basic NLP and Machine Learning pipeline for text classification.

## Project Overview

Spam messages are unwanted messages that may contain advertisements, scams, fake offers, or malicious links.

This project uses Natural Language Processing techniques to convert SMS text into numerical features and then uses a Machine Learning classification algorithm to predict whether a message is spam or legitimate.

## Dataset

The project uses the **SMS Spam Collection** dataset.

The dataset contains approximately **5,574 SMS messages**, consisting of:

* 4,827 legitimate (ham) messages
* 747 spam messages

Each record contains a label and the corresponding SMS message.

Example:

```text
ham    Hey, how are you?
spam   Congratulations! You have won a free prize. Call now!
```

## Technologies Used

* Python
* Pandas
* NumPy
* Natural Language Processing (NLP)
* Scikit-learn
* NLTK
* Matplotlib
* Seaborn

## Machine Learning Workflow

The project follows these general steps:

1. Load the SMS dataset
2. Clean and preprocess the text
3. Convert text into numerical features
4. Split the dataset into training and testing sets
5. Train a Machine Learning classification model
6. Predict whether messages are spam or ham
7. Evaluate the model

## Project Structure

```text
SpamClassifier/
│
├── smsspamcollection/
│   ├── SMSSpamCollection
│   └── readme
│
├── Spamclassifier.py
├── README.md
└── .gitignore
```

## Installation

Clone the repository:

```bash
git clone https://github.com/krishnaik06/SpamClassifier.git
```

Move into the project directory:

```bash
cd SpamClassifier
```

Create a virtual environment:

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
source venv/bin/activate
```

Install the required libraries:

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn
```

## Running the Project

Run the Python script:

```bash
python Spamclassifier.py
```

## NLP Techniques

The project demonstrates the use of Natural Language Processing for text classification.

Typical NLP preprocessing steps include:

* Converting text to lowercase
* Removing unnecessary characters
* Tokenization
* Removing stop words
* Text normalization
* Feature extraction

The processed text is then converted into numerical features that can be used by Machine Learning algorithms.

## Model Evaluation

The trained model can be evaluated using common classification metrics such as:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

For spam detection, precision and recall are particularly important because incorrectly classifying legitimate messages as spam can be problematic.

## Example

Input:

```text
Congratulations! You have won a free lottery ticket. Call now!
```

Prediction:

```text
Spam
```

Input:

```text
Hey, are we meeting today?
```

Prediction:

```text
Ham
```

## Future Improvements

Possible improvements to this project include:

* Building a web interface using Flask or Streamlit
* Trying different Machine Learning algorithms
* Hyperparameter tuning
* Improving text preprocessing
* Adding model persistence using Joblib or Pickle
* Deploying the classifier as a web application
* Adding real-time SMS classification

## Author

This project is based on the SpamClassifier repository by **Krish Naik**.

Original Repository:

https://github.com/krishnaik06/SpamClassifier

## License

This repository is intended for educational and learning purposes.

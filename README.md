# Email Spam Classifier

A Machine Learning project to classify emails as spam or not spam (ham). This repository includes a Streamlit app for an interactive demonstration of the classifier.

## Features
- Preprocessing of email text data
- Implementation of a Naive Bayes Classifier
- Visualization of model performance metrics
- Interactive Streamlit app for testing the classifier

## Installation

### Clone the Repository
```bash
git clone https://github.com/prashant-shinde98/Email_spam_classifier.git
cd Email_spam_classifier
```

### Create and Activate a Virtual Environment
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Linux/Mac:
source venv/bin/activate
```

### Install Dependencies
```bash
pip install -r requirements.txt
```

## Steps Followed in the Project
1. **Data Collection:** Used the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) as the base dataset.
2. **Data Preprocessing:**
   - Cleaned and tokenized the email text data.
   - Converted text into numerical features using TF-IDF vectorization.
3. **Model Training:**
   - Trained a Naive Bayes Classifier on the preprocessed data.
   - Evaluated the model's performance using metrics like accuracy, precision, and recall.
4. **Building the App:**
   - Developed an interactive Streamlit app to test the classifier on new inputs.
5. **Deployment:** Prepared the app for local usage with simple setup steps.

## Usage

### Running the Streamlit App
To launch the Streamlit app:
```bash
streamlit run app.py
```

### Testing the Classifier
- Upload a sample email text file.
- The app will classify the email as **Spam** or **Ham**.

## Dataset
This project uses the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) or a similar dataset. Ensure the dataset is properly preprocessed before training the model.

## Project Structure
```
Email_spam_classifier/
├── app.py                   # Streamlit app for the classifier
├── model.py                 # Script for training and saving the model
├── preprocess.py            # Script for data preprocessing
├── requirements.txt         # Required Python packages
└── README.md                # Project documentation
```

### Description of Each File
- **`app.py`:** Contains the Streamlit code to create an interactive web application for testing the spam classifier.
- **`model.py`:** Includes code for training and saving the Naive Bayes Classifier.
- **`preprocess.py`:** Handles data preprocessing tasks like text cleaning and TF-IDF vectorization.
- **`requirements.txt`:** Lists all Python dependencies required to run the project.
- **`README.md`:** Documentation for the project, including setup and usage instructions.

## Model
The Naive Bayes Classifier is trained on preprocessed text features using the following steps:
1. Text cleaning and tokenization
2. Vectorization using TF-IDF
3. Training the Naive Bayes model

## Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author
[Prashant Shinde](https://github.com/prashant-shinde98)

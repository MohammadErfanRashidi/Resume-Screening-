# Resume Classification Project

This project aims to classify resumes based on the job category they belong to. It uses machine learning techniques to analyze the text content of resumes and predict the most likely category.

## Dataset

The project uses the "UpdatedResumeDataSet.csv" dataset, which contains resumes from various job categories. The dataset is preprocessed to clean and prepare the text data for analysis.

## Methodology

1. **Data Cleaning:** Resumes are cleaned to remove irrelevant characters, URLs, hashtags, and special symbols.
2. **Category Encoding:** Job categories are encoded using Label Encoding to convert them into numerical values.
3. **Text Vectorization:** Resumes are transformed into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) to represent their textual content.
4. **Model Training:** A Support Vector Machine (SVC) model is trained on the vectorized resumes and their corresponding categories.
5. **Model Evaluation:** The trained model is evaluated using metrics like accuracy, confusion matrix, and classification report to assess its performance.
6. **Prediction:** A prediction function is defined to classify new resumes based on the trained model.

## Usage

To use the project:

1. Load the necessary libraries and the trained model.
2. Provide a resume as input to the prediction function.
3. The function will return the predicted category for the resume.

## Files

- `UpdatedResumeDataSet.csv`: The dataset used for training and testing.
- `tfidf.pkl`: The TF-IDF vectorizer object.
- `clf.pkl`: The trained SVC model.
- `encoder.pkl`: The Label Encoder object for category encoding.

## Results

The project achieved an accuracy of approximately 99% on the test set. The model shows strong performance in classifying resumes into various job categories.

## Future Work

- Explore other classification algorithms and hyperparameter tuning to further improve model performance.
- Incorporate additional features, such as skills and experience, for a more comprehensive analysis.
- Develop a user interface for easier interaction with the model.

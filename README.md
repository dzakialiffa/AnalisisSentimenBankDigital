# 🧠 Sentiment Analysis: Digital Bank (Seabank)

This project performs sentiment analysis on user reviews of digital banks using the pre-trained **IndoBERT** model. The steps include data preprocessing, model fine-tuning, evaluation, prediction, and visualization of results.

---

## 📁 Project Structure

### 1. 🔧 Environment Setup
- Mount Google Drive to access the dataset and save the model.
- Install and import necessary libraries:
  - `transformers`
  - `pandas`
  - `numpy`
  - `sklearn`
  - `matplotlib`
  - `seaborn`

### 2. 📥 Load Dataset
- The dataset is loaded from Google Drive using `pandas`.
- File format: `.csv` or `.xlsx`
- Columns:
  - `text` (review text)
  - `label` (sentiment)

### 3. 🧹 Data Preprocessing
- **Clean text**: Remove URLs, numbers, special characters, and convert the text to lowercase.
- **Label encoding**: Convert sentiment labels (positive/negative) into numeric values.

### 4. ✂️ Train-Test Split
- Split the dataset into training and testing sets using `train_test_split`.

### 5. 🧾 Tokenization
- Use the IndoBERT tokenizer (`indobenchmark/indobert-base-p1`) from the `transformers` library.
- Input format: `input_ids`, `attention_mask`.

### 6. 🧠 Fine-Tuning the Model
- Model: `BertForSequenceClassification` from HuggingFace.
- Configuration:
  - Epochs: 10
  - Batch size: 32
  - Learning rate: 2e-5
- Utilize the `Trainer` API from HuggingFace.

### 7. 📊 Model Evaluation
- Evaluation metrics:
  - Accuracy
  - Confusion Matrix
  - Classification Report
- Visualizations:
  - Accuracy and loss curves
  - Confusion matrix

### 8. 🔍 Sentiment Prediction
- Function to predict sentiment on new text:
  ```python
  input_text = "This app is really helpful!"
  predict_sentiment(input_text)  # Output: "Positive"

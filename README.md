🧠 Project Goal:
Build a fake news detection system using a pre-trained transformer model with explainability using LIME.

🛠️ Steps Overview:
📦 Libraries Installed & Imported:
Key libraries: transformers, datasets, scikit-learn, nltk, lime
NLP tools and explainability module (LimeTextExplainer)


📊 Dataset:
Dataset loaded from Hugging Face: "Hasib18/fake-news-dataset"
Converted to a Pandas DataFrame for preprocessing.


🧹 Data Preprocessing:
Renamed columns for clarity (text and label)
Split into training and testing sets using train_test_split.


🤖 Model & Tokenizer:
Used DistilBERT (DistilBertTokenizerFast, DistilBertForSequenceClassification)
Tokenized the text data for input to the model.


🧪 Training:
Used HuggingFace Trainer API
Defined TrainingArguments with standard training hyperparameters
Trained on the processed dataset.


📈 Evaluation:
Model evaluated using metrics like accuracy and classification report.
Predictions converted to labels for comparison with ground truth.


🔍 Explainability:
Integrated LIME to explain individual predictions by showing which words contributed most to the classification decision.


✅ Summary:
The notebook implements a DistilBERT-based fake news classifier trained on a labeled dataset with an LIME-based explanation module to interpret results. It covers the full pipeline: dataset loading, preprocessing, training, evaluation, and interpretability.

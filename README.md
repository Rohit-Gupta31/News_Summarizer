# News_Summarizer
A deep learning-based news summarization project using the facebook/bart-large-xsum transformer model, fine-tuned on the Kaggle dataset CNN-DailyMail News Text Summarization. This system generates concise and coherent summaries of lengthy news articles, making information easier to consume.

---

##  Features

- **Automated Summarization**: Generates meaningful summary for any given news article.
- **State-of-the-Art NLP Model**: Built using the **BART transformer model**, specifically fine-tuned for summarization tasks.
- **Streamlined Workflow**: Accepts raw text input or loads articles from a dataset.

---

##  Technologies Used

- **Python**: Primary programming language.
- **Hugging Face Transformers**: For leveraging `facebook/bart-large-xsum`.
- **Kaggle Datasets**: For accessing and managing the CNN-DailyMail dataset.

---

##   How It Works

1. **Data Input**: Input is provided in the form of plain text or from the CNN-DailyMail dataset.
2. **Preprocessing**: The text is tokenized using BART's tokenizer and formatted for model input.
3. **Summarization**: The fine-tuned `facebook/bart-large-xsum` model generates a summary of the input article.
4. **Postprocessing**: Output is decoded and formatted for display.

---

##  Evaluation Metrics

The model's summarization performance was evaluated using ROUGE scores on the validation/test set. These metrics reflect how closely the generated summaries matched human-written ones:

- **ROUGE-1**    : 0.4045
- **ROUGE-2**    : 0.1790
- **ROUGE-L**    : 0.2750
- **ROUGE-LSum** : 0.3747

> ROUGE (Recall-Oriented Understudy for Gisting Evaluation) is a standard set of metrics for evaluating automatic summarization models by comparing generated summaries with reference summaries.

---

##  Setup and Installation

Follow these steps to set up and run the project:

```bash
# Clone the repository
git clone https://github.com/Rohit-Gupta31/News_Summarizer.git
cd News_Summarizer

# Install required libraries
pip install transformers datasets evaluate scikit-learn tqdm

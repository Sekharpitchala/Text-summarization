## 📝 Text Summarization using Pipeline Function

This project implements **automatic text summarization** using the Hugging Face `pipeline` API. It simplifies lengthy text documents into short, meaningful summaries using state-of-the-art NLP models.

## 🚀 Features

- Extractive and abstractive summarization
- Uses **Hugging Face Transformers**
- Easy-to-use summarization via the `pipeline` function
- Web UI integration with Flask (optional)
- Input: Long text or paragraph
- Output: Condensed summary retaining core meaning



## 🛠️ Technologies Used

- **Language**: Python
- **Library**: Hugging Face Transformers
- **Models**: `facebook/bart-large-cnn`, `t5-base`, or any compatible summarization model
- **Optional Web UI**: Flask (Python)
- **Others**: `torch`, `transformers`, `sentencepiece`



## 💡 Sample Code

```python
from transformers import pipeline

# Load summarization pipeline
summarizer = pipeline("summarization")

# Input text
text = """The history of Hyderabad is fascinating and rich with culture. 
It was founded in 1591 by Muhammad Quli Qutb Shah. Later, it became part of the Nizam's rule. 
The city was famous for its pearl and diamond trading centers. Today, it is one of the fastest-growing IT hubs in India."""

# Get summary
summary = summarizer(text, max_length=50, min_length=25, do_sample=False)
print("Summary:", summary[0]['summary_text'])

# Key Features:

Modular Pipeline: The pipeline architecture is modular, allowing for easy customization and integration with other NLP tasks.
State-of-the-Art Model: The NLP model is a leading choice for text summarization, known for its accuracy and robustness.
Parameter Tuning: The pipeline offers flexibility in adjusting parameters like maximum summary length, language, and model weights to tailor the output to specific requirements.
User-Friendly Interface: The pipeline provides a simple API, making it accessible to developers and non-experts alike.


# Usage:

#Installation:
  pip install [NLP, PIPELINE FUNCTION]
  Use code with caution.

# Import:
  Python
  from summarizer import summarize
  Use code with caution.

# Summarize Text:
 Python
 text = "Your long text here"
 summary = summarize(text, max_summary_length=100, language="en")
 print(summary)
 
# Customization Options:

Maximum Summary Length: Control the length of the generated summary.
Language: Specify the language of the input text.
Model Weights: Experiment with different model weights to fine-tune the summarization process

# Contributing:

We welcome contributions from the community. Please refer to the CONTRIBUTING.md file for guidelines.

## License:

This project is licensed under the  CITD-MSME (https://citdindia.org/index.php)

## 👨‍💻 Author
Pitchala Sekhar
GitHub: [Sekharpitchala](https://github.com/Sekharpitchala)
Email: sekharpitchala2003@gmail.com 

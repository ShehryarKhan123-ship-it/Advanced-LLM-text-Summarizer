# 🚀 LLM-Based Multilingual Document Summarizer

This project is a **Gradio web app** that uses **state-of-the-art transformer models** to summarize text from `.txt`, `.pdf`, and `.docx` files. It supports **multilingual input**, **automatic translation to English**, and **smart chunking** for long documents.

![Demo](https://via.placeholder.com/800x400?text=Document+Summarizer+Demo) *Example interface screenshot*

## ✅ Features

- 📄 **Supports Multiple File Formats**: `.txt`, `.pdf`, `.docx`
- 🌐 **Multilingual Translation**: Auto-detect and translate non-English to English before summarizing
- 🔍 **Smart Chunking**: Splits large text by sentences to preserve context
- 🧠 **Model Options**: BART, DistilBART, PEGASUS
- 📥 **Downloadable Summary Output**
- ⚙️ **Custom Summary Length Options**
- 🧾 **Interactive Summary Analysis**
- 🗂 **Batch File Uploads and Summaries**

## 🔧 Installation

1. Install required packages:
```bash
pip install gradio transformers sentencepiece pdfplumber python-docx langdetect nltk
```
## Download NLTK data:
```python
import nltk
nltk.download('punkt')
```
## 🧪 How to Use
Run the script and open the Gradio interface in your browser
Choose between:
Pasting raw text to summarize
Uploading files to process
Select your preferred:
Summarization model
Output length
View or download your results

## 💡 Example
### Input Paragraph:
```text
Climate change is one of the most pressing global challenges of our time, affecting ecosystems, human health, and economies worldwide. Rising global temperatures, melting ice caps, and extreme weather events like hurricanes and wildfires have become increasingly common...
```
### Model Output Summary:
```text
Rising global temperatures, melting ice caps, and extreme weather events like hurricanes and wildfires have become increasingly common. Scientists attribute these changes largely to human activities, such as the burning of fossil fuels and deforestation. Governments and organizations around the world are advocating for urgent climate action.
```
# 🧠 Available Models

| Model Name                      | Description                              |
|--------------------------------|------------------------------------------|
| `facebook/bart-large-cnn`      | High-quality summaries, larger model     |
| `sshleifer/distilbart-cnn-12-6`| Lightweight, faster inference             |
| `google/pegasus-xsum`          | Best for short, abstractive summaries     |

# 🚀 Running the App

## Run Locally:

```bash
python app.py
```
### Gradio Web App
```python
!pip install gradio transformers sentencepiece pdfplumber python-docx langdetect nltk
import gradio as gr
# Paste your full app code here
```

# 📦 Future Enhancements

- 🧾 **OCR for scanned PDFs**  
  Enable text extraction from scanned documents using Optical Character Recognition.

- 🎙️ **Speech-to-summary using Whisper**  
  Allow users to upload audio files and get summaries via OpenAI's Whisper model.

- 🌐 **Summary translation output**  
  Automatically translate summaries back into the user's preferred language.

- 🔐 **API support for production use**  
  Provide secure API endpoints for integrating the summarization service into other platforms.

- 📊 **Comparative analysis of multiple summaries**  
  Generate and compare outputs from different models for deeper insight and benchmarking.

# 🤝 Contributing
We welcome contributions! Please fork the repository and submit a pull request with your improvements.
# 📄 License
This project is open-source under the MIT License.

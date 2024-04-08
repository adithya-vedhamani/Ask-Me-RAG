# Ask Me RAG

## Features

- **Real-time Insights**: Extracts and analyzes text from uploaded PDF documents to provide immediate insights.
- **Advanced Generative AI**: Utilizes Google's cutting-edge Generative AI model, Gemini-PRO, for delivering high-quality, contextually relevant responses.
- **Secure API Key Handling**: Ensures the safe and secure input of Google API keys for accessing generative AI models.

## Getting Started

### Prerequisites

- Google API Key: Obtain a Google API key to interact with Google's Generative AI models. Visit [Google API Key Setup](https://makersuite.google.com/app/apikey) to obtain your key.
- Streamlit: This application is built using Streamlit. Make sure you have Streamlit installed in your environment.

### Installation

Clone this repository or download the source code to your local machine. Navigate to the application directory and install the necessary Python packages:

```bash
pip install -r requirements.txt
```

### How to Use

```bash
pip install -r requirements.txt
python -m streamlit run <path_to_script.py>nts.txt
```
### Providing Your Google API Key
Securely enter your Google API key when prompted. This key enables the application to access Google's Generative AI models.

### Uploading PDF Documents
You can upload one or multiple PDF documents. The application will analyze the content of these documents to respond to queries.

### Asking Questions
Once your documents are processed, feel free to ask any questions related to the content of your uploaded documents.

### Technical Overview
**PDF Processing:** Utilizes PyPDF2 for extracting text from PDF documents.
**Text Segmentation:** Employs the RecursiveCharacterTextSplitter from LangChain for segmenting the extracted text into manageable chunks.
**Vector Store Creation:** Uses FAISS for creating a searchable vector store from text chunks.
**Response Generation: **Leverages ChatGoogleGenerativeAI from LangChain for generating responses to user queries based on the contextual information provided by the uploaded documents.
vbnet

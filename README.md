# Chat with Multiple PDFs using Gemini & LangChain

Demo Video Link :- https://drive.google.com/file/d/1iuYN-xyXzwppyyYwUfrXj1hbAcsuCPWb/view?usp=sharing

This project allows users to upload multiple PDF files and ask questions based on their content. It uses **Google's Gemini** for embeddings and answering, along with **LangChain**, **FAISS**, and **Streamlit**.

---

## Features

- Upload and process multiple PDF files
- Extract and split text into chunks
- Generate embeddings using Google Generative AI
- Store and search vectors using FAISS
- Answer user questions based on PDF content using Gemini
- User-friendly Streamlit interface

---

## Technologies Used

- Streamlit
- PyPDF2
- LangChain
- Google Generative AI (Gemini)
- FAISS
- dotenv

---

## Setup Instructions

### 1. Clone the Repository


### 2. Create a Virtual Environment (optional)


### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API Key

Create a `.env` file in the project root:

```
GOOGLE_API_KEY=your_google_generative_ai_key
```

### 5. Run the Application

```bash
streamlit run app.py
```

---

## How It Works

1. User uploads one or more PDF files.
2. The app extracts and splits the text into chunks.
3. It generates embeddings using Gemini and stores them using FAISS.
4. When the user asks a question, relevant chunks are retrieved.
5. Gemini answers the question based on the context of the documents.

- If an answer is not in the PDF, the response will be:  
  `"answer is not available in the context"`
- Make sure to stay within API usage limits.

# PDF Conversational Bot using Google Gemini AI
This project implements an AI-powered chatbot that answers questions based on uploaded PDF documents. Using Google’s Gemini AI for generative responses and FAISS for efficient document search, the chatbot provides precise answers by retrieving relevant sections from the PDFs.

## Features
- PDF Upload: Users can upload one or multiple PDF files.
- Efficient Retrieval: Uses FAISS for fast document search based on semantic similarity.
- Conversational AI: Google Gemini AI (gemini-pro) generates responses using the context from the PDFs.
- Context-Aware Responses: If the required information is not present in the PDFs, the bot will indicate that no relevant answer was found.
## Project Architecture
- Streamlit: User interface for uploading PDFs and asking questions.
- FAISS: Vector store for storing and searching document embeddings.
- Google Gemini AI: Used for generating text embeddings and generative responses.
- LangChain: Chains document retrieval and generative responses into a seamless workflow.
## Setup Instructions
### Prerequisites
  Python 3.9 or higher
  Google Gemini AI API key (Get it from Google Cloud)
  FAISS library installed
  A .env file with your Google API key:
    GOOGLE_API_KEY=your_google_api_key
### Installation
  1. Clone the repository:
     git clone https://github.com/your-username/pdf-conversational-bot.git
     cd pdf-conversational-bot
  2. Install Dependencies:
     pip install -r requirements.txt
  3. Set up environment variables in the .env file:
     GOOGLE_API_KEY=your_google_api_key
  4. Run the Streamlit app:
     streamlit run app.py
### Usage Instructions
1. Upload PDFs: In the Streamlit sidebar, upload one or multiple PDF files.
2. Process PDFs: After uploading, click the 'Process' button to extract and store 
   document information.
3. Ask a Question: Type your question in the main text box and press 'Enter'.
4. View the Response: The chatbot will display a detailed response based on the       
   provided context. If no relevant context is found, it will inform the user   
   accordingly.





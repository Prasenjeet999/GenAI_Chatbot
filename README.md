# GenAI_Chatbot: PDFs Conversational Assistant
GenAI Chatbot that can take your pdf docs and give you insights.

This project provides a conversational assistant for interacting with PDF files using Generative AI (Google Gemini). With this tool, you can upload PDF files and ask questions based on their content, receiving detailed and accurate responses.

- Watch the demo video below to see the application in action:
<div align="left">
  <a href="https://www.youtube.com/watch?v=b33nWBskZ10">
    <img src="https://img.youtube.com/vi/b33nWBskZ10/maxresdefault.jpg" alt="Watch the video" style="width:70%; max-width:600px;">
  </a>
</div>

## Features
- Upload multiple PDF files.
- Extract and split text from PDF files into manageable chunks.
- Generate vector embeddings using Google Generative AI.
- Perform similarity searches on the text chunks.
- Answer questions based on the context from the PDF files.

## Installation
1. Clone the repository
2. Create a virtual environment and activate it
3. Install the required dependencies
4. Set up environment variables

## Usage
1. Run the STreamlit application
2. Open the provided URL in your web browser.
3. Upload your PDF files via the sidebar.
4. Ask questions in the main interface based on the content of your uploaded PDFs.

## Code Overview
- `get_pdf_text(pdf_docs)`: Extracts text from the uploaded PDF files.
- `get_text_chunks(text)`: Splits the extracted text into smaller chunks for better processing.
- `get_vector_store(text_chunks)`: Generates vector embeddings and stores them using FAISS.
- `get_conversational_chain()`: Sets up the question-answering chain with a custom prompt template.
- `user_input(user_question)`: Handles user queries, performs similarity search, and provides responses.
- `main()`: Main function to set up the Streamlit interface and handle user interactions.

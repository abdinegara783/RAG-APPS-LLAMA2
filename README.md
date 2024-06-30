# PDF Chatbot with LangChain and Chainlit

This project implements a conversational AI chatbot that interacts with users by processing and understanding PDF documents. It leverages the power of LangChain, PyPDF2, Chainlit, and GROQ language models to provide an efficient and interactive experience.

## Features

- **PDF Processing**: Upload a PDF file to extract and process its text content.
- **Conversational AI**: Interact with the chatbot to ask questions about the content of the uploaded PDF.
- **Vector Store**: Utilizes Chroma vector store for efficient text retrieval.
- **Memory Management**: Maintains conversational context using ConversationBufferMemory.

## Setup

### Prerequisites

- Python 3.8 or higher
- [GROQ API Key](https://groq.com/api-key) (Sign up to obtain your API key)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/abdinegara783/RAG-APPS-LLAMA2.git
    cd RAG-APPS-LLAMA2
    ```

2. Create a virtual environment:
    ```sh
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the root directory and add your GROQ API key:
    ```env
    GROQ_API_KEY=your_groq_api_key
    ```

## Usage

1. Start the application:
    ```chainlit run app_new.py
    ```

2. Open your web browser and navigate to the provided URL.

3. Upload a PDF file when prompted.

4. Once the PDF is processed, you can start asking questions about its content.

## Example

```markdown
📄 **Upload a PDF file to begin!**
🔄 **Processing your file...**
✅ **Processing complete. You can now ask questions!**

**User**: What is the main topic of the first chapter?
**Bot**: The main topic of the first chapter is about the introduction to AI and its applications.

**Sources:** source_0, source_1

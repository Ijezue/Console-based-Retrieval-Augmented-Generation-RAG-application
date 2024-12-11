# Console-based-Retrieval-Augmented-Generation-RAG-application

This project builds an AI-based chatbot to interact with PDF files. The code is designed to run seamlessly in Google Colab but can also be executed locally with minor modifications.

## How to Run the Code

### Running in Google Colab

1. **Open the Notebook**
   - Open Google Colab and Load the file `Console_based_RAG_application.ipynb`.

2. **File Upload**
   - Create a folder named `myfiles` in your Colab environment under the `/content/` directory.
   - Upload all your PDF files into the `myfiles` folder.

3. **Run the Code**
   - Execute all cells in the notebook sequentially, starting from the first cell and proceeding to the last.

4. **Interaction**
   - Type in your questions to interact with the chatbot.
   - Type `exit` to quit the chatbot.

### Running Locally

If you prefer to run the code on your local machine, follow the steps below:

1. **Set Up a Virtual Environment**
   - Install the required modules using the following command:
     ```
     pip install langchain chromadb pypdf langchain_community sentence_transformers langchain_huggingface pyngrok streamlit langchain-groq
     ```

2. **Edit the Code**
   - Update the following lines in the code to reflect your local setup:
     - **`PERSIST_DIRECTORY`**: Update the line
       ```python
       PERSIST_DIRECTORY = "/content/chroma_db/"
       ```
       to your preferred directory path, preferably in the same folder as the `.ipynb` file.

     - **`FOLDER_PATH`**: Update the line
       ```python
       FOLDER_PATH = "/content/myfiles"
       ```
       to the path where your documents are stored, preferably in the same folder as the `.ipynb` file.



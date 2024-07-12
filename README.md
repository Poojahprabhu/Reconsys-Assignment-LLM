# Reconsys-Assignment-LLM

Objective: Develop a RAG-based question-answering system that allows users to upload a document, ask questions about its content, and receive relevant answers.

- This repository contains a Python script that uses Hugging Face's BERT model for Question Answering on documents in PDF and TXT formats. The script provides a simple interface to upload a document, process the text, and ask questions based on the content of the document.

#Features
-Extract text from PDF and TXT files.
-Clean and preprocess the extracted text.
-Split the text into manageable chunks.
-Use Hugging Face's BERT model for Question Answering.
-Provide an interface for users to upload documents and ask questions.

#Requirements
-Python 3.6 or higher
-IPython
-ipywidgets
-pdfminer.six
-transformers
-torch

#Installation
- Clone the repository.
- Create a virtual environment and activate it.
- Install the required packages.

#Usage
- Run the IPYNB in an Google colab or Jupyter Notebook environment.

- Upload a document (PDF or TXT) using the provided file upload widget.

- Ask questions based on the uploaded document using the text input and submit button.

#Output Images 

![348246263-6a4ba46b-a695-47ea-b5eb-b656afc69876](https://github.com/user-attachments/assets/5be905cc-90b9-4e56-ab9f-b7629c6a44a4)
![348246636-11b12560-9d7b-427d-b35e-5113876a88db](https://github.com/user-attachments/assets/bf57fa2c-a9fc-4760-857e-5826d3d7a772)


#Assignment Criteria fullfilled
- The BERT_(Hugging_face).ipynb file consists of code utilising the BERT (Hugging face) model to generate answers to the questions.
#Requirements fulfilled:

Document Upload:

Implement a function to accept and process PDF or TXT files - handle_upload()

Extract text content from the uploaded document. - extract_text_from_pdf(), extract_text_from_txt()

Text Preprocessing:

Implement basic text cleaning (remove special characters, extra whitespace). - clean_text()

Split the document into smaller chunks or passages. - split_into_chunks()

Question Processing:

Implement a function to accept user questions as input. - process_question()
Answer Generation:

Choose an LLM (e.g., GPT-3, BERT, T5) for answer generation.

Construct a prompt using the retrieved chunks and the user's question.

Generate an answer using the LLM. - generate_answer()

User Interface:

Create a simple command-line interface or web application that allows users to: - Implemented using widgets

a. Upload a document

b. Ask questions

c. View generated answers

Limitations:
- Processing time - The model takes 5 to 10 seconds to generate answer for documents with 10000 to 15000 words.
- Error handling - The api may throw unexpected runtime error

Scope to improvement:
- Handling runtime errors
- Fine tuning the model
- Testing for several use cases

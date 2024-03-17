# MultiPDF Chat App

## Overview
MultiPDF Chat App is a Python-based tool allowing interaction with multiple PDF documents through a chat interface. Users can inquire about the contents of the loaded PDFs in natural language, and the app responds with pertinent information, utilizing an advanced language model for precise and accurate answers.

**Note:** Responses are confined to the context of the loaded PDFs.

## Workflow
### 1. PDF Loading
The application scans multiple PDF files and extracts the text within them.

### 2. Text Chunking
The obtained text is fragmented into manageable chunks, ready for processing.

### 3. Language Model Integration
A sophisticated language model is employed to convert text chunks into vector representations (embeddings).

### 4. Similarity Matching
User queries undergo comparison with text chunks to pinpoint the ones with the highest semantic resemblance.

### 5. Response Generation
The isolated chunks are processed by the language model to formulate responses congruent with the PDFs’ content.

## Setup and Installation
1. Clone the repository to your local environment.
2. Install necessary dependencies using:
   ```sh
   pip install -r requirements.txt
   ```
3. Secure an API key from OpenAI and integrate it into the `.env` file located in the project directory:
   ```env
   OPENAI_API_KEY=<your_api_key>
   ```

## How to Use
1. Confirm the installation of dependencies and the integration of the OpenAI API key in the `.env` file.
2. Launch `app.py` using the Streamlit CLI:
   ```sh
   streamlit run app.py
   ```
3. The app will open in your default web browser, presenting the UI.
4. Upload multiple PDF documents following the on-screen instructions.
5. Interact with the app using natural language queries regarding the uploaded PDFs.

## Contributions
This project is primarily educational and supports a YouTube tutorial illustrating the construction of the app. While further contributions are not currently accepted, you are encouraged to adapt and expand the app to suit your needs.

## License
MultiPDF Chat App is distributed under the MIT License. Enjoy experimenting with and building upon this project!

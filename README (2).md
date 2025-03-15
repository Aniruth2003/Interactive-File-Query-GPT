# Interactive File Query GPT 🎈

**Interactive File Query GPT** is a Streamlit-based application that allows users to upload various file formats (PDF, PPT, TXT, Audio) and query the extracted content using a locally available AI model.

## Features 🚀
- **Supports multiple file formats**: PDF, PPT, TXT, and Audio files (WAV, MP3).
- **AI-powered text extraction & querying**: Uses `Ollama` for vector embeddings and document retrieval.
- **Multi-query retrieval**: Generates multiple versions of user questions to improve document search.
- **Whisper integration**: Transcribes audio files using OpenAI Whisper.
- **PDF page visualization**: Displays uploaded PDFs as images for better visualization.

## Installation 🛠️

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- pip
- `ffmpeg` (for audio processing)

### Clone the Repository
```sh
git clone https://github.com/your-repo/interactive-file-query-gpt.git
cd interactive-file-query-gpt
```

### Install Dependencies
```sh
pip install -r requirements.txt
```

## Usage 🏃

### Run the Application
```sh
streamlit run app.py
```

### Upload and Query Files
1. Upload a **PDF, PPT, TXT, or Audio** file.
2. Select a locally available **AI model**.
3. Ask questions related to the document.
4. View extracted **text**, **transcriptions**, or **PDF pages**.
5. Delete the vector database if needed.

## Dependencies 📦
- **Streamlit**: UI framework
- **Ollama**: LLM-based embeddings
- **LangChain**: Document processing & querying
- **pdfplumber**: PDF text extraction
- **Whisper**: Audio transcription
- **Chroma**: Vector database
- **Pillow**: Image processing
- **pptx**: PowerPoint file handling

## Troubleshooting ❓
- If Whisper fails to transcribe, ensure `ffmpeg` is installed:
  ```sh
  sudo apt install ffmpeg  # Linux
  brew install ffmpeg      # MacOS
  ```
- If `Ollama` models are not available, install them manually:
  ```sh
  ollama pull nomic-embed-text
  ollama pull any-other-model
  ```

## License 📜
This project is licensed under the **MIT License**.

## Author 👨‍💻
Developed by **[Your Name]**.

---

Enjoy using **Interactive File Query GPT**! 🚀🔥

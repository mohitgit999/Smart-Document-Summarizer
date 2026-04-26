# Smart Document Summarizer

An AI-powered web application that generates concise, detailed, or bulleted summaries of text and documents. Built with Python, Flask, and the Groq API utilizing the `llama-3.1-8b-instant` model for fast and intelligent text summarization.

## Features

- **Document Support**: Upload and extract text directly from `.txt`, `.pdf`, and `.docx` files.
- **Text Summarization**: Paste text directly for instant summarization.
- **Customizable Styles**: Choose between three summarization styles:
  - *Concise*: 2-3 clear sentences capturing key points.
  - *Detailed*: 5-7 sentences covering all major points and details.
  - *Bulleted*: 5-7 bullet points for quick scannability.
- **Word Count Statistics**: See the exact word count reduction and original vs. summary word counts.
- **Responsive UI**: A modern, user-friendly interface that works on all devices.

## Tech Stack

- **Backend**: Python, Flask
- **AI Integration**: Groq API (OpenAI Python Client)
- **Document Processing**: `pypdf`, `python-docx`
- **Frontend**: HTML, CSS, JavaScript

## Installation and Setup

### Prerequisites
- Python 3.8+
- A Groq API Key

### Local Development

1. **Clone the repository** (if applicable) or navigate to the project directory:
   ```bash
   cd "Smart Document Summerizer"
   ```

2. **Create a virtual environment**:
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

5. **Configure Environment Variables**:
   Create a `.env` file in the root directory and add your Groq API key:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

6. **Run the Application**:
   ```bash
   python app.py
   ```
   The application will be running at `http://127.0.0.1:5000`.

## Deployment

This project includes configuration files for deployment on platforms like Render or Vercel.
- **Vercel**: A `vercel.json` file is included for seamless serverless deployment.
- **Render**: The `requirements.txt` includes `gunicorn`, making it ready for a web service deployment on Render. Ensure the build command is `pip install -r requirements.txt` and the start command is `gunicorn app:app`.

## Usage

1. Open the application in your browser.
2. Type or paste the text you want to summarize, OR upload a supported document (.txt, .pdf, .docx).
3. Select your preferred summary style (Concise, Detailed, or Bullet Points).
4. Click "Summarize" and view the AI-generated result along with reduction statistics.


Created By 
Mohit Kumar ,
Kumari Yukti

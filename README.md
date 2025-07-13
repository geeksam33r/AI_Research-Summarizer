Smart Assistant for Research Summarization

This project is a personal attempt to create a smart research assistant web app. It helps users upload a research paper (PDF), summarizes the document, and allows them to ask questions related to the content — all from a user-friendly interface.

Features

- Upload and read research papers in PDF format
- Generate a simple summary from the document
- Ask custom questions and get relevant answers
- Uses a powerful backend model to understand document context
- Built with a modern frontend using React and backend using FastAPI

Technologies Used

- **Frontend**: React.js
- **Backend**: FastAPI (Python)
- **PDF Parsing**: PyMuPDF
- **AI Integration**: OpenAI's API
- **API Communication**: REST via Fetch API

Project Structure

smart-assistant/
│
├── backend/                 
│   └── main.py             
│
├── smart-assistant/        
│   └── src/
│       └── App.js           
│
├── README.md

How to Run It

1. Clone the Project

bash
git clone https://github.com/yourusername/smart-assistant.git
cd smart-assistant

2. Set Up Backend
   
bash
cd backend
pip install fastapi uvicorn python-multipart openai pymupdf
uvicorn main:app --reload

3. Set Up Frontend
bash
cd ../smart-assistant
npm install
npm start

4. Add Your API Key

Update the file `main.py` to include your OpenAI API key:
python
openai.api_key = "your-api-key-here"

WORKING

1. A PDF file is uploaded via the web interface
2. The backend extracts the text using PyMuPDF
3. The app provides a summary or answers based on user questions
4. Everything is served and displayed via a React web interface




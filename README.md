# AI Voice-Enabled Chatbot

This project is a web-based chatbot that you can interact with using your voice. It uses speech recognition to capture your questions, sends them to Google's Gemini AI for a response, and then uses text-to-speech to speak the answer back to you.

## Features

- Voice input and output
- Integration with Google Gemini for intelligent responses
- Web-based interface

## Technologies Used

- Django
- Google Generative AI (Gemini)
- gTTS (Google Text-to-Speech)
- JavaScript (for frontend interactions)

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your environment variables:**
    - Create a file named `.env` in the root of the project.
    - Add the following line to the `.env` file, replacing `your_api_key` with your actual Google API key:
      ```
      GOOGLE_API_KEY=your_api_key
      ```

5.  **Run the development server:**
    ```bash
    python manage.py runserver
    ```

6.  Open your web browser and go to `http://127.0.0.1:8000/`.

## Usage

- Click the "Start Listening" button and speak your question.
- The chatbot will process your request and respond with voice.

## Project Structure

```
.
├── manage.py
├── requirements.txt
├── settings.py
├── static/
│   └── ...
├── templates/
│   └── index.html
├── urls.py
└── views.py
```
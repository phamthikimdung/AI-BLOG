# YouTube to Blog Generator

This Django-based web application allows users to convert YouTube videos into comprehensive blog articles.
The application leverages YouTube video processing, audio transcription, and AI-based text generation to create blog content.

## Features

- User authentication (sign up, log in, log out)
- Extracts audio from YouTube videos
- Transcribes audio using AssemblyAI
- Generates blog articles from transcripts using OpenAI
- Stores and displays generated blog articles

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x
- Django
- pytube
- assemblyai
- openai

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    ```

2. Navigate to the project directory:
    ```bash
    cd your-repository-name
    ```

3. Create a virtual environment:
    ```bash
    python -m venv env
    ```

4. Activate the virtual environment:
    - On Windows:
        ```bash
        .\env\Scripts\activate
        ```
    - On macOS/Linux:
        ```bash
        source env/bin/activate
        ```

5. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

6. Set up your environment variables:
    Create a `.env` file in the project root and add the following:
    ```bash
    OPENAI_API_KEY=your-openai-api-key
    ASSEMBLYAI_API_KEY=your-assemblyai-api-key
    ```

7. Apply migrations:
    ```bash
    python manage.py migrate
    ```

8. Run the development server:
    ```bash
    python manage.py runserver
    ```

## Usage

1. Open your web browser and go to `http://127.0.0.1:8000/`.

2. Sign up for a new account or log in if you already have an account.

3. On the main page, you can enter a YouTube video link to generate a blog article.

4. View your generated blog articles on the "All Blogs" page.

## Project Structure

- `views.py`: Contains the main views for handling user requests.
- `models.py`: Defines the `BlogPost` model used to store blog articles.
- `templates/`: Contains HTML templates for rendering web pages.
- `urls.py`: URL routing configuration.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature`).
6. Create a Pull Request.

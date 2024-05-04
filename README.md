# SQL Chat

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Welcome to SQL Chat! This is an interactive chat application that allows you to connect to your MySQL database and ask questions in natural language. It leverages the power of LangChain, ChatGroq, and Streamlit to provide a seamless conversational experience.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- Connect to a MySQL database using user-provided connection details.
- Chat with your MySQL database using natural language queries.
- Leverage LangChain's capabilities to generate SQL queries based on user questions.
- Convert SQL responses into natural language for easy understanding.
- Persistent conversation history throughout the chat session.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/Soumya-Kushwaha/SQL-Chat.git
    ```

2. Navigate to the project directory:

    ```bash
    cd SQL-Chat
    ```

3. Create a virtual environment and activate it:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # For macOS/Linux
    # OR
    venv\Scripts\activate.bat  # For Windows
    ```

4. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

5. Create a `.env` file in the root directory with your Groq Free API:

    ```
    GROQ_API_KEY = "groq api key"
    ```

## Configuration

The project requires configuration for MySQL connection, by manually entering the connection details in the sidebar within the app.

## Usage

1. Launch the application:

    ```bash
    streamlit run app.py
    ```

2. Connect to your MySQL database using the sidebar in the app.

3. Start asking questions about your database in natural language using the chat input box.

4. The application will provide SQL queries and natural language responses to your questions.

## Contributing

Contributions to the project are welcome! Please open an issue or submit a pull request if you find any bugs or have ideas for improvements.

## License

This project is licensed under the [MIT License](LICENSE).

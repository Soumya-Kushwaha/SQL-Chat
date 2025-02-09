# SQL Chat 🗣️ 

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Overview
SQL Chat is an intelligent conversational interface that enables natural language interactions with MySQL databases. Built with Streamlit, LangChain, and ChatGroq, it transforms complex SQL queries into simple conversations, making database exploration accessible to users of all technical levels.

## Features

### 🔌 Easy Database Connection
- Simple MySQL database connection through an intuitive UI
- Secure credential management
- Support for custom host, port, and database configurations

### 💬 Natural Language Interface
- Ask questions about your database in plain English
- Get responses in both SQL and natural language
- Maintains conversation context for more relevant answers

### 🤖 Intelligent Query Generation
- Powered by ChatGroq's Mixtral-8x7b-32768 model
- Automatically generates optimized SQL queries
- Converts technical SQL results into human-readable responses

### 🔄 Interactive Chat Experience
- Real-time query processing
- Persistent conversation history
- Clean and intuitive chat interface

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/sql-chat.git
cd sql-chat
```

2. Create and activate a virtual environment:
```bash
# For Unix/macOS
python3 -m venv venv
source venv/bin/activate

# For Windows
python -m venv venv
venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up your environment variables:
```bash
# Create .env file and add your Groq API key
echo "GROQ_API_KEY=your_api_key_here" > .env
```

## Dependencies
```
streamlit==1.31.1
langchain==0.1.8
langchain-community==0.0.21
langchain-core==0.1.24
langchain-openai==0.0.6
mysql-connector-python==8.3.0
groq==0.4.2
langchain-groq==0.0.1
python-dotenv
```

## Usage

1. Start the application:
```bash
streamlit run app.py
```

2. Configure your database connection in the sidebar:
   - Enter hostname (default: localhost)
   - Specify port (default: 3306)
   - Provide username and password
   - Select database name

3. Click "Connect" to establish database connection

4. Start chatting with your database:
   - Ask questions in natural language
   - View SQL queries and their translations
   - Explore your data through conversation

## Example Queries
```
"Show me the top 5 customers by total orders"
"What was the average order value last month?"
"List all products that are out of stock"
```

## Contributing

1. Fork the repository
2. Create your feature branch:
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add amazing feature'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/amazing-feature
   ```
5. Open a Pull Request

## Security Considerations
- Database credentials are handled securely and not stored permanently
- Sensitive information is masked in the UI
- All database connections are session-specific

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Powered by [LangChain](https://python.langchain.com/)
- Uses [ChatGroq](https://groq.com/) for natural language processing

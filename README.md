# Chatbot Q&A for Retail Store

## Introduction
This project is a sophisticated Chatbot Q&A system, specifically designed for retail store interactions. It leverages Google's Palm model through LangChain, coupled with Streamlit for front-end development, to provide intuitive and accurate responses to customer queries about retail products.

## Features
- AI-driven responses using Google's Palm model.
- Integration with SQL databases for dynamic query handling.
- Streamlit-powered user interface for interactive query input and response display.
- Utilization of Semantic Similarity and Chroma for enhancing response accuracy.
- Special handling of complex or exceptional cases through custom logic.

## Requirements
The project depends on several Python libraries as listed in `requirements.txt`, including LangChain, Python-dotenv, Streamlit, TikToken, Faiss-CPU, and more.

## Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/DeependraVerma/Chatbot-Q-A---Retail-Store.git]
   ```
2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure the `.env` file to include `GOOGLE_API_KEY`.

## Project Structure
- `langchain_helper.py`: Sets up the LangChain with GooglePalm and connects to the SQL database. It initializes Chroma for vector storage and Semantic Similarity for example selection.
- `main.py`: The Streamlit application that serves as the front-end, allowing users to input questions and view answers.
- `few_shots.py`: Manages scenarios where the model requires additional context or specific use-case handling.
- `test.ipynb`: A Jupyter notebook for preliminary testing and research.
- `requirements.txt`: Lists all the necessary Python packages.
- `.env`: A configuration file for storing sensitive data like the `GOOGLE_API_KEY`.

## Usage
To start the Streamlit app:
```bash
streamlit run main.py
```
Users can input their queries, and the system will provide relevant answers using the chatbot's intelligent processing capabilities.

## Contributing
Contributions are welcome. Please follow the standard fork-and-pull request workflow.

## License
This project is distributed under the Apache License. See the `LICENSE` file for more information.
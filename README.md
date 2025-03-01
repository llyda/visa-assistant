# Visa Assistant Project

Visa Assistant is an AI-powered chatbot that helps users check visa requirements based on their passport and travel destination.


## Features

- Determine visa requirements for travel between countries.
- Interactive chat interface for user engagement.
- Supports visa-free, visa-on-arrival, and visa-required scenarios.
- Easy-to-update visa information using JSON files.

## Prerequisites

- Python 3.8 or higher
- Virtual environment (optional but recommended)

## Instructions to Run the Project

**Clone the Repository**
   - Open your terminal or command prompt.
   - Run the command: `git clone https://github.com/llyda/visa-assistant.git`
   - Navigate into the project directory: `cd visa-assistant`

**Setup Virtual Environment (Optional)**
   - Create a virtual environment: `pyenv virtualenv 3.8.12 airbot`
   - Activate the virtual environment:
     - On macOS/Linux: `pyenv activate airbot`

**Install Dependencies**
   - Run the command: `pip install -r requirements.txt`

**Setup Environment Variables**
   - Create a `.env` file in the project root directory.
   - Add your OpenAI API key to the `.env` file: `OPENAI_API_KEY=your_openai_api_key_here`

**Run the Project**
   - Open the `visa_assistant.ipynb` notebook in the `notebooks/` directory.

**Interact with the Assistant**:
   - Type your messages in the text field, click Send, and review the AI responses.

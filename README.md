# Visa Assistant Project

Visa Assistant is an AI-powered chatbot that helps users check visa requirements based on their passport and travel destination. Built with OpenAI's function calling and natural language processing, it provides accurate and conversational visa information.

---
## Features
- **Visa Status Identification**:
  
  Checks visa requirements for travel between countries, including:

  - Visa-free travel
  - Visa-on-arrival
  - Visa-required scenarios

- **Interactive Chat Interface**:\
  User-friendly interface built with Jupyter Notebook and `ipywidgets`.

- **Dynamic Data Updates**:\
  Easy-to-update visa information using JSON files.

- **Natural Language Processing**:\
  Supports multi-turn conversations with context awareness.

- **Error Handling**:\
  Handles invalid inputs and missing data.
---
## Prerequisites

- **Python 3.8 or higher**
- **pyenv** (for Python version management)
- **Jupyter Notebook**
- **OpenAI API Key**
---
## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/llyda/visa-assistant.git
cd visa-assistant
```

### 2. Set Up Python Environment with `pyenv`

1. Install Python 3.8.12 using `pyenv`:

```bash
pyenv install 3.8.12
```

2. Create a virtual environment:

```bash
pyenv virtualenv 3.8.12 airbot
```

3. Activate the virtual environment:

```bash
pyenv activate airbot
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

1. Create a `.env` file in the project root directory:

```bash
touch .env
```

2. Add your OpenAI API key:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

---

## Running the Project

1. Start Jupyter Notebook:

```bash
jupyter notebook
```

2. Open the notebook:

- Navigate to `notebooks/visa_assistant.ipynb`.

3. Run all cells to initialize the chat interface.

4. Interact with the assistant:

- Type your messages in the text field.
- Click **Send** to submit.

---

## Example Usage

### Sample Conversation

```
User: Hi! I need visa help for Portugal
AI: Of course! Could you please share your passport country?

User: My passport is from Cyprus
AI: Thank you! Now, where will you be traveling to?

User: Portugal
AI: Good news! Cypriot nationals can obtain a visa on arrival in Portugal (90 days).
```

### Test Cases

Run predefined test cases in the notebook to validate functionality:

```python
test_conversation([
    "Hello! I need visa assistance",
    "My passport is from Lebanon",
    "Portugal"
])
```

---

## Customizing Visa Data

Update `src/airbot/data/visa_information.json` to add/modify visa rules:

```json
{
  "PRT": {
    "visaFree": {
      "SGP": {"maxStay": 30}
    },
    "visaOnArrival": {
      "CYP": {"maxStay": 90}
    }
  }
}

``` 
## Project Status

This project is a work in progress and will continue to be improved. Core functionality is implemented, but additional features and improvements are planned.

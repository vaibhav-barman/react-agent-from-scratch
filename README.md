
# ReAct Agent from Scratch

A hands-on project to understand and build a ReAct (Reasoning and Acting) AI agent from scratch using Python and the Groq API.

The project follows the ReAct pattern, where a language model reasons about a task, chooses actions, observes the results, and iterates toward an answer.

## Project Goals

- Understand how LLM-powered agents work.
- Implement an agent class with conversation history.
- Connect a language model using the Groq API.
- Learn the ReAct reasoning and action loop.
- Experiment with tool calling and tool execution.

## Tech Stack

- **Language:** Python
- **LLM Provider:** Groq API
- **Model:** `openai/gpt-oss-120b`
- **Libraries:** `groq`, `python-dotenv`
- **Development Environment:** Jupyter Notebook in VS Code
- **Version Control:** Git and GitHub

## Current Progress

- [x] Set up a Python virtual environment.
- [x] Configure API key management using `.env`.
- [x] Connect to the Groq API.
- [x] Create an `Agent` class.
- [x] Implement message history and LLM response generation.
- [ ] Design the ReAct system prompt.
- [ ] Implement tool execution.
- [ ] Build the complete reasoning and observation loop.
- [ ] Test the agent with practical tasks.

## Project Structure

```text
react-agent-from-scratch/
├── react_agent.ipynb
├── .env                  # Local API key (not committed)
├── .gitignore
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/react-agent-from-scratch.git
cd react-agent-from-scratch
```

### 2. Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install groq python-dotenv ipykernel jupyter
```

### 4. Configure your API key

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Get an API key from the [Groq Console](https://console.groq.com/).

**Security:** Never commit your `.env` file or expose your API key in notebook cells or outputs.

### 5. Run the notebook

Open `react_agent.ipynb` in VS Code, select the project's `.venv` Python kernel, and execute the cells.

## How ReAct Works

The ReAct pattern combines reasoning and actions in an iterative loop:

1. **Reason:** The LLM determines what to do next.
2. **Act:** The agent executes a selected tool.
3. **Observe:** The agent receives the tool's result.
4. **Repeat:** The LLM uses the observation to decide the next step or produce a final answer.

## Learning Objectives

This project is a practical exercise in LLM APIs, agent architecture, conversation state management, tool execution, and iterative reasoning.

The implementation is a work in progress. Features will be added as development continues.

## Acknowledgements

Built as a learning project while following the tutorial **"Python: Create a ReAct Agent from Scratch."**

---

*This project is for educational purposes.*
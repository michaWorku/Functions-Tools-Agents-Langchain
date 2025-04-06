# 🧠 Functions, Tools, and Agents with LangChain

## 📘 1. Course Overview

This course, offered by [DeepLearning.AI](https://www.deeplearning.ai/short-courses/functions-tools-agents-langchain/), provides a hands-on introduction to **LangChain's latest features** for building advanced LLM applications. You’ll learn to:

- Use **OpenAI function calling** for structured outputs and automation.
- Build modular chains and agents with **LangChain Expression Language (LCEL)**.
- Leverage **Pydantic** for schema validation and JSON-based interactions.
- Construct **conversational agents** with tool routing and external API integrations.

By the end, you’ll be equipped to develop powerful, production-ready LLM systems with flexibility and composability.


## 🧩 2. Course Content

### [**1. OpenAI Function Calling**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L1-OpenAI_Function_Calling.ipynb)
- Define and call functions using GPT-3.5/4.
- Modes: `auto`, `none`, and force function execution.
- Structured responses using JSON-based arguments.

### [**2. LangChain Expression Language (LCEL)**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L2-LCEL.ipynb)
- Use `Runnables` to compose prompts, models, parsers.
- Support for `async`, `batch`, `streaming`, `fallbacks`, and `parallelism`.
- Create robust LLM chains with minimal code.

### [**3. OpenAI Function Calling in LangChain**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L3-Function_Calling.ipynb)
- Use **Pydantic** to define function schemas.
- Convert schemas to OpenAI-compatible format.
- Bind functions directly to models and chains.

### [**4. Tagging and Extraction**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L4-Tagging_and_Extraction.ipynb)
- Use LangChain + OpenAI to extract structured info from text.
- **Tagging**: Extract sentiment, language, etc.
- **Extraction**: Retrieve names, paper titles, and more from documents.

### [**5. Tools and Routing**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L5-Tools_Routing_API.ipynb)
- Build tools using the `@tool` decorator.
- Integrate external APIs (OpenAPI specs).
- Route function calls based on user input context.

### [**6. Conversational Agent**](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L6-Functional_Conversation.ipynb)
- Construct tool-augmented conversational agents.
- Use `agent_scratchpad` to track intermediate steps.
- GUI demo via `Panel`.


## 📓 3. Notebooks

| Notebook Title | Description |
|----------------|-------------|
| [`01_openai_function_calling.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L1-OpenAI_Function_Calling.ipynb) | Learn the basics of OpenAI's function calling API. |
| [`02_lcel_chaining.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L2-LCEL.ipynb) | Build modular chains with LangChain Expression Language. |
| [`03_pydantic_function_calling.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L3-Function_Calling.ipynb) | Use Pydantic to structure and validate function schemas. |
| [`04_tagging_extraction.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L4-Tagging_and_Extraction.ipynb) | Perform text tagging and structured information extraction. |
| [`05_tools_routing.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L5-Tools_Routing_API.ipynb) | Define tools, integrate APIs, and route function calls. |
| [`06_conversational_agent.ipynb`](https://github.com/michaWorku/Functions-Tools-Agents-Langchain/blob/main/L6-Functional_Conversation.ipynb) | Create a tool-enhanced conversational assistant. |


## ⚙️ 4. Getting Started

### 🧰 Prerequisites

- Python 3.9+
- OpenAI API Key
- `pip install -r requirements.txt`

### 📦 Environment Setup

```bash
# Clone repo
git clone <repo-url>
cd <repo-folder>

# Set up environment
python -m venv .env
source .env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Add OpenAI Key
touch .env
echo "OPENAI_API_KEY=your_key_here" >> .env
```

### ▶️ Running Notebooks

Open Jupyter Lab or Notebook:
```bash
jupyter lab
```

Select any notebook to explore!


## 📚 5. Resources and References

- [LangChain Documentation](https://docs.langchain.com/)
- [OpenAI API Reference](https://platform.openai.com/docs)
- [Pydantic Docs](https://docs.pydantic.dev/)
- [DeepLearning.AI Course](https://www.deeplearning.ai/short-courses/functions-tools-agents-langchain/)
- [Panel for Python GUIs](https://panel.holoviz.org/)


## 🧩 6. Helpers & Utils

### ✅ Common Utilities Used

- `convert_pydantic_to_openai_function`: Converts `Pydantic` classes to OpenAI-compatible function schemas.
- `JsonOutputFunctionsParser`: Parses and extracts structured JSON from function calls.
- `RunnableLambda`: Custom transformations within a chain.
- `RecursiveCharacterTextSplitter`: Efficiently chunk long texts for processing.
- `format_tool_to_openai_function`: Converts `@tool`-decorated functions to OpenAI’s format.

These utilities simplify schema generation, output parsing, and seamless tool integration in LLM pipelines.


Feel free to modify this README as needed for your project or repository. Let me know if you'd like a markdown version!

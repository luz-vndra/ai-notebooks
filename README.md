# Getting Started


## Setup `uv`
```bash
# navigate to project root
cd llm-engineering 

# create virtual environment
uv venv
source .venv/bin/activate

# install dependencies from `pyproject.toml`
# this creates the uv.lock and downloads and installs dependenices in `pyproject.toml`
uv sync 
```

## Attach kernel to Jupyter Notebook (each time you open one)

- ensure you have the jupyter notebook plugin installed for VSCode
- in VSCode, open the sub-folder as the workspace (`code llm-engineering` for instance)
- open the Jupyter notebook you're interested in
- in the right top corner, click on select kernel, explore python enviroments to find the starred option
- now you're ready to run the cells in the Jupyter Notebook

## Installing additional dependecies

```bash
# example dependency installation

# install playwright
uv add playwright
uv run playwright install chromium
```

## Using `llama3.2` locally

- visit, [download and install Ollama for your OS here](https://ollama.com/download)
- then, in your CLI, pull llama3.2 using:
```bash
ollama pull llama3.2

# other examples
ollama pull mistral
ollama pull gemma2:2b
```
- word of caution: other versions of llama are not fit to run locally on a laptop


# Contents

- [Website Summarizer](llm-engineering/week1_day1_playwright_webscraper_implementation.ipynb) - `llm-engineering/week1_day1_playwright_webscraper_implementation.ipynb` 
    - works with both HTML websites (beautifulsoup scraper) and JS-heavy websites (playwright scraper)

- [Prompt Token Generator](llm-engineering/week1_day4.ipynb) - `llm-engineering/week1_day4.ipynb`

- [Chat Memory](llm-engineering/week1_day4.ipynb) - `llm-engineering/week1_day4.ipynb`

- [Brochure Generator & Streamer](llm-engineering/week1_day5.ipynb) - `llm-engineering/week1_day5.ipynb`

- [OpenAI Config](llm-engineering/week1_openai.ipynb) - `llm-engineering/week1_openai.ipynb`

- [Technical Chat](llm-engineering/week1_exercise.ipynb) - `llm-engineering/week1_exercise.ipynb`

- [3-way Agentic Conversation (Sequential)](llm-engineering/week1_day5.ipynb) - `llm-engineering/week1_day5.ipynb`

- [3-way Agentic Conversation (Random Order)](llm-engineering/week2_day1_single_user_prompt_alternative.ipynb) - `llm-engineering/week2_day1_single_user_prompt_alternative.ipynb`

- [Ollama open source multiple models workbook](llm-engineering/week2_open_source_multi_model.ipynb) - `llm-engineering/week2_open_source_multi_model.ipynb`

- [gradio basics](./llm-engineering/week2_day2_gradio_multi_model.ipynb) - `llm-engineering/week2_day2_gradio_multi_model.ipynb`
    - includes simple UI, one-step chat, multi-model selection single step chat, and generating company brochure with the scraper and the one-step chat


- [gradio chat bot for customer support](llm-engineering/week2_day3_gradio_chatbot.ipynb) - `llm-engineering/week2_day3_gradio_chatbot.ipynb`
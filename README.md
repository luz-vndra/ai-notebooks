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
```
- word of caution: other versions of llama are not fit to run locally on a laptop


# Contents

- Website Summarizer - `llm-engineering/week1_day1_playwright_webscraper_implementation.ipynb` 
    - works with both HTML websites (beautifulsoup scraper) and JS-heavy websites (playwright scraper)

- Token Generator - `llm-engineering/week1_day4.ipynb`

- Memory - `llm-engineering/week1_day4.ipynb`
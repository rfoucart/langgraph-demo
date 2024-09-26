# LangGraph Demo

## Prerequisites
### Install uv
```warp-runnable-command
# On macOS and Linux.
$ curl -LsSf https://astral.sh/uv/install.sh | sh

# On Windows.
$ powershell -c "irm https://astral.sh/uv/install.ps1 | iex"

# With pip.
$ pip install uv
```
See the [<u>installation documentation</u>](https://docs.astral.sh/uv/getting-started/installation/) for details and
alternative installation methods.


## Clone the repo
```warp-runnable-command
git clone git@github.com:rfoucart/langgraph-demo.git
```

## Set up the environment
Use `uv` to install the dependencies specified in `pyproject.toml`:
```warp-runnable-command
uv sync --frozen
```
Ensure you have a `.env` file with the necessary environment variables:
```dotenv
TAVILY_API_KEY=your_api_key
OPENAI_API_KEY=your_api_key
```

## Run Jupyter Lab
```warp-runnable-command
uv run jupyter lab
```

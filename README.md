# Entity Extraction with Large Language Models (LLMs)

This project provides a Jupyter notebook for exploring entity extraction with **OpenAI** using structured JSON outputs via custom `pydantic` models. Students can follow along to build foundational skills in extracting and structuring information from unstructured data sources.

## Prerequisites

- **Python 3.8+**
- **Poetry**: For package management, install it by following [Poetry's official installation guide](https://python-poetry.org/docs/#installation).

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/aissar/entity-extraction-intro.git
cd entity-extraction-intro
```

### 2. Install Dependencies with Poetry

Ensure you're in the project directory. Install the required dependencies by running:

```bash
poetry install
```

This command will create a virtual environment, install dependencies listed in `pyproject.toml`, and make the environment ready to use.

### 3. Activate the Poetry Shell

To work in the Poetry environment, activate the shell:

```bash
poetry shell
```

### 4. Set Up OpenAI API Key

To interact with the OpenAI API, you'll need an API key. Follow these steps:

1. Sign up or log into your OpenAI account.
2. Retrieve your API key from [OpenAI API keys](https://platform.openai.com/account/api-keys).
3. Create a `.env` file in the project directory to store the API key.

```bash
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

### 5. Run Jupyter Notebook

Open the code repo within the VS Code:

```bash
code .
```

Then open the Entity_Extraction_with_LLMs.ipynb file and set the virtual environment to the one created by Poetry by using the change kernel dropdown menu located on the top right hand side of VS Code.

Alternatively, launch the Jupyter notebook server within the Poetry shell:

```bash
jupyter notebook
```

Open the notebook (`Entity_Extraction_with_LLMs.ipynb`) and start exploring the examples.

## Project Structure

- **`Entity_Extraction_with_LLMs.ipynb`**: Main notebook file with guided exercises on entity extraction.
- **`pyproject.toml`**: Poetry configuration file with dependencies.
- **`.env`**: Environment variables file to store sensitive data like API keys.

## Dependencies

The following dependencies are used in this project:

- **openai**: Access GPT-4 via OpenAI's API.
- **pydantic**: Data validation and settings management using Python type annotations.
- **jupyter**: To run and interact with Jupyter notebooks.
- **python-dotenv**: Loads environment variables from a `.env` file for security.

## Troubleshooting

- **Poetry installation issues**: Ensure `Poetry` is correctly installed by running `poetry --version`. Follow the [Poetry documentation](https://python-poetry.org/docs/#installation) if you encounter issues.
- **API Key errors**: If you receive an API key error, ensure the key is correctly added to your `.env` file and that you’ve installed `python-dotenv` to load environment variables.

## Useful Links

Here are some useful resources to help you get started with Entity Extraction and using OpenAI's API:

- [OpenAI Python SDK](https://github.com/openai/openai-python): Official Python client for the OpenAI API, which simplifies the process of interacting with OpenAI's models.
- [Guides on Structured Outputs](https://platform.openai.com/docs/guides/structured-outputs): Documentation on how to work with structured outputs in the OpenAI API, including techniques for effective entity extraction.
- [Guides on Batch Processing](https://platform.openai.com/docs/guides/batch): Learn how to utilize batch processing for efficient API calls, which can be especially useful when dealing with large datasets.

Feel free to explore these resources for more information and examples!

## Exploring Advanced Topics and Future Directions

As you delve deeper into Entity Extraction with Large Language Models (LLMs), consider exploring the following advanced topics and potential future directions:

1. **Integrating with Other APIs**: Explore how to combine entity extraction capabilities with other APIs for tasks like sentiment analysis, web scraping, RAG based conversational AI assistants, etc.

2. **Deployment to Cloud**: Learn how to deploy your entity extraction pipeline to various cloud providers (e.g, AWS, GCP), to handle large volumes of unstructured data efficiently.

3. **Real-Time Processing**: Build real-time entity extraction pipelines from streaming data sources, enabling immediate insights from incoming information.

4. **Cross-Model Comparisons**: Experiment with different LLMs (e.g., OpenAI's larger / more capable models, Google’s Gemini, Anthropic's Claude) to compare their performance on entity extraction tasks across various datasets.

5. **Model Output Evaluation**: Techniques to measure the accuracy and quality of model outputs to ensure entity extraction jobs can be used reliably within production workloads.

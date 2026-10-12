AI Code Doctor is a Python debugging assistant that analyzes Python files, detects syntax errors and code quality issues, and uses OpenAI to explain detected problems in simple language.

## Features

- **Syntax Checking:** Detects Python syntax errors using Parso and Python's built-in compiler.
- **Code Analysis:** Uses Ruff to identify code quality issues and potential mistakes.
- **AI-Powered Explanations:** Explains detected issues and suggests possible fixes using OpenAI.
- **Error Locations:** Displays line and column numbers when available.
- **Duplicate Detection:** Removes duplicate diagnostic reports.
- **Safe Analysis:** Analyzes the target file without executing it.

## Requirements

- Python 3.10 or compatible version
- OpenAI API key for AI explanations
- Required Python packages: `openai`, `parso`, `python-dotenv`, and `ruff`

## Installation

Install the required packages:

```bash
pip install openai parso python-dotenv ruff
```

Create a `.env` file in your project directory:

```env
OPENAI_API_KEY=your_openai_api_key
OPENAI_MODEL=gpt-4.1-mini
```

## Usage

Run the program:

```bash
python main.py
```

Enter the full path of the Python file you want to analyze when prompted.

## Limitations

AI explanations require a valid OpenAI API key. The tool performs static analysis and does not execute, automatically repair, or test the target Python file.

## License

Choose a license before distributing this project publicly.

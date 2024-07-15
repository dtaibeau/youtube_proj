# YouTube Speaker Identification and Transcript Correction

This project uses OpenAI's ChatGPT-4o to identify speakers and correct transcription errors in YouTube video transcripts from a YouTube url. 

## Features

- Fetch YouTube video details and transcripts.
- Identify different speakers in the transcript.
- Correct transcription errors.
- Display the corrected transcript in a readable HTML format.

## Requirements

- [Streamlit](https://streamlit.io) for the user interface.
- [Pytube](https://pytube.io) for fetching video details.
- [YouTube Transcript API](https://github.com/jdepoix/youtube-transcript-api) for obtaining video transcripts.
- [LangChain](https://github.com/hwchase17/langchain) and [OpenAI's GPT-4](https://openai.com/research/gpt-4) for speaker identification and text correction.
- [Pydantic](https://pydantic-docs.helpmanual.io) for data validation.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/youtube-project.git
cd youtube-project
```

2. Install Poetry if you haven't already:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

3. Install the dependencies:

```bash
poetry install
```

## Usage

1. Activate the virtual environment:
```bash
poetry shell
```

2. Run the Streamlit app:
```bash
streamlit run youtube_project/main.py
```

## Project Structure

```plaintext
├── README.md            # Project README file
├── pyproject.toml       # Poetry configuration file
├── poetry.lock          # Poetry lock file 
├── transcript.json      # Example JSON transcript
├── src/                 # Source files/packages
│   ├── main.py          # Main script for Streamlit app
├── tests/               # Test files
│   ├── test_transcripts.py # Example test file
├──
```

## How to Contribute

1. Fork the repository
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a pull request

Happy transcripting! :D
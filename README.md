# YouTube Speaker Identification and Transcript Correction

This project uses OpenAI's ChatGPT-4o to identify speakers and correct transcription errors in YouTube video transcripts from a YouTube url. 

## Features

- Fetch YouTube video details and transcripts
- Identify different speakers in the transcript
- Correct transcription errors
- Display the corrected transcript in a readable HTML format

## Requirements

- [Streamlit](https://streamlit.io) for the user interface
- [Pytube](https://pytube.io) for fetching video details
- [YouTube Transcript API](https://github.com/jdepoix/youtube-transcript-api) for obtaining video transcripts
- [LangChain](https://github.com/hwchase17/langchain) and [OpenAI's GPT-4o](https://openai.com/research/gpt-4) for speaker identification and text correction
- [Pydantic](https://pydantic-docs.helpmanual.io) for data validation

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/dtaibeau/youtube-project.git
    cd youtube-project
    ```

2. **Install Poetry if you haven't already:**
    ```bash
    curl -sSL https://install.python-poetry.org | python3 -
    ```

3. **Install the dependencies:**
    ```bash
    poetry install
    ```

## Usage

1. **Activate the virtual environment:**
    ```bash
    poetry shell
    ```

2. **Run the Streamlit app:**
    ```bash
    streamlit run youtube_project/main.py
    ```

3. **Access the app:**
   - Open your web browser and go to `http://localhost:8501`

5. **Using the app:**
   - Input a YouTube URL into the provided field
   - Click the "Process Video" button
   - View HTML of transcript on the app interface

## Project Structure

```plaintext
├── README.md            # Project README file
├── pyproject.toml       # Poetry configuration file
├── poetry.lock          # Poetry lock file
├── transcript.json      # Example JSON transcript
├── .gitignore           # Git ignore file
├── youtube_project/     # Source files/packages
│   ├── main.py          # Main script for Streamlit app
├── tests/               # Test files
│   ├── test_transcripts.py # Example test file
```

## Deployment
The app is deployed and can be accessed at https://youtubeproj-dtaibeau.streamlit.app/. Just input a YouTube URL and click "Process Video" to the transcription process in action!

## How to Contribute
1. **Fork the repository:**

```bash
git clone https://github.com/dtaibeau/youtube_project.git
cd youtube_project
```

2. **Create your feature branch:**

```bash
git checkout -b feature/awesome_feature
```

3. **Commit your changes:**

```bash
git commit -m 'add some awesome feature'
```

4. **Push to the branch:**

```bash
git push origin feature/awesomeFeature
```

5. **Open a pull request:**

- Go to forked repository on GitHub
- Click on "New Pull Request" button

  
## Future Updates
- Adding feedback to indicate the app's progress to users during transcription process
- Pytube description bug fix
- Additional features and improvements based on user feedback :-)

Happy transcripting!

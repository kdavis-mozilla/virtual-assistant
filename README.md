# Project aestethics

![aesthetics](https://psychonautgirl.space/images/project_aesthetics.png)

# How to use:

## Unix users:

### Setup

1. Create a virtual environment using your favorite tool
2. Using a Python >= 3.5 `pip install PySide2 rasa deepspeech torch` or use the requirements file
3. Download the model from DeepSpeech's repo and unzip it `wget https://github.com/mozilla/DeepSpeech/releases/download/v0.6.1/deepspeech-0.6.1-models.tar.gz tar xvfz deepspeech-0.6.1-models.tar.gz`
4. Start a TTS server locally on port 5002 as described [here](https://github.com/mozilla/TTS/wiki/Released-Models#simple-packaging---self-contained-package-that-runs-an-http-api-for-a-pre-trained-tts-model).
5. `cd qt-rasa && rasa train`\*

### Running your assistant

6. On `qt-rasa` directory run `rasa run --enable-api -p 5003 -vv` to start the NLP server
7. On the main directory run `python main.py` to open the GUI

\* Every time you change something in the .md files you'll have to retrain this

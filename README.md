### Initial Setup:
Creating the venv:
- Open a new cmd terminal in VS code (if not default, click dropdown arrow next to '+' on the terminal top right then choose command prompt)
- In the terminal, ```pip install virtual env```
- Create an environment: ```virtual env venv```
- Launch environment: ```venv\Scripts\activate.bat.``` You should see (venv) at the beginning of the command line if you've successfully entered the environment.

Setup/install necessary libraries:
- Once the virtual environment is launched, run:
    - ```pip install openai speechrecognition gtts playsound torch torchvision matplotlib PyAudio Pillow dotenv```
- Make sure your python interpreter is correct by doing ```CTRL + SHIFT + P```, then "Python: Select Interpreter", and choosing "Python 3.11.4" or similar

### Every time:
Launching the display is hella easy:
- Just run the ```app.py``` file in ```src```
- The display is made using tkinter library



### MVP: Create a Working Voice Assistant

The goal was to develop a minimal voice assistant capable of interpreting speech, getting a response from ChatGPT, and converting the response back into speech, all with a simple display.

---

## Features Proposed and Achieved

### Speech-to-Text (STT)
- **Functionality**: 
  - Recognize speech from the microphone using Google STT.
  - Convert microphone inputs into text.


### Interface With OpenAI
- **Functionality**: 
  - Send and receive text over the internet to interact with ChatGPT.


### Text-to-Speech (TTS)
- **Functionality**: 
  - Convert AI responses from text to speech using the eSpeak library.
  - Output speech through the microphone.


### Status Display
- **Functionality**: 
  - Create a simple graphical display using the `tkinter` library to show the current state of operation.

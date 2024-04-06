# Quick Voice bot demo

# This is a Demo showing a bot that uses Text-To-Speech, Speech-To-Text, and a language model using GROQ, Deepgram, Langchain, to have voice a conversation with a user in real time.

This demo is set up to use [Deepgram](www.deepgram.com) for the audio service and [Groq](https://groq.com/) the LLM.
(Deepgram offers $200 free credit without using any credit card/payment details. So, you can check it out.)

This demo utilizes streaming for sst and tts to speed things up.

The files in `building_blocks` are the isolated components if you'd like to inspect them for each task like speech to text , text to speech with deepgram.

You can also modify the system prompt, to enhace the chatbot's response to a more controlled domain specific use case.
# You can run the proect after installing required packages. Make sure to provide Deepgram API key and Groq API key to run the project.

```
git clone https://github.com/gkamradt/QuickAgent.git
cd QuickAgent
pip install -r requirements.txt
python3 QuickAgent.py
```

# NOTE on running the project smoothly without running into issues

If you are on windows:
1. Download ubuntu in VS code and run the project in it.
2. Naivate to directory
``` 
cd QuickAgent
```
3. Now activate the virtual env. This will ensure that all packages installed will not cause any build issues. 
```
. ./test_env/bin/activate
```
5. After this run 
```
    pip install -r requirements.txt
```    
4. Download the following packages if you face additional issues relating to audio input device not found :
```
    pip install PyAudio
    apt-get install pavucontrol
    apt-get install ffmpeg
```    

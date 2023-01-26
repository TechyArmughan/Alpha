# Alpha
What can this A.I. assistant do for you?
It can send emails on your behalf.
It can play music for you.
It can do Wikipedia searches for you.
It is capable of opening websites like Google, Youtube, etc., in a web browser.
It is capable of opening your code editor or IDE with a single voice command.
Enough talks! Let's start building our own A.L.P.H.A

10:08 – Starting Pycharm
I am going to use the Pycharm IDE in this video. Feel free to use any other IDE you are comfortable with. Start a new project and make a file called jarvis.py.

10:54 – Defining Speak Function
The first and foremost thing for an A.I. assistant is that it should be able to speak. To make our A.L.P.H.A talk, we will make a function called speak(). This function will take audio as an argument, and then it will pronounce it.

def speak(audio):
       pass      #For now, we will write the conditions later.
Now, the next thing we need is audio. We must supply audio so that we can pronounce it using the speak() function we made. We are going to install a module called pyttsx3.

What is pyttsx3?
A python library that will help us to convert text to speech. In short, it is a text-to-speech library.
It works offline, and it is compatible with Python 2 as well as Python 3.
Installation:

pip install pyttsx3
In case you receive such errors: 

No module named win32com.client
No module named win32
No module named win32api
Then, install pypiwin32 by typing the below command in the terminal :

pip install pypiwin32.
After successfully installing pyttsx3, import this module into your program.

Usage:

import pyttsx3

engine = pyttsx3.init('sapi5')

voices= engine.getProperty('voices') #getting details of current voice

engine.setProperty('voice', voice[0].id)
What is sapi5?
Microsoft developed speech API.
Helps in synthesis and recognition of voice.
What Is VoiceId?
Voice id helps us to select different voices.
voice[0].id = Male voice 
voice[1].id = Female voice

---
layout: project-screenshots
title:  "KTaNE Assistant"
teaser: "A KTaNE assistant for when you're alone."
tags:
    - post format
categories:
    - projects
image:
    thumb: projects/ktane-assistant-thumb.png
    title: projects/ktane-assistant-thumb.png
show_meta: false
gallery:
    - image_url: projects/ktane-assistant/screenshots/screenshot1.png
github: https://github.com/Multipixels/Keep-Talking-and-Nobody-Explodes-Bot
header: no
---

A high-school project made to help users play [Keep Talking and Nobody Explodes](https://keeptalkinggame.com/) without the need of another player. Simply start up the program and describe the bomb as it tells you which wires to cut or what code to insert.

### Built With

* [Python](https://www.python.org/)
* [Vosk](https://alphacephei.com/vosk/)

### Prerequisites

* pip
  ```sh
  pip install --upgrade pip
  ```

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/Multipixels/Keep-Talking-and-Nobody-Explodes-Bot.git
   ```
2. Install Python package dependencies
   ```sh
   pip install pynput
   pip install pyttsx3
   pip install pyaudio
   pip install vosk
   ```
3. Install a [Vosk Audio Recognition Model](https://alphacephei.com/vosk/models). Put it in the root folder of the repo.
   - The only two models supported are the following.
     - [vosk-model-en-us-0.22-lgraph](https://alphacephei.com/vosk/models#:~:text=vosk%2Dmodel%2Den%2Dus%2D0.22%2Dlgraph), Faster bootup, but provides less accuracy. If having trouble, try using the next model.
     - [vosk-model-en-us-0.22](https://alphacephei.com/vosk/models#:~:text=Apache%202.0-,vosk%2Dmodel%2Den%2Dus%2D0.22,-1.8G), Provides more accuracy, but initial bootup takes longer and takes up much more space.

### Usage

Run the main.py file. If installation was done correctly, a window will popup. Wait until it shows "Bot heard: Ready to Listen!"
When you're ready to start, press the "Activate" button below. Press it again if you want to stop.

_Full tutorials will be found [here](https://www.youtube.com/playlist?list=PLll7a_aZOiE63zbNZDA6jSA71DDJmMIG4)._

_For more in-depth details on specific modules and information, please refer to the [Wiki](https://github.com/Multipixels/Keep-Talking-and-Nobody-Explodes-Bot/wiki)._
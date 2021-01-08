
## Projects

*This is a collection of some of my recent projects*

### Pokemon Johto Pokedex Voice Assistant 

This is a simple voice assistant that returns information on Pokemon from the Johto region based on user voice queries. 
The Pokemon objects are all stored in a SQLite database, and the text to speech is handled using gTTS.

Made with Python, SQLite, Google Text To Speech

### Video Game Screen Reader and Ambient LED Controller

Using PyTesseract, this code is capable of reading data from my main monitor in order to detect important stats across four games by isolating a fraction of the screen. 
It is capable of reading numerical, text, and color data depending on the game. 
In order to determine the chosen game, there is both a GUI set up using Tkinter, and automatic detection by checking subprocesses. 
The captured data is transferred to Arduino across a serial port in order to change the color of an individually addressible LED strip.
In addition to the LED strip, the code also is capable of changing the color of Kasa bulbs, adjusting the speed of Dyson fans, sending text messages using Twilio, and sending toast notifications.

Made primarily with Python, PyTesseract, Arduino, FastLED

### Secret Santa Randomizer 

I was tasked with randomizing the Secret Santa assignments for my family gift exchange, and decided to automate the task. 
Using some permutation theory and a randomized list, I was able to distribute names randomly. I also designed a loop to block pairs that were not allowed, i.e. spouses. 
The data of the pairs was then saved to a text file, and used again with a dictionary of phone numbers to send text messages from Twilio.

Made with Python, Twilio

### Alexa Skill Code Template

Kin-Keepers | Junior Software Engineer | Summer 2020

In Spring 2020 I started working for a company called Kin-Keepers. Kin-Keepers focuses on creating a voice of representation for seniors by creating services and technology. 
My specific job was to design Alexa skills and explore Voice User Interface a viable solution for seniors without computer access. 
In addition to the skills I made, I took the opportunity to create a template for future skill development. 
My Alexa Skill Code Template is not only a step-by-step guide to creating Alexa skills, but also a fill-in-the-blank system for custom skill responses. 
Kin-Keepers mostly wanted simple call and response style skills, and this template made that process much easier. 

Made using Python and Alexa Skills Kit

### Coronavirus Tracker Map 

This project was originally my final project for a Data Visualization in Python course, but I continued the project after the class ended. 
This code projects coordinates from latitude and longitude values of counties onto four images of the United States, representing confirmed cases, active cases, and deaths. 
These points scaled in opacity based on the number of cases or deaths with respect to the total county population, which I had stored separately.
Data for the coronavirus statistics was pulled from the reports that the John Hopkins Center for Systems Science and Engineering put on Github.

Made with Python, Matplotlib, and Basemap

### Magic the Gathering Random Card Generator

Now that there are more than 20,000 unique Magic the Gathering cards, I knew it would take time to find the best cards for my deck. 
My current deck uses cards that are only blue, black, or green, and specializes in creatures that have an effect when they enter the battlefield.
Using Scrython's card database and Regex, I was able to create a random card generator that specifically returns blue, black, green, and colorless cards with an "enters the battlefield" effect. 

Made with Python, Scrython (Scryfall API), Regex

### City to Zip Web Application

This project was mostly a sandbox to test Brython (Browser Python), which let's users program websites using Python instead of Javascript. 
The user interface of this application is a table with a textbox, whose value gets replaced. While the html itself is simple, the concept of Browser Python is awesome.

Made with Python, HTML, CSS, Brython

### 'Feelix' | Emotion Journal for HackDavis 2020 

For HackDavis 2020 my team and I developed a text-based emotion journal named Feelix. 
Feelix responded randomly based on the time of day, and detected emotion. 
The main idea with out limited knowledge was to validate emotions, and provide relevant inspiring quotes. 
There was also an effort to ask for confirmation and detect negation (i.e. 'I am not sad')

Made with Python

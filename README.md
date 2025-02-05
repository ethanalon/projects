
## Projects

*This is a collection of some of my recent projects*

### Lorcana Card Scanner and Classifier

Lorcana is a new Trading Card Game by Disney and Ravensburger. Leveraging the power of OpenCV, this project enables webcam scanning for card identification.

Presently, the project focuses on identifying cards and overlaying their names onto the webcam feed. However, it's poised for future enhancements. The inspiration stemmed from observing card scanners utilized in Magic the Gathering tournaments and livestreams.

Users can conveniently scan their physical cards, generating larger and clearer images in a separate frame. Moreover, potential expansions include integrating TCGPlayer functionality to offer pricing information or aid in collection tracking.

Made with Python, OpenCV

### Magic the Gathering Collection Database

Now that there are more than 20,000 unique Magic the Gathering cards, I knew it would take time to find the best cards for my deck. 
My current deck only uses cards that are only blue, black, or green, and it specializes in creatures that have an effect when they enter the battlefield. For some terrible reason, my love for these specific cards led me to the arduous task of collecting them all.

Using Scrython's card database and Regex, I was able to create a custom query that specifically returns blue, black, green, and colorless cards with a triggered "enters the battlefield" effect. Then, I used the output of the HTTP request for the Scryfall API of this query and ran it through a custom function I created in Python. This function added a column to check if the card is in my collection or not, and removed some other unnecessary columns. When the data was finally clean and aggregated, it was passed into BigQuery to create my very own collection database. Now I can run SQL queries to check if I am missing a specific card, or to see the entire list of cards in my collection.

Made with Python, Scrython (Scryfall API), Regex, BigQuery, SQL

### Magic the Gathering Random Card Alexa Skill

Note: I wrote this skill *before* I created my fancy BigQuery database, so it does not implement the Collection database at all. Maybe in the future it will.

Also using Scrython's card database and Regex, I created a random card generator that specifically returns blue, black, green, and colorless permenant cards with a triggered "enters the battlefield" effect. Then, I turned this powerful query into an Alexa Skill to make it more accessible. It isn't publically published since it has a very very specific use case, but I still use it for curiosity and fun.

Made with Python, Scrython (Scryfall API), Regex, Alexa Skills Kit

### Thumbs Up Clicker

Overcrowded Tycoon is a mobile game by Zeptolab, where you simulate the creation of an amusement park. In that game, guests can show their satisfaction with a thumbs up emoji inside a little speech bubble. This program uses PyAutoGUI to detect those thumbs up emojis on my screen, and click them. In order to project my phone screen to my computer, I used Windows Phone Link.

Made with Python, Windows Phone Link,  PyAutoGUI, and win32api

### Pokemon Johto Pokedex Voice Assistant 

This is a simple voice assistant that returns information on Pokemon from the Johto region based on user voice queries. 
The Pokemon objects are all stored in a SQLite database, and the text to speech is handled using gTTS.

Made with Python, SQLite, Google Text To Speech

### Video Game Screen Reader and Ambient LED Controller

Using PyTesseract, this code is capable of reading data from my main monitor in order to detect important stats across four games by isolating a fraction of the screen. 
It is capable of reading numerical, text, and color data depending on the game. 
In order to determine the chosen game, there is both a GUI set up using Tkinter, and automatic detection by checking subprocesses. 
The captured data is transferred to Arduino across a serial port in order to change the color of an individually addressable LED strip.
In addition to the LED strip, the code also is capable of changing the color of Kasa bulbs, adjusting the speed of Dyson fans, sending text messages using Twilio, and sending toast notifications.

Made with Python, PyTesseract, Arduino, FastLED

### Secret Santa Randomizer 

I was tasked with randomizing the Secret Santa assignments for my family gift exchange, and decided to automate the task. 
Using some permutation theory and a randomized list, I was able to distribute names randomly. I also designed a loop to block pairs that were not allowed, i.e. spouses. 
The data of the pairs was then saved to a text file, and used again with a dictionary of phone numbers to send text messages from Twilio.

Made with Python, Twilio

### Graph Database Alexa Skill Query

Kin-Keepers | Software Engineer | Summer 2021

In Spring 2020 I started working for a company called Kin-Keepers. Kin-Keepers focuses on creating a voice of representation for seniors by creating services and technology. 
My specific job was to design Alexa skills and explore Voice User Interface a viable solution for seniors without computer access. 
Without releasing confidential information, I can disclose that I was in charge of connecting a graph database system to an Alexa Skill. So this skill was able to query our remote database and get information stored in it. 

Made using Python and Alexa Skills Kit

### Coronavirus Tracker Map 

This project was originally my final project for a Data Visualization in Python course, but I continued the project after the class ended. 
This code projects coordinates from latitude and longitude values of counties onto four images of the United States, representing confirmed cases, active cases, and deaths. 
These points scaled in opacity based on the number of cases or deaths with respect to the total county population, which I had stored separately.
Data for the coronavirus statistics was pulled from the reports that the John Hopkins Center for Systems Science and Engineering put on Github.

Made with Python, Matplotlib, and Basemap

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

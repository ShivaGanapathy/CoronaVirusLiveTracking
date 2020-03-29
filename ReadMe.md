## COVID-19 Live Tracking Website

CoronaVirus Tracker was a collab between Sam Williams (ayunami2000 on GitHub), Ali Ahmad (aahmad4 on Github) & Myself. 


The website(designed with HTML,CSS,NodeJS & a Python Backend) tracks international data on the COVID-19 pandemic and displays it in easy to read graphics. I was responsible for the the data collection, preproccessing, and visualization processes using Python & Matplotlib. To see the website, click this link:
https://coronatracker.glitch.me/

## Repository Contents
- server.js: This contains our first back-end programming file which was written in Node.js. This file contains the web server and assets to run the python aspect and return the images of data to the end-user.
- server.py: This is our second back-end programming language. This file contains the logic for the server to communicate with the JavaScript and HTML. Also, this is where we have the logic written for using the Coronavirus Monitor Rapid API to make our own graphs with matplotlib and distrubute them to the end-user.
- index.html and style.css in the public folder both contain the front-end of the website and that's where the user interface and overall design of the website was developed.


![](demo1.PNG)

![](demo2.PNG)

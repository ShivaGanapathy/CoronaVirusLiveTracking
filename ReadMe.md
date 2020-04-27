## COVID-19 Live Tracking Website

CoronaVirus Tracker was a collaboration between Sam Williams (ayunami2000 on GitHub), Ali Ahmad (aahmad4 on Github) & Myself. 


The website(designed with HTML,CSS,NodeJS & a Python Backend) tracks international data on the COVID-19 pandemic and displays it in easy to read graphics. I was responsible for the the data collection, preproccessing, and visualization processes using Python & Matplotlib. To see the website, click this link:
https://coronatracker.glitch.me/

## Repository Contents
- [server.js](https://github.com/ShivaGanapathy/CoronaVirusLiveTracking/blob/master/server.js): This contains our first back-end programming file which was written in Node.js. This file contains the web server and assets to run the python aspect and return the images of data to the end-user.
- [server.py](https://github.com/ShivaGanapathy/CoronaVirusLiveTracking/blob/master/server.py): This is our second back-end programming language. This file contains the logic for the server to communicate with the JavaScript and HTML. Also, this is where we have the logic written for using the Coronavirus Monitor Rapid API to make our own graphs with matplotlib and distrubute them to the end-user.
- [index.html](https://github.com/ShivaGanapathy/CoronaVirusLiveTracking/blob/master/index.html) and [style.css](https://github.com/ShivaGanapathy/CoronaVirusLiveTracking/blob/master/style.css) in the public folder both contain the front-end of the website and that's where the user interface and overall design of the website was developed.


![](demo1.PNG)

![](demo2.PNG)

## Clone
```bash
git clone https://github.com/aahmad4/Live-Coronavirus-Tracker
```

## Implementation

In [server.py](https://github.com/ShivaGanapathy/CoronaVirusLiveTracking/blob/master/server.py), change `"apikey"` to match your personal key on Rapid API.
```python
def apiReq(countries):
  apiArr=[]
  for item in countries:
      querystring = {"country":fixCountryNames(item)}

      headers = {
          'x-rapidapi-host': "coronavirus-monitor.p.rapidapi.com",
          'x-rapidapi-key': os.environ["apikey"] # security measure, see ".env" in files to find the key
          }
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

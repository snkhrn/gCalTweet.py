**Warning!!**
Please be aware that this project is nicely working but incomplete for distribution.

gCalTweet.py
======================
Helps creating a bot to automatically tweet events from Google Calendar V3.


## Dependencies

```
tweepy==2.1
APScheduler==3.0.0
google-api-python-client
PyCrypto==2.6
```

## Installation

Install dependencies.

You need to create OAuthSettings.py file: 
````
settings = {
    'consumer_key': 'xxxx',
    'consumer_secret': 'xxxx',
    'access_token_key': 'xxxx',
    'access_token_secret': 'xxxx'
}
````

And get an OAuth Json Key file from https://console.developers.google.com/ and rename the downloaded file to "secret_json.json": 

In bot.py file, insert google your calendar IDs into calIds.

````
    calIds = [
        "xxx@group.calendar.google.com",
        "xxx@group.calendar.google.com"
    ]

````


Test in the terminal first; use cloud application platforms like Heroku (free) for deployment.
Modify ( gCalTweetBot(), GCalendar.formTweet(), etc... )  and schedulers as you want.
Happy coding! :)

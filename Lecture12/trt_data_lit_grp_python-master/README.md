# trt_data_lit_grp_python
The Repository for Learn Python Hard Way: Mining Social Media Series

Installing Python
---------

If you don't have python on your computer already, please install Anaconda Python 2.7
Follow the instruction here and select the most appropriate option based on your OS
https://www.continuum.io/downloads

Twitter API Access
---------
In order to get access to the Twitter API through OAuth (open standard for authorization), 
we have to obtain our consumer information and access tokens first by registering 
our app on https://apps.twitter.com.

1. Go to https://apps.twitter.com/ and log into your twitter account

2. Click on "Create New App"

3. Obtain the Consumer key, Consumer secret

4. Go to "Manage Your Access Token", "Generate Access Token", Obtain Access token, and Access token secret. Save them somewhere.
DO NOT SHARE THIS INFORMATION WITH ANYBODY ELSE!

Test Twitter Access
---------
We will use Twython to access Twitter data, you can install it by 

```
pip install twython
```

Note: if you have installed Anaconda for Windows, go to Anaconda Command Prompt, cd into C:\Program Files\Anaconda2\Scripts


Create a Twython instance with your Consumer Key and Consumer Secret

```
from twython import Twython

APP_KEY = "your_consumer_key"
APP_SECRET = "your_consumer_secret"
OAUTH_TOKEN= "your_access_key"
OAUTH_TOKEN_SECRET= "your_access_token"

twitter = Twython(APP_KEY, APP_SECRET,OAUTH_TOKEN, OAUTH_TOKEN_SECRET)
```

Let's try to post a status on your twitter account through Python

```
twitter.update_status(status='I am going to TDLG to Learn Python the Hard Way!')
```

Check your Twitter Profile. Hooray! You have completed the Prerequisites! See you at the session!

Credits
---------
* [Mining Social Media Web 2nd Edition](https://github.com/ptwobrussell/Mining-the-Social-Web-2nd-Edition)

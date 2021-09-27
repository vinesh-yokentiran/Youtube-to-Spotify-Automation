# Youtube to Spotify playlist automation
A python automation script that generates a spotify playlist, searches, and then adds all your youtube liked videos playlist songs to your newly generated spotify playlist. This project serves the purpose of automating a process that was previously tedious for me to do and also acts as a project to become more familiar with using API's. 

## Table of Contents
* [Technologies](#Technologies)
* [Setup](#LocalSetup)



## Technologies
* [Youtube Data API v3]
* [Spotify Web API]
* [Requests Library v 2.22.0]
* [Youtube_dl v 2020.01.24]

## LocalSetup
1) Install All Dependencies   
`pip3 install -r requirements.txt`

2) Collect Your Spotify User ID and Oauth Token From Spotfiy and add it to secrets.py file
    * To Collect your User ID, Log into Spotify then go here: [Account Overview] and its your **Username**
    * To Collect your Oauth Token, Visit this url here: [Get Oauth] and click the **Get Token** button

3) Enable Oauth For Youtube and download the client_secrets.json   
    * Just follow the guide here [Set Up Youtube Oauth] ! 
    If you are having issues check this out [Oauth Setup 2] and this one too [Oauth Setup 3] 

4) Run the File  
`python3 create_playlist.py`   
    * you'll immediately see `Please visit this URL to authorize this application: <some long url>`
    * click on it and log into your Google Account to collect the `authorization code`



   [Youtube Data API v3]: <https://developers.google.com/youtube/v3>
   [Spotify Web API]: <https://developer.spotify.com/documentation/web-api/>
   [Requests Library v 2.22.0]: <https://requests.readthedocs.io/en/master/>
   [Account Overview]: <https://www.spotify.com/us/account/overview/>
   [Get Oauth]: <https://developer.spotify.com/console/post-playlists/>
   [Set Up Youtube Oauth]: <https://developers.google.com/youtube/v3/getting-started/>
   [Oauth Setup 2]:<https://stackoverflow.com/questions/11485271/google-oauth-2-authorization-error-redirect-uri-mismatch/>
   [Youtube Video]:<https://www.youtube.com/watch?v=7J_qcttfnJA/>
   [Youtube_dl v 2020.01.24]:<https://github.com/ytdl-org/youtube-dl/>
   [Oauth Setup 3]:<https://github.com/googleapis/google-api-python-client/blob/master/docs/client-secrets.md/>

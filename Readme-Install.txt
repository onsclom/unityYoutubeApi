Installation:
Local:
	For local instalation use pip:
		pip install -r requirements.txt
	Then just run python -m youtube_dl_server

Heroku:
Create one application and deploy the source code to heroku (it will get all the dependencies automaticaly)
Updating the youtubedl version in heroku, if some videos stop to work you need to update the youtube dl, to update in heroku you need to clear the app cache.

To do this you need to run these commands:
heroku plugins:install heroku-repo
heroku repo:purge_cache -a appname
git commit --allow-empty -m "Purge cache"
git push heroku master

this will make the heroku reinstall the youtubedl with the lastest version.



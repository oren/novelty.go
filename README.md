Setup
===

# Get your [dev environment](https://developers.google.com/appengine/docs/go/gettingstarted/devenvironment) setup for GAE. It comes with a version of Go, so don't worry about compiling/installing that.
# Clone this repository, cd into the directory.
# $ cp app.yaml.example app.yaml
# Edit app.yaml with the app name you plan to use.

Running locally
===

# Start the dev server: $ dev_appserver.py .
# Seed the server with starting data: $ curl whatever:bees@localhost:8080/yes
# Visit localhost:8080 in your browser.

Your novelty server is ready to go. The answer is current set to "yes", and the
password for changing the answer is "bees".

To change the answer to "no", simply visit larry:bees@localhost:8080/no

Running on appspot
===

# Follow the [registration instuctions](https://developers.google.com/appengine/docs/go/gettingstarted/uploading) for GAE.
# Make sure that the app id in app.yaml matches you new app id.
# Push the app: $ appcfg.py .
# Seed the server with starting data. I'd suggest a different password than
"bees": $ curl http://moe:$PASSWORD@$APPID.appspot.com/yes
# Visit $APPID.appspot.com in your browser to behold your new novelty server.

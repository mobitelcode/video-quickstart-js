**NEW:** Please check out the newly open-sourced [multi-party video application](https://github.com/twilio/twilio-video-app-react)
built with twilio-video.js and [React.js](https://reactjs.org/).

# Twilio Video Quickstart for JavaScript

[![OS X/Linus Build Status](https://secure.travis-ci.org/twilio/video-quickstart-js.png?branch=master)](http://travis-ci.org/twilio/video-quickstart-js) [![Windows Build status](https://ci.appveyor.com/api/projects/status/3u69uy9c0lsap3dr?svg=true)](https://ci.appveyor.com/project/markandrus/video-quickstart-js)

_For Twilio Video 1.x Quickstart, go [here](https://github.com/twilio/video-quickstart-js/tree/1.x)._

This application should give you a ready-made starting point for writing your
own video apps with Twilio Video. Before we begin, we need to collect
all the config values we need to run the application:

- Account SID: Your primary Twilio account identifier - find this [in the console here](https://www.twilio.com/console).
- API Key SID: Used to authenticate - [generate one here](https://www.twilio.com/console/runtime/api-keys).
- API Key Secret: Used to authenticate - [just like the above, you'll get one here](https://www.twilio.com/console/runtime/api-keys).

## A Note on API Keys

When you generate an API key pair at the URLs above, your API Key Secret will only
be shown once - make sure to save this in a secure location,
or possibly your `~/.bash_profile`.

## Setting Up The Application

Create a configuration file for your application:

```bash
cp .env.template .env
```

Edit `.env` with the configuration parameters we gathered from above.

Next, we need to install our dependencies from npm:

```bash
npm install
```

Now we should be all set! Run the application:

```bash
npm start
```

Your application should now be running at [http://localhost:3000](http://localhost:3000). Just enter
the name of the room you want to join and click on 'Join Room'. Then,
open another tab and join the same room. Now, you should see your own
video in both the tabs!

![screenshot of chat app](quickstart/public/quickstart.png)

## Examples

The project contains some use-case examples for the Twilio Video JS SDK. After running the application
by following the instructions above, go to [http://localhost:3000/examples](http://localhost:3000/examples)
to try them out.

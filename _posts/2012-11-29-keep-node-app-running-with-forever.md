---
layout: post
category : nodejs
tags : [deployment]
---
{% include JB/setup %}

node app can be run with the following command:

    node app.js

however, when the session is quit, the app stops the run. To keep the app running, we can use forever, first, install forever gloablly:

	npm install -g forever

then we can use forever to run our app:

	forever start app.js

we can also check the current running app:

	forever list


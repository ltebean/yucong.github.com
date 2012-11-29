---
layout: post
category : nodejs
tags : [debug]
---
{% include JB/setup %}

node-inspector can make it easy for us to debug node app, first, install it:

    npm install -g node-inspector

start the node app in debug mode:

	node --debug app.js

start the inspector:

	node-inspector &

open http://127.0.0.1:8080/debug?port=5858 in  WebKit based browser, done~


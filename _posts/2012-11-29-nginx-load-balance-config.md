---
layout: post
category : nginx
tags : [beginner, tutorial]
---
{% include JB/setup %}

nginx can handle the load balance for us

first define the backend servers:

    upstream backend_server {
    	server 127.0.0.1:8080 weight=1 max_fails=2 fail_timeout=10s;
    	server 127.0.0.1:9000 weight=1 max_fails=2 fail_timeout=10s;
	}

then in the location block:

    location / {
    	proxy_pass http://backend_server;
	}



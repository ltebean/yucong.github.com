---
layout: post
category : nginx
tags : [auth]
---
{% include JB/setup %}

How to

first define the block:

    location  /  {
 		auth_basic           "Restricted";
	  	auth_basic_user_file  authfile; // relative to conf 
	}
the filename path is relative to directory of nginx configuration file nginx.conf

The authfile is created by htpasswd:

    htpasswd -c -m authfile <user>
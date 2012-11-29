---
layout: post
category : nginx
tags : [beginner, tutorial]
---
{% include JB/setup %}

## prerequisite

nginx needs the following libraries, they must first be installed on the system

- openssl http://www.openssl.org/
- pcre http://www.pcre.org/
- zlib http://www.zlib.net/

download and install these libraries:  

    tar -zxvf package.tar.gz
    make && make install

## install nginx

download the nginx source package from the official website and run the following command

    tar -zxvf nginx.tar.gz
    ./configure
    make && make install

usage:

	start: /usr/local/nginx/sbin/nginx
	stop: /usr/local/nginx/sbin/nginx -s stop
	reload: /usr/local/nginx/sbin/nginx -s reload


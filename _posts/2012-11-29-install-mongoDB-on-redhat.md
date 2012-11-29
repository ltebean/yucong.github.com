---
layout: post
category : mongo
tags : [beginner, tutorial]
---
{% include JB/setup %}



select suitable repo for your system and add one of following to /etc/yum.repos.d/10gen-mongodb repo:

    [10gen]
	name=10gen Repository
	baseurl=http://downloads-distro.mongodb.org/repo/redhat/os/x86_64
	gpgcheck=0


install stable version of MongoDB:

	yum install mongo-10gen mongo-10gen-server

edit /etc/mongod.conf file:
	
	vim /etc/mongod.conf

check and set basic settings, before starting MongoDB (default settings are good)

	logpath=/var/log/mongo/mongod.log
	port=27017
	dbpath=/var/lib/mongo

start mongoDB server:

	service mongod start
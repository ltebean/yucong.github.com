---
layout: post
category : nodejs
tags : [beginner, tutorial]
---
{% include JB/setup %}

### enable the repository

to enable this repository, simply download and install the release RPM:

    wget http://nodejs.tchol.org/repocfg/el/nodejs-stable-release.noarch.rpm
	yum localinstall --nogpgcheck nodejs-stable-release.noarch.rpm

### install

once enabled the repository,  install the compatibility symlinks and npm by running the following command:

	sudo yum install nodejs-compat-symlinks npm



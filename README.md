openshift-httpd-php
===================

This is a simple build script for setting up httpd server and php 5.6 on Red Hat's OpenShift platform.

How to start
------------

- let's pick up a name for our new app, hmmm, myapp!
- create a new app with rhc: `rhc app create myapp diy-0.1`
- go to the app's directory: `cd myapp`
- get the build script: `git pull -s recursive -X theirs https://github.com/mrinx/openshift-httpd-php.git`
- push the build script to the clouds: `git push`
- tadaa! wait, it's not done yet, take a coffee, watch your favorite TV show, check again in an hour
- yop, something got broken, let's restart the build process: `rhc app deploy master`
- tadaa! wait again, get a coffee, watch some TV show. If the process doesn't finish successfully, repeat the previous step (not that coffee one)
- tadaa! tadaa! check your application in the web browser, phpinfo should appear

I got inspired by similar scripts written by boekkooi (https://github.com/boekkooi/openshift-diy-nginx-php)

openshift-httpd-php
===================

This is a simple build script for setting up httpd server and php 5.6 (with yaf and phalcon php framework extensions and mongo php driver as modules) on Red Hat's OpenShift platform.

How to start
------------

0. let's pick up a name for our new app, hmmm, `myapp`!
1. create a new app with rhc: `rhc app create myapp diy-0.1`
2. go to the app's directory: `cd myapp`
3. get the build script: `git pull -s recursive -X theirs https://github.com/mrinx/openshift-httpd-php.git`
4. push the build script to the clouds: `git push`
5. tadaa! wait, it's not done yet, take a coffee, watch your favorite TV show, check again in an hour
6. yop, something got broken, let's restart the build process: `rhc app deploy master`
7. tadaa! wait again, get a coffee, watch some TV show; if the process doesn't finish successfully, repeat the previous step
8. tadaa! tadaa! check your application in the web browser, phpinfo should appear

I got inspired by similar scripts written by [boekkooi](https://github.com/boekkooi/openshift-diy-nginx-php)

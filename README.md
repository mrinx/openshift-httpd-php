httpd + php 5.6 on OpenShift
============================

This is a simple build script for setting up httpd server and php 5.6 (with yaf and phalcon php framework extensions and mongo php driver as modules) on Red Hat's OpenShift platform.

Installation
------------

0. Let's pick up a name for our new app; `myapp`!
1. Create a new application: `rhc app create myapp diy`.
2. Go to the app's directory: `cd myapp`.
3. Get a build script from this repo: `git pull -s recursive -X theirs https://github.com/mrinx/openshift-httpd-php.git`.
4. Push your app to the clouds: `git push`.
5. Tadaa! Wait, we're not done yet, take a coffee, watch your favorite TV show for a bit, and check the building process in an hour or so.
6. Yop, something got broken, let's start the build process again: `rhc app deploy master`.
7. Tadaa! Wait again, get a coffee, watch some TV show; if the process doesn't finish successfully, repeat the previous step.
8. Tadaa! Tadaa! Check your application in the web browser, information about your php configuration and set up should appear.

I got inspired by similar project by [boekkooi](https://github.com/boekkooi/openshift-diy-nginx-php).

I'm currently in a phase of eliminating bashisms from my scripts.

Welcome to cf-redis-commander!
===================

Overview
-------------

Wrapper of redis-commander for cloud foundry.
Thanks to https://github.com/joeferner/redis-commander/.

----------
Deployment to Cloud Foundry
-------------
1) git clone this repository,
```
git clone https://github.com/jimbasler-pivotal/cf-redis-commander
cd cf-redis-commander
```
Remember to install [cf cli](https://github.com/cloudfoundry/cli/releases) and then get an account from [Pivotal Web Services](http://run.pivotal.io/).

2) Push the application:
```
cf push --no-start
```
3) Bind redis service to this app.

4) Change the env variable SERVICE_NAME to the bound service instance name.

5) You can access your app at 
```
http://<random route>.cfapps.io
```
6) Login with 'admin' and 'pass' unless you changed it in index.js

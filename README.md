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
git clone https://github.com/Aswin3405/cf-redis-commander
cd cf-redis-commander
```
    Remember to install [cf cli](https://github.com/cloudfoundry/cli/releases) and then get an account from [Predix.io](https://www.predix.io/).

2) Remember to change REDIS_TLS to true if the redis instance supports TLS in the manifest.yml

3) Push the application:
```
cf push --no-start
```

4) Bind redis service to this app.

5) Change the env variable SERVICE_NAME to the bound service instance name.

6) Start the app.
```
cf restart cf-redis-commander
```

7) You can access your app at 
```
http://<random route>.run.aws-usw02-pr.ice.predix.io
```

8) Login with 'admin' and 'pass' unless you changed it in index.js

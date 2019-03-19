# Node.js Process Manager

The most challenging aspect when it comes to maintaining an application is keeping it alive and running. Additionally with Node.js, scaling a single threaded process can be hard to do; that’s where Process managers comes in.

#### Process Managers out there

* PM2
* SystemD - https://en.wikipedia.org/wiki/Systemd
* Forever - https://github.com/foreverjs/forever
* StrongLoop's Process Manager - http://strong-pm.io/

#### PM2

PM2 is a battle tested, production ready runtime and process manager for Node.js applications. It comes with a built-in load balancer, as well, which makes scaling applications even easier. Best of all, it works on Linux, Windows, and macOS. You specify the process.json file and PM2 takes care of the rest.

What all of this means is that PM2 allows you to keep your Node.js applications alive forever, and to reload them with zero downtime when you have updates to your application or server.

##### Cheatsheet - Process Management

```
$ pm2 start process_prod.json  # Start process(es) via process JSON file
$ pm2 ls                       # Show a list of all applications
$ pm2 stop <app>               # Stops a specific application
$ pm2 start <app>              # Starts a specific application
$ pm2 <app> scale N            # Scales the application to N number of instances (up or down)
$ pm2 kill                     # Kills all running applications
$ pm2 restart                  # Restarts all running applications
$ pm2 reload                   # Reloads the app configuration (handy when you modify environment variables)
```

##### Cheatsheet - Log management & Monitoring

```
$ pm2 monit            # return a rich set of data around your application’s health
$ pm2 logs             # Outputs logs from all running applications
$ pm2 logs <app>       # Outputs logs from only the app application
$ pm2 flush            # Flushes all log data, freeing up disk space
$ pm2 install pm2-logrotate    # enable log rotation
```

#### References

```
https://hackernoon.com/running-pm2-node-js-in-production-environments-13e703fc108a
https://pm2.io/doc/en/runtime/overview/
https://pm2.io/doc/en/runtime/guide/log-management/
```




This is munin plugin for count of Capistrano(v3) deploy count of day.


# How to setup

```
# curl https://raw.githubusercontent.com/takeshiyako2/munin-capistrano_deploy/master/capistrano_deploy -O /usr/share/munin/plugins/capistrano_deploy
# ln -s /usr/share/munin/plugins/capistrano_deploy /etc/munin/plugins/capistrano_deploy
# emacs /etc/munin/plugin-conf.d/munin-node
[capistrano_deploy]
env.log /home/<you>/<your app>/revisions.log
# service munin-node restart
# cd /etc/munin/plugins/
# munin-run capistrano_deploy
count.value 2
```



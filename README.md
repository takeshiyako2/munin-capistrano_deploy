This is munin plugin for count of Capistrano(v3) deploy of day.


# How to setup

```
# cd /usr/share/munin/plugins/
# wget --no-check-certificate https://raw.githubusercontent.com/takeshiyako2/munin-capistrano_deploy/master/capistrano_deploy
# chmod +x capistrano_deploy
# ln -s /usr/share/munin/plugins/capistrano_deploy /etc/munin/plugins/capistrano_deploy
# emacs /etc/munin/plugin-conf.d/munin-node
[capistrano_deploy]
env.log /home/<you>/<your app>/revisions.log
# munin-run capistrano_deploy
count.value 2
# service munin-node restart
```


# AUTHOR

Contributed by Takeshi Yako
https://github.com/takeshiyako2

# LICENSE

MIT


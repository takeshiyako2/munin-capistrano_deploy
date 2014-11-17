## How to setup

```sh
# ln -s /usr/share/munin/plugins/capistrano_deploy /etc/munin/plugins/capistrano_deploy
# emacs /etc/munin/plugin-conf.d/munin-node
[capistrano_deploy]
env.log /home/<you>/<your app>/revisions.log
# service munin-node restart
# cd /etc/munin/plugins/
# munin-run capistrano_deploy
count.value 2
```

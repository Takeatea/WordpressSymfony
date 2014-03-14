README
======

Setup
-----

Clone repository
```Shell
git clone git@github.com:Takeatea/wordpress.git your-project
cd your-project
git submodule update --init
cd wordpress
cp wp-config-sample.php wp-config.php
```

Don't forget to update database settings and languages settngs (French translations are already loaded).

Update Wordpress
----------------

```Shell
cd wordpress
git checkout 3.8.1
```
# Wordpress'n'Tea


## The Tea way to Wordpress.

Here is the "Tea way to Wordpress" from the [official Wordpress git repository](https://github.com/wordpress/wordpress) using command lines.


## Summary

+ [1) Install](#1-install)
+ [2) Configuration](#2-configuration)
+ [3) All about Curl](#3-all-about-curl)
+ [4) That's all folkes!](#4-thats-all-folkes)
+ [5) Update](#5-update)
+ [6) Authors](#6-authors)
+ [7) Copyright and license](#7-copyright-and-license)


### 1) Install

**To get started**, checkout or download the https://github.com/Takeatea/wordpress package into your `docroot`

```Shell
git clone git@github.com:Takeatea/wordpress.git your-project
```

Access to your `your-project` folder and get the [official Wordpress git repository](https://github.com/wordpress/wordpress) as a submodule, and checkout the 3.8.1 tag

```Shell
cd your-project
git submodule update --init
cd wordpress
git checkout 3.8.1
cd ..
```

Make your own `wp-config.php` as Wordpress asked

```Shell
cp wp-config-sample.php wp-config.php
```


### 2) Configuration

Edit your new `wp-config.php` and set the `DB_NAME`, `DB_USER`, `DB_PASSWORD` and `DB_HOST` from line 27 to 36.  
Go now to your website front page `your_wp_website.com` and follow the Wordpress instructions.


### 3) All about Curl

Your last step is to define your Authentication Unique Keys and Salts... using `curl` command.  
NOTA: if `curl` command is not installed, you can visit the page https://api.wordpress.org/secret-key/1.1/salt/ and get your variables.

```Shell
curl https://api.wordpress.org/secret-key/1.1/salt/
```

Copy and paste the response into your `wp-config.php` file, from line 53 to 60.


### 4) That's all folkes!

Here is the latest step: check your website

+ Go to your `your_wp_website.com/wordpress/wp-admin`
+ Log in to your admin panel

That's all to begin working with the **Tea way to Wordpress**


### 5) Update

To update your Wordpress CMS, simply go to your Wordpress folder and checkout the wanted version

```Shell
cd wordpress
git checkout 3.8.x
```


### 6) Authors

**Take a Tea**

+ http://takeatea.com
+ http://twitter.com/takeatea
+ http://github.com/takeatea

**Nicolas Assing**

+ http://fr.linkedin.com/pub/nicolas-assing/21/3b3/769
+ http://twitter.com/nicolassing
+ http://github.com/nicolassing


### 7) Copyright and license

Copyright 2014 [Take a tea](http://takeatea.com "Take a tea")  
Brewed by Take a tea ;)

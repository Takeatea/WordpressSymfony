# TEA WordpressSymfony
## Introduction
This application allow you to easily integrate Wordpress into a Symfony application

## Installation
### Code
- Clone the repository `git clone git@github.com:Takeatea/WordpressSymfony.git ./MyAwesomeProject`
- Install wordpress `git submodule update --init`
- Copy `./wp-config-sample.php` file to `./wp-config.php` and edit the values
- Edit the values for EkinoWordpressBundle configuration in `symfony/app/config/config.yml`
- `cd` into symfony directory and install the vendors. 

### Web server
Your document root must be point to `./symfony/web` directory. The index file should be, `index.php`.

## Misc
For further configuration, please read the [EkinoWordpressBundle documentation](https://github.com/ekino/EkinoWordpressBundle).

### Versionning
In order to push the code to your own repository, run the following command :
```bash
git remote set-url origin git@myhost/my-repo.git
git push -u origin master
```

### Recomandations
In order to have a better control on wordpress core, wordpress plugins, or wordpress themes, we advice to disable backend user upgrades and to use them as submodules.

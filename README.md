# Docker-compose.yml file for WordPress

## Usage

* Install docker from [https://www.docker.com/](https://www.docker.com/)
* Clone this repo
* Run `docker-compose up`

## Themes & plugins development

This is a really simple environment for themes & plugins development. Nothing fancy. Please be aware that:

* Your WordPress installation will be available at `http://localhost:8000`
* the `wp-content` folder you'll find in this repo will be shared with the WordPress installation, put your code there.

## Extra Notes

##### fix wordpress asking for ftp credentials when trying to add files (plugin install, upload media)
* add this define to wp-config.php ` define('FS_METHOD','direct'); ` allready applied, see use of WORDPRESS_CONFIG_EXTRA variable in docker-compose.yml
https://hub.docker.com/_/wordpress


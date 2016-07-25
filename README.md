# Quick Wordpress Installation using WP CLI

## Prerequisites
Install WP-CLI: https://wp-cli.org/docs/installing/


***


## Steps

### 1. Download Wordpress
`wp core download`

### 2. Create Database
Log in PHPmyadmin and create UTF-8 General CI database.

### 3. Install Wordpress
First, run the following command to create wp-config.php file.

`wp core config --dbname=wordpress --dbuser=root --dbpass=root`

The above command assumes that, you previously have created a database named wordpress. Change the database name with the one that you have created for the WordPress site.

Next, we use wp core install command to install WordPress. This commands the following parameters:

--url The website address url, e.g. http://localhost:8888/wordpress/.
--title The website title, e.g. My Blog.
--admin_user The admin username. It should be all in lowercase, e.g. admin.
--admin_password
--admin_email

Type the command below. Swap the parameters value as per your own setup.

`wp core install --url=http://localhost.dev/ --title=WordPress --admin_user=myusername --admin_password=mypassword --admin_email=name@gmail.com`

### 3. Install optional language(s)

`wp core language install cs_CZ`

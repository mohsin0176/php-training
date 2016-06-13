# PHP
>_[Training](https://github.com/simplonco/training) / PHP_

![PHP](php.png)

## Exercises

* [Cooking data with PHP](https://github.com/simplonco/php-cooking-data) _Learn how to play with the dictionary and an example dataset of movies in PHP! :egg:_
* [Send Mail Form](https://github.com/simplonco/php-send-mail-form) _Send mails with a simple HTML form and a PHP backend! :mailbox:_
* [Challenges](https://github.com/simplonco/php-challenges) _It will maybe hurt a bit, but for your good! :cactus:_

## Resources

### Official Documentation

* [The PHP Official Manual](http://php.net/manual/en/index.php) :uk:
* [Le Manuel PHP Officiel](http://php.net/manual/fr/index.php) :fr:

### Big Books

* [PHP The Right Way](http://www.phptherightway.com/) :uk:

### Learn X in Y minutes

* [Learn PHP in Y minutes](https://learnxinyminutes.com/docs/php/) :uk:
* [Apprendre PHP en Y minutes](https://learnxinyminutes.com/docs/fr-fr/php/) :fr:

### Digital Ocean Tutorials

* [How to install LAMP](https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04) :uk:
* [How to install LLMP](https://www.digitalocean.com/community/tutorials/how-to-install-the-llmp-stack-linux-lighttpd-mysql-and-php-on-ubuntu-12-04) :uk:
* [How To Change Your PHP Settings](https://www.digitalocean.com/community/tutorials/how-to-change-your-php-settings-on-ubuntu-14-04) :uk:
* [How to install PHPMyAdmin](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-16-04) :uk:

### OpenClassrooms

* [Concevez votre site web avec PHP et MySQL](https://openclassrooms.com/courses/concevez-votre-site-web-avec-php-et-mysql) :fr:
* [Programmez en orienté objet en PHP](https://openclassrooms.com/courses/programmez-en-oriente-objet-en-php) :fr:
* [Découvrez le framework PHP Laravel](https://openclassrooms.com/courses/decouvrez-le-framework-php-laravel-1) :fr:
* [Évoluez vers une architecture PHP professionnelle](https://openclassrooms.com/courses/evoluez-vers-une-architecture-php-professionnelle) :fr:

### Google Docs

* https://docs.google.com/a/simplon.co/document/d/1RvkdTdjyl0Z6mY5cU-DV0y39BJNkgUC_Gwcb0KySmiI
* https://docs.google.com/document/d/1wIrS26TAZYIFIJ8o11sj-ZvhgbVgBlTdyN8-41RiZ_0

_To be continued.._

## Code snippets

### PHP Setup :tada:!

```markdown
# Install LAMP
sudo apt-get install tasksel
sudo tasksel install lamp-server
# Fix a permission issue
sudo chown -R www-data:www-data /var/www
```

### What's mean LAMP?

```markdown
# LAMP: Linux Apache MySQL PHP

*apache2: Handle HTTP Request | nginx
*php5: Templating language | python | ruby
*mysql: Local Database (SQL) | postgresql | mongodb | rethinkdb
```

### Where is my PHP?

```php
<!-- HTML CODE -->
<?php
    ...
?>
<!-- HTML CODE -->
```

### URLS, PROTOCOLS & REQUESTS

```markdown
# URLS

http://www.google.com/doodle/page.html

# PROTOCOLS

* http
* ftp
* ssh

# REQUESTS

HTTPS = HTTP + SSL

METHODS:
- GET
- POST

## Google example of GET method
?gferd=cr&ei=eVpRV5r4Ooru8wfn-bqwAQ&gwsrd=ssl#q=test

?...=...&...=...&...=...

https://www.google.fr/?q=cookie
https://www.google.fr/?q=pizza
```

### `index.php`

```php
<?php
if ($_POST['password'] != "cookie") { // => database
    header('Location: form.html');
} else {
?>
<!DOCTYPE>
<html>
    <head>
        <meta charset="utf8" />
        <title>PHP Test</title>
    </head>
    <body>
        <h1>Welcome <?php echo $_POST['name']; ?>!</h1>
    </body>
</html>
<?php
}
?>
```

### `form.html`

```php
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf8"/>
        <title>PHP Form Example</title>
    </head>
    <body>
        <form action="index.php" method="POST">
            <input name="name" type="text" />
            <input name="password" type="password" />
            <input value="login" type="submit" />
        </form>
    </body>
</html>
```

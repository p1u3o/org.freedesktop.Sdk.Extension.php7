# org.freedesktop.Sdk.Extension.php7

This extension adds PHP support to Flatpak. 

You can access it at `/usr/lib/sdk/php7`. If you want to setup VSCode to use the PHP binary inside you can use `/usr/lib/sdk/php7/bin/php`

Includes

* [php](https://php.net/) (7.3.6)
* [composer](https://github.com/composer/composer) (1.8.6)
* [xdebug](https://xdebug.org/) (2.7.2)
* [phpcbf/phpcs](https://github.com/squizlabs/PHP_CodeSniffer) (3.4.2)
* [php-cs-fixer](https://github.com/FriendsOfPHP/PHP-CS-Fixer) (2.15.1)

You can place your own ini files in `$HOME/.config/php/ini/`

#### Troubleshooting
`/usr/bin/env: ‘php’: No such file or directory`

Run `. /usr/lib/sdk/php7/enable.sh` or add `/usr/lib/sdk/php7/bin` to your $PATH.

Hopefully in the future there is an organised way for extensions to add to the path. See this [related issue](https://github.com/flathub/com.visualstudio.code/issues/72).

#### Modules

```bash
bash-4.4$ php -m
[PHP Modules]
bcmath
calendar
Core
ctype
date
dba
dom
exif
fileinfo
filter
ftp
hash
iconv
intl
json
libxml
mbstring
mysqlnd
openssl
pcntl
pcre
PDO
pdo_sqlite
Phar
posix
Reflection
session
SimpleXML
sockets
SPL
sqlite3
standard
sysvmsg
sysvshm
tokenizer
wddx
xdebug
xml
xmlreader
xmlwriter
zlib

[Zend Modules]
Xdebug
```
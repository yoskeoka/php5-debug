# How to start php debug server

specify your local ip address.
```
ip a // linux, macOS
ipconfig // windows
```

modify IP address in docker-compose.yml file.

```sh
docker-compose build
docker-compose up
``` 
output messages look like
```
Recreating phpdebug_php-debug_1 ... 
Recreating phpdebug_php-debug_1 ... done
Attaching to phpdebug_php-debug_1
php-debug_1  | httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.3 for ServerNam
```

access http://172.17.0.3/phpinfo.php

# Reference
https://github.com/nickistre/docker-lamp/tree/centos-6.6

https://gist.github.com/chadrien/c90927ec2d160ffea9c4
## nginx-TEST
~~~
Bastille template to build nginx-TEST-final
- nginx, goaccess, letsencrypt
~~~

## Status
~~~
~~~

## TODO
~~~
~~~

## Required host commands
~~~
mkdir -p /usr/local/jails/share/ule-letsencrypt
mkdir -p /usr/local/etc/www
mkdir -p /usr/local/jails/nginx-TEST/ule-nginx
~~~

## Required mount points
~~~
MOUNT /usr/local/jails/share/ule-letsencrypt usr/local/etc/letsencrypt nullfs ro 0 0
MOUNT /usr/local/jails/nginx-TEST/ul-www usr/local/www nullfs rw 0 0
MOUNT /usr/local/jails/nginx-TEST/ule-nginx usr/local/etc/nginx nullfs rw 0 0
~~~

## Bootstrap
~~~
bastille bootstrap https://github.com/adriel-tech/FreeBSD13-BastilleBSD-Tips
bastille template TARGET-JAIL FreeBSD13-BastilleBSD-Tips/nginx-TEST-final
~~~

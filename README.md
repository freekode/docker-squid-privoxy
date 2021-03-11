# Docker squid and privoxy

docker-compose with squid and privoxy. Squid configured with privoxy as parent proxy

Test is squid and privoxy working
```shell
curl -x http://<ip>:13128 -L https://google.com
```

Test is privoxy working
```shell
curl -x http://<ip>:18118 -L https://google.com
```

Thanks to these repos  
https://github.com/sameersbn/docker-squid  
https://github.com/rafacouto/docker-privoxy

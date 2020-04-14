Nginx Ingress Controller


### 확인
```
curl http://[lb_ip]/coffee
curl http://[lb_ip]/tea
```

```
Server address: 10.100.3.48:8080
Server name: coffee-67c6f7c5fd-c58l2
Date: 07/Apr/2020:08:24:27 +0000
URI: /coffee
Request ID: e831901e441303ad59fb02214c49d84a
```

```
Server address: 10.100.2.24:8080
Server name: tea-7df475c6-lxqsx
Date: 07/Apr/2020:08:25:03 +0000
URI: /tea
Request ID: 59303a5a5baa60802b463b1856c8ce8d
```

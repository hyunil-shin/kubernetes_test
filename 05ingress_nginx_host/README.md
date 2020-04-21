Nginx Ingress Controller


### 확인
```
[centos@shi-kubectl 05ingress_nginx_host]$ curl --resolve coffee.cafe.example.com:80:133.186.154.73 http://coffee.cafe.example.com/
Server address: 10.100.3.6:8080
Server name: coffee-67c6f7c5fd-5pnvt
Date: 14/Apr/2020:09:14:49 +0000
URI: /
Request ID: 706a90c919f538252394da9ed7036e68


[centos@shi-kubectl 05ingress_nginx_host]$ curl --resolve tea.cafe.example.com:80:133.186.154.73 http://tea.cafe.example.com/
Server address: 10.100.3.7:8080
Server name: tea-7df475c6-ntdmg
Date: 14/Apr/2020:09:15:18 +0000
URI: /
Request ID: 5567b3337aec4629c12ca1884730878a
```

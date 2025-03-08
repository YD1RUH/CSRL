# CSRL
an example C used to build server, reverse proxy, and load balancer multiple server

## what is this ?
1. `http_server` just an example http server build using C.
2. `single_server_reverse_proxy` an example reverse proxy build using C, also work with php.
3. `multiple_server_reverse_proxy_balancer` an example reverse proxy build using C with round-robin method to distribute request with multiple server, also work with php too.

## how to use ?

### http_server
- just run `server.exe <IP Address> <Port>` then your http server ready to use.

### single_server_reverse_proxy
- run `server.exe <IP Address> <Port>` or you can use php server like `php.exe -S <IP Address>:<port>`.
- run `reverse_proxy.exe <IP Inbound> <Port Inbound>`.
- your reverse proxy ready to use.

### multiple_server_reverse_proxy_balancer
- run `server.exe <IP Address> <Port>` or you can use php server like `php.exe -S <IP Address>:<port>`. you can run another server with same IP Address but must different port.
- edit the file configuration `config.json` to match with server and port that your server run.
- run `reverse_balancer.exe <IP Inbound> <Port Inbound>`
- your load balancer ready to use.

## Motivation
it's just a hobby, challenging my self to creat something more efficient and practical.
73

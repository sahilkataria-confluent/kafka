# kafka load balancer config

## Install Nginx Package
```bash
sudo apt install nginx-core
```

## Update /etc/nginx/nginx.conf file based upon this template file:  [`nginx.conf`](nginx.conf)

1. Update Broker DNS entries in stream block

2. Update backend ip and port for each broker  

## Start Nginx Service
```bash
sudo systemctl restart nginx
```



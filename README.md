# kafka load balancer config

## Install Nginx Package
```bash
sudo apt install nginx-core
```

## Update /etc/nginx/nginx.conf file based upon this template file:  [`nginx.conf`](nginx.conf)
> Update Broker DNS entries in stream block
> Update backend ip and port for each broker  

```bash
sudo systemctl restart nginx
```



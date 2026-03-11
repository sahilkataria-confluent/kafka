# Kafka load balancer Setup

## Setup Kafka Cluster
1. Install Python 3.11 and Ansible 11.x and bcrypt modules
   
2. Modify hosts.yaml inventory file and add unique ports for each broker

3. Deploy Kafka Cluster
```bash
ansible-playbook -i hosts.yaml confluent.platform.all
```

4. Configure respective broker ip and port in nginx.conf file

## Install Nginx Package
```bash
sudo apt install nginx-core
```

## Update /etc/nginx/nginx.conf file based upon this template file:  [`nginx.conf`](nginx.conf)

1. Update Broker entries in stream block

2. Update backend ip and port for each broker  

## Start Nginx Service
```bash
sudo systemctl restart nginx
```


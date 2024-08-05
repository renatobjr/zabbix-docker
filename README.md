## Badges

![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)
![Static Badge](https://img.shields.io/badge/Docker_Compose-1.29.2-blue)
![Static Badge](https://img.shields.io/badge/Grafana-9-Orange)

# Zabbix + Docker

## Description

This project allows for easy deployment of a monitoring stack using Docker Compose. It includes:

- Zabbix server with MySQL database backend
- Zabbix web frontend with Nginx server
- Zabbix agent for monitoring systems
- Grafana with Zabbix plugin for data visualization

Official Documentation Links:

Zabbix: https://www.zabbix.com/manuals
Grafana: https://grafana.com/docs/grafana/latest/

## How to use

**1. Prerequisites:**

- Docker Engine and Docker Composed 2 installed.

**2. Clone this repository:**

```
git clone https://github.com/your-username/zabbix-grafana-docker.git
```

**3. Enviroment variables:**
This repository contains all env files need to running Zabbix Project. Fell free to set your own confs.

**4. Build and Run the stack:**

```
cd zabbix-grafana
docker compose up --build
```

This command will build the images (if not already built) and start all the services in detached mode.

**5. Accessing Zabbix Frontend:**
Zabbix web interface will be available on `http://your-ip-address:8080`

**6. Accessing Grafana:**
Grafana will be available on `http://your-ip-address:3000`

**7. Configuration:**

- Configure Zabbix server and agent according to your monitoring needs.
- Install the Grafana Zabbix plugin and configure the data source to connect to your Zabbix server.

**8. Additional Notes:**

- This configuration uses a private network for container communication.
- You can customize ports, volumes, and resource limits as needed.
- Remember to update environment variables with your specific credentials.

# Time Series Database System Laboratory (2022)


___
## Prerequisites and dependencies

- Ubuntu 18 or higher
- Docker version 20.10 (or higher)

___
## InfluxDB Installation
Downloading and installing InfluxDB
```bash
sudo docker pull influxdb:1.8
sudo docker run -p 8086:8086 influxdb:1.8 
```

Grafana Installation
```bash
docker run -d --name=grafana -p 3000:3000 grafana/grafana-oss:9.2.3-ubuntu
```

Plugin installation options could be found in https://grafana.com/docs/grafana/v9.0/setup-grafana/installation/docker/

Default username and passwords are 'admin'

Launch InfluxDB
```bash
influx
```

Test Connectivity: 
```bash
show databases
create database mydatabase
show databases
```

___
## Data Loading



___
## Running Queries



___
## Retention Policies



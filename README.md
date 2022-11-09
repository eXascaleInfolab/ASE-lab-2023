# Time Series Database System Laboratory (2022)


___
## Prerequisites and dependencies

- Ubuntu 18 or higher
- Docker version 20.10 (or higher)
- Clone this repository, you will need the data files. 
___
## InfluxDB Installation
Use the following run to download and run the InfluxDB v2.0 Docker image. Expose port `8086`, which InfluxDB uses for client-server communication over the `InfluxDB HTTP API`.
```bash
sudo docker run --name influxdb -p 8086:8086 influxdb:2.4.0
```
Or if it is already installed: 
```bash
sudo docker start influxdb
```

___
## Telegraf Installation
In a new terminal, Install Telegraf from the InfluxData repository with the following commands:
```bash
wget -qO- https://repos.influxdata.com/influxdb.key | sudo tee /etc/apt/trusted.gpg.d/influxdb.asc >/dev/null
source /etc/os-release
echo "deb https://repos.influxdata.com/${ID} ${VERSION_CODENAME} stable" | sudo tee /etc/apt/sources.list.d/influxdb.list
sudo apt-get update && sudo apt-get install telegraf
```




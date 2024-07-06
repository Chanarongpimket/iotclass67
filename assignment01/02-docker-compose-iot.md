# IoT Docker compose


## How to start docker compose

```bash sudo docker compose up

```

## Error we found

1. On docker-compose.yml Service zoonavigator-api & zoonavigator-web
2. when compose up get this error 'c:\:/rootfs:ro'
3. mongo can't connect 
4. setup.sh

## How to solve the problems.

1. Comment All Service On docker-compose.yml file zoonavigator-api & zoonavigator-web
2. copy path of iot file with command pwd
    go to docker-compose.yml 
    find c:\:/rootfs:ro' change to your path like /home/bmd/iot_event_streaming_architecture
3. Remove mongo latest version and downgrade version
    sudo docker compose down
    sudo docker rmi mongo
    sudo docker pull mongo:4.2
    go to docker-compose.yml change service mongo to mongo:4.2
4. go to /home/bmd/iot_event_streaming_architecture/grafana path
    RUN chmod 777 /home/bmd/iot_event_streaming_architecture/grafana/setup.sh
    
## Output

- [ ] IoT Sensor - Dashboards - Grafana 
- [ ] UI for Apache Ka
- [ ] Mongo Expr
- [ ] Node Expor
- [ ] Prometheus Time Series Collection and Processing Ser
- [ ] Prometheus Pushgateway
- [ ] ZooNavigator


### IoT Sensor - Dashboards - Grafana URL

### UI for Apache Kafka

### Mongo Express

### Node Exporter

### Prometheus Time Series Collection and Processing Server

### Prometheus Pushgateway

### ZooNavigator
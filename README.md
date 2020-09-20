
## Monitoring Stack
Stack de monitoramento exemplo para estudo.
 
### Containers

- Grafana
- Prometheus
- Node-exporter
- Alertmanager
- Cadvisor

### Iniciando e acessando Stack

```ssh
$ docker-compose up -d --build
```

### Acessando containers

```ssh
$ docker container ls
$ docker exec -ti container_name sh
```

### Acessando via Browser

- Grafana  [http://localhost:3000](http://localhost:3000) (admin/admin)
- Prometeus [http://localhost:9090](http://localhost:9090) 

### Documentação oficial para consulta
- Grafana Dasboards [https://grafana.com/grafana/dashboards](https://grafana.com/grafana/dashboards).
- Grafana Documentação [https://grafana.com/docs/](https://grafana.com/docs/)
- Prometheus [https://prometheus.io/](https://prometheus.io/)
- CAdvisor [https://github.com/google/cadvisor](https://github.com/google/cadvisor)
- Node-Exporter [https://github.com/prometheus/node_exporter](https://github.com/prometheus/node_exporter)
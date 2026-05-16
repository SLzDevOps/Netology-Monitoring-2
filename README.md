# Домашнее задание к занятию 14 «Средство визуализации Grafana» - `Фомичев Анатолий`

## Ссылка на Д3 - https://github.com/netology-code/mnt-homeworks/blob/MNT-video/10-monitoring-03-grafana/README.md

## Ссылка на репозиторий - https://github.com/SLzDevOps/Netology-Monitoring-2

### Скриншоты - https://github.com/SLzDevOps/Netology-Monitoring-2/tree/main/screenshots


### Ссылки на ресурсы:
````
https://www.dmosk.ru/miniinstruktions.php?mini=prometheus-stack-docker&ysclid=mp83nt5gx7575760902
https://habr.com/ru/companies/slurm/articles/314212/
https://docs.docker.com/guides/go-prometheus-monitoring/compose/
https://dev.to/rafi021/how-to-set-up-a-monitoring-stack-with-prometheus-grafana-and-node-exporter-using-docker-compose-17cc?ysclid=mp83oz4htm879389756
https://docs.tantorlabs.ru/tp/6.0/admin/monitoring_with_prometheus_and_grafana.html?ysclid=mp83oww4kd775069262
https://servermon.ru/blog/instrukcii-manualy/podrobnyy-gayd-razvertyvanie-grafana-prometheus-ehksportery-cherez-docker-compose.html?ysclid=mp83p14bgh834097163
````

### Команды-запросы сбора метрик
````
CPU Usage
  100 - (avg(rate(node_cpu_seconds_total{mode="idle"}[5m])) * 100)

Load Average
  node_load1
  node_load5
  node_load15

Filesystem-FreeSpace-%
  (node_filesystem_avail_bytes{mountpoint="/"} / node_filesystem_size_bytes{mountpoint="/"}) * 100

Memory-Free-MB
  node_memory_MemFree_bytes / 1024 / 1024

Network RX-TX
  rate(node_network_receive_bytes_total{device!~"lo|docker.*|veth.*"}[5m]) * 8 / 1000000
  rate(node_network_transmit_bytes_total{device!~"lo|docker.*|veth.*"}[5m]) * 8 / 1000000
````




![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_849.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_850.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_851.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_852.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_853.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_854.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_855.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_856.png).
![alt text](https://github.com/SLzDevOps/Netology-Monitoring-2/blob/main/screenshots/Screenshot_857.png).

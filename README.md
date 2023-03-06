# Metrics
docker compose project to collect and manipulate prometheus metrics

Prometheus generate random metric and sen it to telegraf by prometheus remote write protocol.
Telegraf receive metrics and write in out file configured in telegraf/telegraf.conf and into influxdb (can send to AWS S3?).
Fluentd read telegraf out file, transform the metrics and write in file both as is and tranformed version. Config in fluentd/fluent.conf
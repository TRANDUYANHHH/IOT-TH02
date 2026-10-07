# IoT pipeline performance report

Range: `-20m`

| Metric | Value |
|---|---:|
| Total messages | 54 |
| Accepted | 54 |
| Rejected | 0 |
| Duplicates | 0 |
| Observed duration (s) | 468.86 |
| Average throughput (msg/s) | 0.1152 |
| Payload received (bytes) | 9571 |
| Estimated payload rate (bytes/s) | 20.41 |
| MQTT ingest minimum (ms) | 1694.0 |
| MQTT ingest average (ms) | 101652.21 |
| MQTT ingest maximum (ms) | 201696.0 |
| DB write minimum (ms) | 15.78 |
| DB write average (ms) | 57.87 |
| DB write maximum (ms) | 187.21 |
| Processing average (ms) | 348.69 |

Notes:

- MQTT ingest is device timestamp to collector receipt.
- DB write is the synchronous InfluxDB write call duration.
- Payload bytes exclude InfluxDB index/metadata overhead; disk usage must be read from the Docker volume.
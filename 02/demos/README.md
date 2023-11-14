### How to run in Macos

## Run pull docker image of node-exporter
```bash
docker run -p 9100:9100 prom/node-exporter:latest 
```

## Then visit or do curl 

```bash
curl http://localhost:9100/metrics
```

## How to run prometheus on Macos 

Download darwin-arm64.tgz from here: https://github.com/prometheus/prometheus/releases/tag/v2.48.0-rc.2


## Make binary executable. 

```bash
## make binary executable
chmod +x ./prometheus
```


## Circumvent macos quarantine for downloaded binary from web

```bash
xattr -d com.apple.quarantine ./prometheus
```


## Change the scrape_targets on prometheus.yml

to a port where some exporter is running like `localhost:9100`


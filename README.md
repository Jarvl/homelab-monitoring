# homelab-monitoring
docker-compose file and configs for monitoring nodes in my homelab

## Setup

Ensure Docker is installed on the node.

### Install Netdata agent

Follow instructions to install [netdata-agent](https://learn.netdata.cloud/docs/netdata-agent/installation/linux) on the node directly. Not recommended to run in a container.

Install script:
```bash
curl https://get.netdata.cloud/kickstart.sh > /tmp/netdata-kickstart.sh && sh /tmp/netdata-kickstart.sh --disable-telemetry
```

### Create env files

Copy `*.env.example` files to `*.env` and define/change variables appropriately.

```bash
cp pihole_exporter.env.example pihole_exporter.env
cp plex_metrics_exporter.env.example plex_metrics_exporter.env
```

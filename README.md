# homelab-monitoring
docker-compose file and configs for monitoring nodes in my homelab

## Installing Netdata agent

https://learn.netdata.cloud/docs/netdata-agent/installation/linux/

```bash
curl https://get.netdata.cloud/kickstart.sh > /tmp/netdata-kickstart.sh && sh /tmp/netdata-kickstart.sh --disable-telemetry
```
# Netdata

Real-time performance monitoring for Linux, FreeBSD, and macOS.

## Features

- Interactive dashboards
- Zero configuration
- Metrics collection from various sources

## Quick Start

### Linux/macOS

```bash
curl -s https://my-netdata.io/kickstart.sh | bash
```

Open http://localhost:19999.

### Docker

```bash
docker run -d --name=netdata \
  -p 19999:19999 \
  -v /var/run/docker.sock:/var/run/docker.sock:ro \
  netdata/netdata
```

## Support

Visit [netdata.cloud](https://www.netdata.cloud) for more info.
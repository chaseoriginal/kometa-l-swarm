# kometa-l-swarm

Metadata manager for Plex libraries (Linux/Plex host).

## Stack

- **Host**: ore-dock-110-1
- **Stack**: `kometa-l-swarm`
- **Image**: lscr.io/linuxserver/kometa:latest
- **Config**: named volume `kometa-l-swarm.config`

## Deploy

```bash
ssh ore-dock-110-1
cd /data/compose/kometa-l-swarm
set -a && source .env && docker stack deploy -c docker-compose.yml --with-registry-auth kometa-l-swarm && set +a
```

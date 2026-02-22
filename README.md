```bash
chown -R 65534:65534 linx-data/meta && chown -R 65534:65534 linx-data/files
(set -a; source .env; envsubst <lilywhitebot/config.yml.template >lilywhitebot/config.yml)
```

```bash
NAPCAT_UID=$(id -u) NAPCAT_GID=$(id -g) docker compose up napcat
```

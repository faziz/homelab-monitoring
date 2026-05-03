# homelab-monitoring
Created this compose to set-up monitoring tools on my Synology box which normally sits idle. Unfortunately, Synoloy already occupies ports 80 and 443 so I couldn't run Traefik on default 80, and 443 ports.

Good thing about this configuration is, it uses DNS-01 challenge using Cloudflare. Therefore, I don't have to open up any port on my home firewall.

To run the command just use the following standard command.

```console 
docker compose --env-file ./.env up -d
```

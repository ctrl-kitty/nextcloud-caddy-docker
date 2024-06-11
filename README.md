# nextcloud-caddy-docker

# Requirements

- docker compose



# Installation & Running

1. Change pihole dns records in dns-pihole/etc-pihole/custom.list. Just set X.X.X.X to your host ip
2. Create .env file(example below)
3. docker compose build && docker compose up -d
4. Set your dns to docker host ip
5. Porfit. Pihole accessable on pihole.local & nextcloud on nextcloud.local

# .env example

```
TIMEZONE="Europe/Moscow"
# PIHOLE CONFIGURATION
PIHOLE_WEBPASSWORD=
# DB CONFIGURATION
DB_USER=
DB_PORT=5432
DB_PASSWORD=
DB_NAME=
# NEXTCLOUD CONFIGURATION
NEXTCLOUD_ADMIN_USER=
NEXTCLOUD_ADMIN_PASSWORD=
# if change, change caddyfile+dns record
NEXTCLOUD_HOST=nextcloud.local
```



# TODO:

- Autogenerate custom.list
- Autogenerate Caddyfile(insert domains)
- pihole domain?

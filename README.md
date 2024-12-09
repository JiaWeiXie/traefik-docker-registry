## Registry Basic Auth

### htpasswd
This file contains a user and password for accessing Basic-auth; note that this is not your tesla.com password. You can generate it on the web if you don't have the Apache tools installed (e.g. http://www.htaccesstools.com/htpasswd-generator/). Use BCrypt encryption mode.

.htpasswd file example:
```
test:$2y$10$/Lhsb2wpuLe9TKA2SpRCxOgFU/HZ209GYPt17ugE7phXarebFrKbG
test2:$2y$10$/Lhsb2wpuLe9TKA2SpRCxOgFU/HZ209GYPt17ugE7phXarebFrKbG
```

## Dotenv(.env)

```
REGISTRY_PROXY_USERNAME=
REGISTRY_PROXY_PASSWORD=
REGISTRY_DOMAIN=
CF_DNS_API_TOKEN=
```

## Install

1. Create cloudflare API token (DNS)
2. Create .env file
3. Create htpasswd file
4. Run `docker compose pull && docker compose up -d`

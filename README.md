# Traefik-v3 Docker Compose Template

This small public repo contains a `docker-compose.yml` with a working traefik- and an additional apache instance that can be used as a template.

The `docker-compose.yml` is heavily commented in order to make everything as clear as possible.

## Entrypoints and Redirections
- 3 entrypoint ports: `80` ( default HTTP), `443` (default HTTPS), `4444`
- The traefik dashboard is reachable via port `4444`
- All traffic from port `80 HTTP` is redirected to port `443 HTTPS`
- All traffic from port `4444 HTTTP` is redirected to port `4444 HTTPS` (same port)

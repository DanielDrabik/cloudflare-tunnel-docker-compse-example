
## Usage

1. Edit docker-compose and change `<cloudflare_token>` to your token from cloudflare zero-trust tunnel dashboard.
2. Add network docker 
```bash
docker network create tunnel
```
3. Run docker-compose
```bash
docker-compose up -d
```
4. Create other docker service with given example at `docker-compose.example.yml`
5. Create subdomain in cloudflare zero trust dashboard that directs to http://ip:docker_service_exposed_port url

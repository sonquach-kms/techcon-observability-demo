# techcon-observability-demo

1. Requirements

    - Docker compose
    - Loki Docker plugin
    - K6

2. Start application with docker-compose

   ```bash
   docker compose up -d
3. Send requests with [k6](https://k6.io/)
   ```bash
   # Send with 2 user in 5m 
   k6 run k6/k6-script_2vus-5m
   # Send with 4 user in 15m 
   k6 run k6/k6-script_4vus-15m
4. Endpoints
    - App a: http://localhost:8000
    - App b: http://localhost:8001
    - App c: http://localhost:8002
    - Prometheus: http://localhost:9090
    - Grafana: http://localhost:3000




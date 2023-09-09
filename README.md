## How to install

 Create prom cert files from vault in ./prometheus/
    - ca.crt
    - tls.crt
    - tls.key

Set password on following files:
----------------
./docker-compose.yml
./alertmanager/alertmanager.yml
./grafana/datasources/datasources.yaml
./unpoller/unpoller.conf

docker-compose up -d
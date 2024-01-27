## How to install

 Create secret/cert/prom and secret/cert/rootca cert files from vault in ./prometheus/
    - ca.crt # rootca
    - tls.crt # prom
    - tls.key # prom

Create vmware_password.txt in ./docker/secrets

<!-- Set password on following files:
----------------
./docker-compose.yml
./alertmanager/alertmanager.yml
./grafana/datasources/datasources.yaml
./unpoller/unpoller.conf -->

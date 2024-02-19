## How to install

 Create certs in ./prometheus/
    - ca.crt # rootca
    - tls.crt # prom
    - tls.key # prom

chmod 644 tls.key
vault kv get -mount=secret -field=crt cert/rootca > ca.crt
vault kv get -mount=secret -field=crt cert/prom > tls.crt
vault kv get -mount=secret -field=key cert/prom > tls.key
chmod 400 tls.key

Create vmware_password.txt in ./docker/secrets

Set password on following files:
----------------
./docker-compose.yml
./alertmanager/alertmanager.yml
./grafana/datasources/datasources.yaml
./unpoller/unpoller.conf

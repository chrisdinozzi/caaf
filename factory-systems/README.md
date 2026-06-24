# Factory Systems

|**Service**|**Image**|**Web UI**|**Purpose**|
|-------|-----|------|-------|
|NeuronEX|emqx/neuronex:3.7.1|neuronex.factory.home.lab|Gateway|
|HiveMQ CE|hivemq/hivemq-ce:2026.5|None|MQTT broker / UNS|
|Ignition|inductiveautomation/ignition:latest|ignition.factory.home.lab|SCADA / HMI / Historian|
|Caddy|caddy:2-alpine| None	| Reverse proxy / TLS termination|

## Deployment
```bash
mkdir -p ./secrets
echo "your-admin-password" > ./secrets/ignition_admin_password
chmod 600 ./secrets/ignition_admin_password
cp .env.example .env   # then edit with your licence key and timezone
```

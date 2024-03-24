# Dekaf for Apache Pulsar™

Dekaf is a proprietary visual user interface for Apache Pulsar: <https://dekaf.io>

Community forum: https://github.com/tealtools/dekaf/discussions

## Quick Start


- Please make sure that you have [Docker](https://docs.docker.com/get-docker/)
- Open your terminal
- Create a new directory: `mkdir dekaf && cd ./dekaf`
- Download the `docker-compose.yaml` file and start it:

```
wget https://raw.githubusercontent.com/tealtools/dekaf/main/docker-compose.yaml
docker-compose pull && docker-compose up
```

- Open <http://localhost:8090>
- Wait until Pulsar is ready
- Enjoy ☕️

<img width="1435" alt="Screenshot 2024-02-22 at 12 43 44 PM" src="https://github.com/tealtools/dekaf/assets/9302460/d224e725-48e2-4cad-a2c5-e2a94246362b">

### Demo Application

 We also run a demo application that produces data for two new tenants in this quick start.

If you don't see the `demo-schema-types` and `demo-shop` tenants in the tenant list, try to wait for a few seconds and reload the page.

If you want to disable the demo application, remove it from the `docker-compose.yaml` file.

### Troubleshooting

- We recommend ensuring that you have **6GB** or more Docker memory limit.
- If you have issues with file permissions:
  - Remove the data dir `rm -rf ./data`
  - Create data directory for Pulsar `mkdir -p ./data/pulsar`
  - Set the required file permissions by running `sudo chown -R 10000 ./data/pulsar`

## Configure

<https://www.dekaf.io/docs/dekaf/configuration-reference>

## Consume

<https://www.dekaf.io/docs/consume/consumer-session-tutorial>

🚧 The rest docs are under construction 🚧

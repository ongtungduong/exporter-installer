# Exporters installer for Ubuntu servers

Run the following command to install postgres exporter on your Ubuntu server:

```bash
bash <(curl -sSL https://github.com/ongtungduong/installers/raw/main/postgres-exporter/install.sh)
```

**You can customize the installation by setting environment variables:**

- EXPORTER_VERSION: To install specific version of postgres exporter (default: latest)
- EXPORTER_PORT: To specify a custom port (default: 9187)
- DB_HOST: To specify a custom database host (default: localhost)
- DB_PORT: To specify a custom database port (default: 5432)

**For example, to use port 17018, run the following command:**

```bash
EXPORTER_PORT="17018" bash <(curl -sSL https://github.com/ongtungduong/installers/raw/main/postgres-exporter/install.sh)
```

**Make sure that you run the queries to create the postgres exporter user and grant access to the user.**
